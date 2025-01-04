# ergonomics and I/O devices

Created: October 19, 2024 4:01 PM
Tags: LEC

# ergonomics

- ergonomics (or human factors) is the scientific discipline concerned with the understanding of the interactions among human and other elements of a system, and **the profession that applies theory, principles, data and methods to design in order to optimize human well-being and overall system performance**
    - design for humans in interaction with software and hardware, so to **optimize human well-being and overall system performance**

## system performance

- the ‘system’ is both the **human and the technical system in interaction** (not the technology alone)
- performance is determined by **effectiveness, efficiency, and effort** (of both humans and machines)
- efficiency is a **trade-off between speed and accuracy** (cf. fitts’ law)
- ‘optimal’ according to **human judgment** (users and other stakeholders)

## physical

- physical ergonomics is concerned with human anatomy, anthropometry (the measurement of human aspects), physiology and bio mechanical characteristics as they relate to **physical activity in work or daily life**

## cognitive

- **how do users expect the technology to work?**
- **how is information displayed?**
- **how well are stereotypical expectations met**
- **how complex is the interface?**
- **how much training is required?**
- **what user knowledge assumptions are met?**
- **how does information facilitate learning and memory?**

### how HCI is indebted to ergonomics

| user orientation | **design and application of tools, procedures, and systems must be user-oriented**, rather than just “task” oriented |
| --- | --- |
| diversity | **recognition of diversity in human capabilities and limitations**, rather than “stereotyping” workers/users |
| effect on humans | tools, procedures, and systems are not “inert”, **but do influence human behavior and well-being** |
| measurements | **empirical information and evaluation is key in design process**, rather than just use of “common sense” |
| scientific methods | **test and retest hypothesis with real data**, rather than “anecdotal” evidence or “good estimates” |
| system  | **objects, procedures, environments, and people are interconnected**, affect one another, and do not exist in “isolation” |

![Screenshot 2024-10-19 at 4.09.27 PM.png](ergonomics%20and%20I%20O%20devices%20124b756f81228011ac33c521b91a3d30/Screenshot_2024-10-19_at_4.09.27_PM.png)

> together, **I/O devices form the ‘user interface’**
> 

### mouses as pointing devices

| pros | cons |
| --- | --- |
| works in **small spaces** (trackballs are better?) | hand must be **removed from the keyboard** |
| can adjust **granularity of movement**, inexpensive | **require space beside keyboard movements** |
| user can keep eye on display | relative mode only |
| direct relationship between **hand and cursor movement on the dimensions of direction, distance, and speed** | **mechanical mice pick up dust and other debris** / **optical mice might not work on certain surfaces** (e.g., glass) |
| **diagonal and continuous movement**, spaced control | require a **certain amount of learned eye-hand coordination** (awkward and difficult for first-time users) |

# input devices

1. degree of freedom (DoF)
    - **the** **limits to which physical movement or other physical processes are possible**
2. joysticks (2D, like a mouse) 
    - left stick - 2 DoF
    - right stick - 2 DoF
3. drone (3D) 
    1. up / down, turn left / right, forward / backward

## touch screens

### pros

- **direct manipulation** (i.e., direct eye-hand coordination)
- several technologies to choose from, **including pressure-sensitive, resistive, infrared, capacitive**
- **faster and easier to learn** than other input devices (kids can use!)
    - **no command memorization** needed
    - user may be led through correct command sequence
    - good for **infrequent use**
    - **minimal training needed**, high user acceptance
- **continuous motion in all directions**
- no extra desk space and no moving parts

### cons

- very fast, **not very accurate**
    - “big” fingers
    - limited resolution
    - **difficult to select small targets**
    - **very slow text** and data entry
- finger/arm may **obscure screen**
- **overlays may lead to motion parallax**
- inadvertent activation
- **screen can get dirty** (oil from fingers)
- susceptible to temperature and humidity
- **arm fatigue** for conventional computer monitors
    - should be limited to low-frequency usage

## speech recognition

- conversion of spoken language to commands or data
- advantages over other input methods:
    - **more natural form of communication**, so less training required
    - **does not require the use of hands or other limbs**, so user can carry out multiple other actions
    - **opportunities for physically disabled users**

## monitoring devices

- cameras, mics, and similar devices that **allow interpretation of “natural" human activities**
    - observation of movements for a task
    - gestures
- requires distinction between:
    - **control activity** (signals to the computer that **something relevant is going to happen**)
    - **intentional activity** (**purposefully performed** within a task)
    - **spurious activity** (**activity unrelated to the task** at hand)

## eyetracker

- camera captures the **infrared reflection of a user’s cornea**
- **track eyeball rotations via calculation**
- often used in **usability and physiology experiments** (for recording and analysis of user attention)
- sometimes **used as input device** (e.g., selection of commands or letters by looking at them)

| heatmap | **red - more fixations
green - less fixations** |
| --- | --- |
| scanpath | **saccades** - **rapid, ballistic movements of the eyes** that abruptly **change the point of fixation**

**smooth pursuit movements** - **much slower tracking movements** of the eyes designed to keep a **moving stimulus on the fovea**

**(con)vergence movements** - **align the fovea of each eye with targets** located at **different distances** from the observer

**vestibulo-ocular movements** - **stabilize the eyes relative to the external world**, thus compensating for head movements |

## headtracker

- **head movement to convey control information to the computer** (limited range of movements)
- **keyboard is a display on the computer screen**
    - **the system detects slight movements of the user’s head and moves the cursor accordingly**
    - to operate a key, the user must locate the cursor, and then blow on a blow switch in the headset mouthpiece— this type of device can be used by severely impaired users

## brain computer interfaces

![Screenshot 2024-10-19 at 4.22.06 PM.png](ergonomics%20and%20I%20O%20devices%20124b756f81228011ac33c521b91a3d30/Screenshot_2024-10-19_at_4.22.06_PM.png)

### affective computing

- **emotions affect rational thinking** (e.g., decision making, perception, learning)
- computers should recognize, understand, and express emotions
- ideally, computers sample data from head pose, face, eyes (gaze), gestures, heart rate, EEG, etc. **to guess the mood a user is in and respond appropriately**
- a number of emotions may be regarded as ‘universal’ or ‘basic’ but which is still under debate
    - moreover, their expression may differ according to culture and individual
- further, interpretation of emotions is **situation or context dependent**

## kuleshov effect

- **same face, same expression, different context**

# output devices

## visual

| character-based displays | liquid- rystal displays (LCDs), flat-panel displays (FPDs)

**used in stationary devices, in telephones, calculators, etc** |
| --- | --- |
| graphics displays | cathode ray tubes (CRTs), LCDs, and other FPDs, 3D

**high-resolution graphic displays in stationary output devices (e.g., cockpits, helmet-mounted displays)** |
| printing devices | **color vs. b/w**, dot matrix, laser jet, inkjet

fax, plotters (colored pens)

3D printing |
| microfiche, micro-film, videotape | require old-school equipment to read |

## haptic (tactile)

### force feedback

- **very realistic in certain scenarios** (e.g., in the training of dentists)
- commercial products are widely available

### textural feedback

- generic feedback of textures is **hard to achieve**
- **sensory / perceptual illusions** can help create realistic textural feedback
    - **rubber hand illusion**
    - **haptic retargeting (use a single physical object to create the illusion of touching multiple virtual objects)**
    - **haptic proxy**

### thermal feedback

- **body transfer illusion**: the illusion of owning either a part of a body or an **entire body other than one’s own**
- embodiment - three sub-components:
    1. **sense of self-location** - a **determinate volume in space** where one feels to be located
    2. **sense of agency** - **the sense of having global motor control**, including the subjective experience of action, control, intention, motor selection, and the conscious experience of will
    3. **sense of body ownership** (your body is ‘yours’)

### haptic resolution

- different haptic devices can **render haptics in different resolutions**
- different body areas have **different spatial and temporal resolving capacity of haptics**
- virtual touch mouse for the **visually impaired** (mouse as output device)
    - the virtouch mouse has two **4 x 4 pin matrices for tactile feedback**
    - **texts can be read in braille (one character for each matrix)**
    - the virtouch mouse also **reacts on visual imagery by using contrasts** (dark colors against light colors) to offer a tactile representation (geographical maps)
    - together, these two functions may be used to **scan a display screen for text, layout, but is harder for images**

![Screenshot 2024-10-28 at 12.26.34 PM.png](ergonomics%20and%20I%20O%20devices%20124b756f81228011ac33c521b91a3d30/Screenshot_2024-10-28_at_12.26.34_PM.png)

> when evaluating the point-localization threshold, **a stimulus is presented to the skin, followed in time by a second stimulus that may or may not be applied to the same site**
> 

## sound

- **tone generators** (beeps, alerting tones)
- **alarms** (warning signals)
- **digitized speech** (digitally recorded human speech)
- **text-to-speech synthesis** (speech generated by concatenating basic speech sounds according to rules)
- **auditory icons** and “earcons”
    - **non-speech sounds to inform about current events** (e.g., empty trash, new mail, move, copy, delete)
    - should be optional (annoying, may disturb others)
    - corporate earcons (auditory logos), commercial brand-lining, distinctive music (e.g., mac startup sound, windows launch sound, “intel inside”
    
    ![Screenshot 2024-10-28 at 12.37.53 PM.png](ergonomics%20and%20I%20O%20devices%20124b756f81228011ac33c521b91a3d30/Screenshot_2024-10-28_at_12.37.53_PM.png)
    

| compatibility | signals should correspond to **natural sound experience** |
| --- | --- |
| approximation | two-stage signals should bring clear message

1) **basic meaning (e.g., attention)**
2) **higher meaning (where, what for, how)** |
| parsimony | signal should provide **only necessary information** |
| avoid extremes | **high intensity signals cause distraction** or disruption of response |
| environment | comply with **signal-to-noise ratio** |
| design trade-off | **invariance**: type of signal should be **constant in its meaning** (signal used for different purposes is bad → ambiguity!)

use interrupted or variable signals: humans adapt to signals and **might react less on those signals in the future**  |

### spatial audio

- issues:
    - **acoustic attention - spatial perception of the acoustic source**
    - **occlusion**
    - **reflection**

### advanced and futuristic

- the trend
    - blending input and output (e.g., tablets and phones, VR headsets, wearable gadgets, etc)
        - it becomes harder to **find a pure input/output device**
        - every gadget is a **“multimedia PC”** since the 90s
    - **more intuitive and natural interactions** (e.g., NLP, touch interface, motion-tracked controllers, etc.)
    - **multimodal interaction**
    - more **personalized** experience (potentially dangerous?)
- robotics, BCI, human augmentation

### personalized experiences

| handwriting recognition/personal assistants | 3M palm pilot, go corp., sony, toshiba |
| --- | --- |
| smart card | thin plastic card, **embedded processor and memory**

information about a user (e.g., employee ID, credit details, etc.) is stored on the card

**outputs information to special card readers** |
| biometric devices | advanced smart card that **contains characteristics about a user** such as fingerprints, voice prints, retina prints, or signature dynamics |
| texture sensation  | sandpaper system (MIT) - uses a motor-driven, force-feedback joystick that uses tiny virtual springs to **simulate motion while the user moves the joystick over patches of computationally created textures displayed on a screen** |
| gesture, speech, and gazing | **two-handed gesturing by voice, and selection by gaze (CMU)** |
| person tracking | active **badgeTM** system 
- **tracks people inside a building**
- used as a **communications device**
- can be turned off for privacy |

### wearables

- wearable computer
    - **private eyeTM** (reflection technology)
        - user wears a single high-resolution LCD over one eye, while looking out the other eye; **image projected at infinity**
        - coupled with a **portable computer, and other input devices**
    - **wearable computerTM** (computing devices international)
        - **portable, body-mounted, voice-activated computer**
        - tested in bosnia, presently being adopted by the U.S. armed services
    - **sixth sense**
        - **combination of camera and projector**
- **helmet-mounted display with speech interface**
    - military applications, “aim-fire” scenarios

### robotics and human augmentation

- compensate for **physical disability**
    - tissue-synthetic interfaces **connecting the biological body to a machine**
- compensate for **neurological conditions** (e.g., dementia, parkinson’s disease, etc.)

### smart living

- **smart rooms**
    - **can identify people and interpret their actions**
        - house that knows where your kids are and tells you if they are getting into trouble
    - can supervise students during exams
    - research being conducted globally
        - **person finder - pfinder**
            - video cameras to recognize faces, expressions, gestures
            - mics for speech recognition
- **smart home**
    - **performs activities according to user’s preferences** and usual actions

### smart textiles

- sort of a **personal assistant that you wear**
- **built-in computer, camera, microphones, other sensors**
- camera built into the **frame of eyeglasses that captures images**
- face-recognition software that tells you the name of the person you are looking at by whispering

# agency-centered design

- **bionic people**
- machines with biochips
- **the distinction between virtual and real humans becomes obsolete**— the transition is gradual
- ‘me’ as ‘identity of self’ is not restricted to the organic body anymore— parts can be exchanged or upgraded by technology
    - psychologically, people attribute agency (including emotion) to non-living artifacts
    - deliverance of a function is important, whether done by a human being or a machine is not
- **people attribute agency (including emotion) to non-living artifacts**