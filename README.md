# CND-Notes-week2
# Why access control

CIA
confidentiality
integrity
availablility

security featues to control user and systems and their control
protects system and resources from unauthorised acess
provide authorisation for transactions
broad trem coevering several mechanisms 

who has access?
systems also need access, humans need it.

Sample access control
system prompts user for password
user enters password
system authenticates user
User access a file
system checks the permission of a file
system grants/denies access to a file
-rw-rwx-rwx

subject = active entity
object = target

C
Ensures only authenticated and authorised entiites have access to information
I
ensure only authenticated entities with authorized transaction can modify information
A
Ensure only authenticated and authorised entitites modify systems in order to ensure availability

IAAA
Identification
ensure a subject is who they say they are
Authentication
the verification of the identiy of the subject against some other information
Authorisation
lookup of the authenticated subject and target object in the access matrix
Accountabillity
the maintaining of audit trails and other logging mearues to ensure accountabillity 

# Identification
The action of process of identifing someone or somthing or the fact of being identified
Subjects claimed identity must be verified
TWO phases
public claimed identity
private verification of claim

can be based on three primary factor
something you know password
something you have token
something you are biometrics

# Authentication
Passwords
oldest form of identity authorisation
most insecure due human element

Better passwords
password checkers
tested against criteria before being set, dictionaries, complexity, length
password generators
more secure hard to remeber
pronouncable passwords may be used
aging
expire and require changing
stops reuse

Better passwords 2
fact or opinion based challenge response
recovery teqniuqe
one-time passwords
system genereated

Graphical passwords
limited login attempts
raise an alarm if there is an incorrect entry, and limit further attempts

Salt
passphrases

# Token 
A physical pieces of hardware
build on the one time password
requires a pin and provide time synched OTP
other digital certificate
cryptographic keys
strong public key encryption is used to generate a key pair
identity authentication is based on they being a matching cryptograpic pair
SSH

Smart card has a functional CPU, weaker processing power
both have memory, simplet is an ATM card smartcards can be used as token.

Type 3
Face, Voice, Fingerprint, Behavioral, emerging
has to be appropriate to the enviroment
palm scan
hand geometry
hand topology
retina // invasive
iris scan less invasive
facial scan, computers have hard time
signature dynamics
keyboard dynamics
voice print
Effectiveness vs Acceptance

Biometrics Type 1 error false rejection rate
type 2 false acceptance rate
Cer crossover error

# Authorisation

Authentication validating an identy claim
Authorisation  the subject is allowed to preform action

access criteria should be fine grained
least priviledge
prenvent access creep
Roles
Groups
pyshical logical location
time of day
transaction type

Know your default
default allow
defualt deny

Need to know least privlidege
Access control methods
layered protection

physicol controls
technical controls
administrative control

access control types
preventive
detective
corrective
deterrent
recovery
compansation

auditing
provides for accountability
haveing logs without checks is worse then logs
users must know they are being monitored

Summary
access control is the first line of defence
critical to the CIA
can be varied
one size does not fit all.
