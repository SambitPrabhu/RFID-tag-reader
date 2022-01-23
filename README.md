# Keypad Door Lock
ArIES recruitment project for 1st year students.
We were initially given the project *RFID Tag Reader* but because its simulation was not possible on TinkerCad, we were given a different project : *Keypad Door Lock*.

                                                           *Problem Statement*
Nowadays, our society is facing a lot of issues and one of the prime issues to ponder upon is security. People tend to look for a solution that is reliable, sturdy, long-lasting, and also cost-effective. Modern technologies are expensive and therefore there are very few affordable security solutions in the market for people to buy for making their homes and valuables secure.

                                                              *Objective*
Our aim is to make an affordable, easy to use, reliable security door lock using Arduino and a keypad lock.

                                                       *How a Keypad Locks Work*
Instead of a key, this type of lock system requires a numerical code to grant entry to a facility or property. The code is punched in by users via a numerical pad, similar to those on a basic calculator that one uses. If the correct code is entered, the door lock should be released. Some mechanisms require batteries or a small electrical current in order to unlock.
Some keypad locks have an integrated security feature that keeps the door locked for a set amount of time ( 15 seconds or  minute ) after several incorrect attempts to enter the code.

*a. Keyless Entry and Exit*
The convenience of keyless entry is perhaps the most outstanding benefit of using a keypad lock. No fumbling around with keys when you’re trying to unlock your door at night, no calling a locksmith when you’re locked out of your house, no frantic search for your keys when you’re rushing to get out the door, no need for keys, period. Simply punch in your PIN number on the keypad and voila–you’re inside with no fuss and no muss. When it’s time to leave the house, a keypad lock will automatically lock behind you, essentially eliminating that all-too-common scenario where you’re halfway to work and wondering whether you locked the front door or not.

*b. Time-Determined Locking and Unlocking Schedules*
Time-determined access control, “scheduling”, is one of the most outstanding benefits of using a keypad lock. Business owners can schedule time periods for doors to be locked or unlocked in order to keep strict control over employee access to certain areas of the premises. Homeowners can ensure that their doors are always locked at night without having to make the nightly rounds to do so. The ability to set time-determined locking and unlocking schedules will save both time and money, and it will ensure a higher degree of safety and convenience versus using traditional locks and keys.

*c. Increased Security*
Mechanical keypad locks such as the Lockey 2835 offer a higher level of security in that they are pick proof and bump proof. Traditional locks are subject to both lock picking and lock bumping, the latter of which leaves no signs of forced entry, making it difficult to collect from your insurance company should a theft occur.

*d. Additional Safety for Kids*
Keypad locks eliminate the need for your child to keep up with a house key if they come home from school before you come home from work. During a busy school day, it’s relatively easy for a child to accidentally drop or otherwise misplace a house key, and if they’re locked out of the house when they come home from school, this poses a potential risk to their safety. With a keypad lock, all your child needs to have is their personal security code, and they can enter it into the keypad to unlock the front door. Once they’re inside, the keypad lock will automatically lock behind them. 

*e. Better Durability*
Traditional locks can get worn down and eventually malfunction due to frequent or heavy use. If you’ve ever had to deal with a lock that requires you to jiggle or shimmy the key just to get it to work, you know how aggravating it can be. Accidentally breaking a key off inside the lock can also be a pain to deal with. Keypad locks are remarkably durable because they don’t sustain the repetitive friction of inserting and turning keys; pressing a few buttons on the keypad is all that’s required to engage the lockset and open the door.

                                                               *Working*
1.	Firstly, we make the necessary connections among Arduino, breadboard, keypad lock, lcd screen, servo motor, buzzer and LED bulbs. For the code, we used some necessary libraries like <LiquidCrystal.h>, <Keypad.h>, <string.h>, <Servo.h> required for the components we used. 
The connections are as follows:
a)	All the analog pins (A0-A5) are connected to the LCD screen via the breadboard. Arduino controls all the output on the screen.
b)	The digital pin 11 is connected to the servo motor which locks and unlocks the door.
c)	The digital pins 2-9 are connected to the keypad lock for taking the input from it.


1. We set the system initially in such a way that it remains locked all the time until we open it with a proper passcode/ password.
2.	Now, we set a password for the door to unlock in the keypad lock ( here ABC123). Then, if we type the password correctly, the door will unlock with a message on  the lcd screen-“Unlocked” otherwise it will show “locked”. 
3.	Also on pressing the key ‘*’ on the keypad, the door gets locked instead of an automatic locking mechanism where usually the person must enter inside within a stipulated time interval ( the idea of fixing a stipulated time for the lock is not going to be good when multiple people need to enter the house where they need to unlock the door multiple times with the password). Clicking ‘#’ invokes master control over the device when the master key is entered. Now, required changes can be made to the device ( like changing password etc.).
As for the software simulation, we can do it on tinkercad circuit simulator as it has all the required components like Arduino, keypad lock, breadboard etc.
