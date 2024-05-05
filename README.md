# ULTRON - Automatic Control of JTDX/WSJT-X/MSHV 📻

**Created by:** https://lu9dce.github.io/

**Copyright:** 2023 Eduardo Castillo  

**Contact:** castilloeduardo@outlook.com.ar  

**License:** https://creativecommons.org/licenses/by-nc-nd/4.0/

**I recommend AUTOSPOT:** https://github.com/lu9dce/autospot

**EASY FOR WIN DOWNLOAD** : 📥 [Ultron (WIN)](https://drive.google.com/drive/folders/1JYWeMY5giVzscMdtq1dMDu2BknGj-CeX?usp=sharing)

**DOWNLOAD** : 📥 [Ultron (Main Branch)](https://github.com/lu9dce/ultron/archive/refs/heads/main.zip)

"Remember that this software requires knowledge in both operating systems and PHP.

I have tested this program on Slackware 15.0, and other colleagues have tested it on Fedora and Debian, as well as on Windows.

I do not guarantee its functionality if the user lacks knowledge."

## [DONATE](https://www.paypal.com/donate/?hosted_button_id=WHG8FQRMAPA3E)

Ayuda en español en la [Wiki!](https://github.com/lu9dce/ultron/wiki).

![ultron](https://pbs.twimg.com/media/F23jEfzWYAApY9t?format=webp&name=small)

## Description

ULTRON is a sophisticated software tool designed for **remotely or locally controlling programs like JTDX, MSHV, and WSJT-X**. It offers seamless operation on both **Windows and Linux platforms**, supporting both 32-bit and 64-bit versions. The software relies on the **latest version of PHP** for optimal performance.

## Advantages of Using ULTRON

ULTRON offers a multitude of advantages as a **BOT** for controlling programs like JTDX, MSHV, and WSJT-X:

1. **Effortless Remote Control**: ULTRON empowers users with the ability to control radio programs remotely, eliminating the need for physical presence. This is particularly beneficial for scenarios where real-time adjustments and monitoring are required without being tied to a specific location.

2. **Enhanced Efficiency**: By automating repetitive tasks such as CQ calling and message recognition, ULTRON boosts operational efficiency. It can tirelessly manage communication, freeing up operators to focus on more strategic aspects of their radio activities.

3. **Seamless Integration**: ULTRON integrates seamlessly with both Windows and Linux platforms, providing a consistent and user-friendly experience across different operating systems. Its support for various versions ensures compatibility with a wide range of setups.

4. **Real-Time Adaptability**: The real-time functionality of ULTRON enables dynamic changes in software preferences without the need for frequent restarts. Users can switch between programs like JTDX, MSHV, and WSJT-X effortlessly, adapting to changing communication needs on the fly.

5. **Automated Logbook Management**: ULTRON's dedicated logbook management ensures accurate tracking of QSOs. The ability to use a personalized logbook while keeping it separate from other software simplifies record-keeping and QSO verification.

6. **Intelligent Decision-Making**: ULTRON's ability to identify messages, respond to correspondents, and manage waitlists demonstrates its intelligence in making informed decisions during communication. It streamlines the QSO process, increasing the chances of successful interactions.

7. **Signal Strength Assessment**: ULTRON's consideration of signal strength enhances QSO success rates. By taking into account signals weaker than -20dB, it assists in prioritizing communications with better chances of success.

8. **Visual Feedback**: For Raspberry Pi users, the LED control and audible tone features provide visual and audio feedback, enhancing user awareness of ongoing operations and the status of the communication process.

In summary, employing ULTRON as a BOT for radio program control offers an array of benefits, ranging from operational efficiency and adaptability to intelligent decision-making and enhanced communication success rates. Its seamless integration, real-time capabilities, and intelligent automation make ULTRON a valuable asset in the world of amateur radio communication.

**Try ULTRON today and elevate your amateur radio experience!**

## Requirements

Before utilizing ULTRON, please ensure the following prerequisites are met:
- Latest version of **PHP** installed
- List of required **PHP modules** (specified at the end of the script)
- Properly configured radio software for optimal performance
- Recommendations for optimal usage:
  - Disable the Tx watchdog
  - Configure the UDP server to target the program's IP location
  - Enable transmission of logged QSO ADIF data
  - Do not filter UDP data
  - Adjust firewall settings to facilitate data flow

## 📋 Details

- ULTRON operates in **real-time**, allowing seamless software switches without requiring restarts. It automatically detects your **call sign**, **IP address**, and communication ports.
- ULTRON uses its own **logbook**, but you can provide your own by placing it in the "**wsjtx_log.adi**" folder within ULTRON. This logbook remains separate from other software.
- In addition to calling CQ, ULTRON recognizes messages like **73** / **RRR** or **RR73** and determines if correspondents are busy or unresponsive.
- If a correspondent doesn't respond, they will be **waitlisted for 30 minutes** before a QSO retry.
- Signals weaker than **-20dB** are considered less likely to result in successful QSOs.
- The logged ADIF message is sent to ULTRON when the WSJT-X user accepts the "Log  QSO" dialog by clicking the "OK" button.

## Terminal and Color Support

ULTRON requires a terminal with **ASCII color support**. You can use the **Linux terminal** or the new **Windows 10/11 terminal**, both of which support ASCII color. For color support on Windows, consider using [**ConEmu**](https://conemu.github.io/) for an enhanced experience.

## Raspberry Pi

To control Raspberry Pi LEDs, use the `sudo` command configured without a password prompt. The **green LED** lights up for each decoding and turns off when inactive. The **red LED** exhibits a heartbeat-like effect during QSOs. Conducting a QSO emits an audible tone if a speaker is connected to the Pi's jack.

## ULTRON Execution Instructions

To run ULTRON on both Windows and Linux, you have several options:

1. **Terminal Execution:**
   You can execute ULTRON directly through the terminal by running the following command: `php robot.php`

2. **Batch Script (Windows) or Shell Script (Linux):**
Alternatively, you can create a batch script (.BAT) for Windows or a shell script (.sh) for Linux with the necessary commands to execute ULTRON.

3. **Task Scheduler:**
You may also utilize a task scheduler to run ULTRON in the background upon system startup.

Please note the following important considerations:

- ULTRON requires specific modules. Please ensure that you have the required modules installed. Refer to the "robot.php" file for the list of requirements.
- Make necessary modifications to the "php.ini" configuration to meet the requirements of ULTRON.

For reference, an example "php.ini" configuration is provided in the "extras" folder.

For any further assistance, please refer to the documentation or contact our support team.

Thank you for using ULTRON!

## ⚠️ Disclaimer

"I am not liable for the use or inability to use this software or any other."

## Thinking

Ultron was developed by me for me and some friends. It requires the user to have prior knowledge in using PHP and knowing how to use a Windows or Linux terminal. That's no longer up to me, but I guarantee you Ultron works very well. It can operate for years without the need for intervention.

**Why PHP!** Because it runs on any operating system and no compilation is needed. The script is just text with commands. Ultron will execute on any device that can run PHP (PC/CELLPHONE/ROUTER... ETC).

## 🖥️ Devices that Can Run PHP

- Personal Computers (PC) with Windows, macOS, or Linux.
- Smartphones and tablets with iOS, Android, etc.
- Web servers (Linux, Windows Server, etc.).
- Network devices (routers, switches, etc.).
- Internet of Things (IoT) devices with processing capabilities.
- Development boards like Raspberry Pi (Linux).
- Modified gaming consoles.
- Smart TVs and multimedia devices.
- Some printers and multifunctional devices.
- Industrial control systems and embedded devices.
