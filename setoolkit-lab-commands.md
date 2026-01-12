STEP 1
Launching SEToolkit

**command**
sudo setoolkit

Explanation

SEToolkit requires root privileges to access network interfaces and system resources. The sudo command ensures the tool runs with the necessary permissions.

Result

SEToolkit launched successfully

Legal disclaimer was displayed

SET main menu appeared in the terminal

STEP 2
Selecting Social-Engineering Attacks

Explanation
At this stage, the Social-Engineering Attacks option was selected from the SEToolkit main menu. This option is used to simulate attacks that exploit human behavior rather than technical vulnerabilities. Since website cloning and credential harvesting rely on deceiving users into submitting sensitive information, this option is the correct path for the lab.

Result / Observation
After selecting Social-Engineering Attacks, SEToolkit displayed a new submenu containing various social engineering attack techniques. This confirmed that the tool had moved from the main menu into the social engineering attack section, allowing further configuration of the website cloning attack.

STEP 3
Selecting Website Attack Vectors

Explanation
After selecting the Website Attack Vectors option from the Social-Engineering Attacks menu, SEToolkit presented another menu containing different web-based attack methods. Each option in this section included a brief description explaining its purpose and how it works. These explanations were helpful in guiding the selection of the most appropriate attack method based on the objective of the lab.

The Website Attack Vectors section is specifically designed for attacks that involve hosting malicious or cloned web pages, making it the correct choice for simulating website cloning and credential harvesting.

Result / Observation
Once the Website Attack Vectors option was selected, SEToolkit displayed a new menu with multiple website-based attack options, each accompanied by a short explanation. This made it easier to understand the available attack paths and confirmed that the lab was progressing toward the website cloning and credential harvesting objective.

STEP 4
Selecting the Credential Harvester Attack Method

Explanation
The Credential Harvester Attack Method was selected because it is designed to capture information entered by a user on a fake or cloned website, such as usernames and passwords.

Result / Observation
After selecting this option, SEToolkit prepared the environment for credential harvesting and prompted for additional configuration related to the website cloning process.

STEP 5
Selecting the Site Cloner

Explanation
The Site Cloner option was selected to replicate the login page of a target website. At this stage, SEToolkit requested the IP address to be used for hosting [10.6.6.1]. The URL for the target site [http://dvwa.vm], which was used as the test environment for this lab.

Result / Observation
After entering the [IP address and the URL], SEToolkit proceeded to clone the target website and prepared it for hosting locally. This confirmed that the site cloning process was successfully initiated using the specified target.

STEP 6
Providing the Attacker IP Address and Target URL

Explanation
After selecting the Site Cloner option, SEToolkit requested the IP address to be used for hosting the cloned website. The IP address provided was 10.6.6.1, which represents the attacker’s (local machine) IP address in the lab environment. This IP address is where the fake website will be hosted and where captured credentials will be sent.

SEToolkit then prompted for the URL of the website to be cloned. The target URL provided was http://dvwa.vm
, which is an intentionally vulnerable web application used for security testing.

Result / Observation
Once the IP address and target URL were entered, SEToolkit began cloning the DVWA website and configuring the local web server. This allowed the cloned login page to be hosted locally and prepared the environment to capture any credentials submitted through the fake site.

STEP 7
Accessing the Cloned Website and Simulating Credential Harvesting

Explanation
At this stage, the cloned website was accessed to verify that the cloning process was successful. The cloned page replicated the appearance of the original [DVWA] login page. In addition, a simple HTML page was created created during the setup, containing a simulated phishing message with a link directing the user to the cloned website.

Since this is a controlled lab environment with no real target, it was assumed that a target user clicked the phishing link and accessed the cloned site. This simulation allowed observation of how a user could be tricked into entering login credentials on a fake website.

Result / Observation
When the cloned website was accessed and login details were submitted, SEToolkit successfully captured the entered credentials and displayed them in the terminal. This confirmed that the site cloning and credential harvesting functionality was working as intended.

This step demonstrated how attackers combine phishing techniques with cloned websites to harvest sensitive user information, even when no software vulnerability is exploited.

STEP 8
Lab Summary and Key Takeaways

Explanation
This final step summarizes the outcome of the SEToolkit website cloning lab. The lab demonstrated how social engineering attacks rely on deception rather than technical exploits. By cloning a legitimate website and hosting it locally, it was possible to simulate how attackers harvest credentials when users unknowingly submit sensitive information on fake login pages.

The lab highlighted the effectiveness of phishing attacks and showed that even technically secure systems can be compromised if users are not security-aware.

Result / Observation

SEToolkit successfully cloned the target website (DVWA)

Login credentials submitted on the fake site were captured

The attack required minimal commands but relied heavily on user interaction

This confirmed that social engineering remains a major cybersecurity threat

Key Takeaway
Human behavior is often the weakest link in security. Awareness, verification, and cautious online behavior are essential defenses against phishing and social engineering attacks.




