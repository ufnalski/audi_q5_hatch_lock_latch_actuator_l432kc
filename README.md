# Audi Q5 (2019) tailgate pull-down motor [STM32L432KC]
The part number is [3V5827887B](https://allegro.pl/listing?string=3V5827887B).

![Audi Q5 tailgate pull-down motor in action](/Assets/Images/audi_q5_tailgate_pull_down_motor_in_action.jpg)
![Audi Q5 tailgate pull-down motor inner workings](/Assets/Images/audi_q5_tailgate_pull_down_motor_inside.jpg)

> [!NOTE]
> Sorry for a misleading filename :innocent: This repo is devoted only to the pull-down motor. The latching mechanism is a separate unit. The accompanying part number is [4M0827506D](https://allegro.pl/listing?string=4M0827506D). It's on my to-do list.

> [!TIP]
> I don't know the original external circuitry. In this simplified demo the pulling action stops after a pre-determined period of time has passed. My guess is that the original circuitry uses current sensing. Play with that concept in your version of the experiment. Some current sensors common among DIY-ers include [ACS712](https://www.allegromicro.com/-/media/files/datasheets/acs712-datasheet.ashx) and [ACS724](https://www.allegromicro.com/-/media/files/datasheets/acs724-datasheet.ashx).

# Pinout

| Pin # | Signal          |
|:-----:|:---------------:|
| 1     | Not connected   |
| 2     | Motor (+), 12 V |
| 3     | Switch C1       |
| 4     | Motor (-)       |
| 5     | Switch L1 (NO)  |
| 6     | Motor casing    |

> [!IMPORTANT]
> Both switch (position sensor) terminals are separate from the motor terminals - there is no need to introduce an optocoupler like [here](https://github.com/ufnalski/nissan_qashqai_j11_rear_wiper_motor_l432kc). There is one in the picture because I kept the setup from the previous exercise.

# Missing files?
Don't worry :slightly_smiling_face: Just log in to MyST and hit Alt-K to generate /Drivers/CMCIS/ and /Drivers/STM32L4xx_HAL_Driver/ based on the .ioc file. After a couple of seconds your project will be ready for building.

# Call to action
Create your own [home laboratory/workshop/garage](http://ufnalski.edu.pl/control_engineering_for_hobbyists/2025_dzien_popularyzacji_matematyki/Dzien_Popularyzacji_Matematyki_2025.pdf)! Get inspired by [ControllersTech](https://www.youtube.com/@ControllersTech), [DroneBot Workshop](https://www.youtube.com/@Dronebotworkshop), [Andreas Spiess](https://www.youtube.com/@AndreasSpiess), [GreatScott!](https://www.youtube.com/@greatscottlab), [bitluni's lab](https://www.youtube.com/@bitluni), [ElectroBOOM](https://www.youtube.com/@ElectroBOOM), [Phil's Lab](https://www.youtube.com/@PhilsLab), [atomic14](https://www.youtube.com/@atomic14), [That Project](https://www.youtube.com/@ThatProject), [Paul McWhorter](https://www.youtube.com/@paulmcwhorter), [Max Imagination](https://www.youtube.com/@MaxImagination), [Nikodem Bartnik](https://www.youtube.com/@nikodembartnik), [Stuff Made Here](https://www.youtube.com/@StuffMadeHere), [Mario's Ideas](https://www.youtube.com/@marios_ideas), [Aaed Musa](https://www.aaedmusa.com/), [Haase Industries](https://www.youtube.com/@h1tec), and many other professional hobbyists sharing their awesome projects and tutorials! Shout-out/kudos to all of them! Promote [README-driven learning](http://ufnalski.edu.pl/proceedings/sene2025/Ufnalski_PE_formatted_SENE_2025.pdf) :sunglasses:

> [!WARNING]
> Electric motors - do try them at home :exclamation:

220 challenges to start from: [Control Engineering for Hobbyists at the Warsaw University of Technology](http://ufnalski.edu.pl/control_engineering_for_hobbyists/Control_Engineering_for_Hobbyists_list_of_challenges.pdf).

Stay tuned!
