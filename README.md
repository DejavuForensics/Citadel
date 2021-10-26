# Citadel
Retrieval for Citadel Malware Analysis

## Commercial Antivirus Limitation

Technically, the modus operandi for the identification of malicious files and servers refers to consult in named blacklist databases. The VirusTotal platform issues the diagnoses regarding malignant characteristics related to files and web servers.

When it comes to suspicious files, VirusTotal issues the diagnostics provided by the world's leading commercial antivirus products. Regarding suspicious web servers, VirusTotal uses the database responsible for sensing virtual addresses with malicious practices.

VirusTotal has Application Programming Interface (APIs) that allow programmers to query the platform in an automated way and without the use of the graphical web interface. The proposed paper employs two of the APIs made available by VirusTotal. The first one is responsible for sending the investigated files to the platform server. The second API, in turn, makes commercial antivirus diagnostics available for files submitted to the platform by the first API.

Initially, the executable malwares are sent to the server belonging to the VirusTotal platform. After that, the executables are analyzed by the 86XX commercial antiviruses linked to VirusTotal. Therefore, the antivirus provides its diagnostics for the executables submitted to the platform. VirusTotal allows the possibility of issuing three different types of diagnostics: malware, benign and omission.

Then, through the VirusTotal platform, the proposed paper investigates 86XX commercial antiviruses with their respective results presented in Table 1. We used 3136 malicious executables for 32-bit architecture obtained from the REWEMA database [10]. The goal of the work is to check the number of virtual pests cataloged by antivirus. The motivation is that the acquisition of new virtual plagues plays an important role in combating malicious applications. Therefore, the larger the database of malwares blacklisted, the better it tends to be the defense provided by the antivirus.

As for the first possibility of VirusTotal, the antivirus detects the malignity of the suspicious file. In the proposed experimental environment, all submitted executables are public domain malwares. Therefore, in the proposed study, the antivirus hits when it detects the malignity of the investigated executable. Malware detection indicates that the antivirus provides a robust service against cyber-intrusions. As larger the blacklist database, better tends to be the defense provided by the antivirus.

In the second possibility, the antivirus attests to the benignity of the investigated file. Therefore, in the proposed study, when the antivirus attests the benignity of the file, it is a case of a false negative – since all the samples are malicious. That is, the investigated executable is a malware; however, the antivirus attests to benignity in the wrong way.

In the third possibility, the antivirus does not emit opinion about the suspect executable. The omission indicates that the file investigated has never been evaluated by the antivirus neither it has the robustness to evaluate it in real time. The omission of the diagnosis by the antivirus points to its limitation on large-scale services.

In the third possibility, the antivirus does not emit opinion about the suspect executable. The omission indicates that the file investigated has never been evaluated by the antivirus neither it has the robustness to evaluate it in real time. The omission of the diagnosis by the antivirus points to its limitation on large-scale services.

Table 2 shows the results of the evaluated 86 antivirus products. Five of these antiviruses scored above 98%. These antiviruses were: McAfee-GW-Edition, McAfee, Kaspersky, NANO-Antivirus and Panda. Malware detection indicates that these antivirus programs provide a robust service against cyber-intrusions.

A major adversity in combating malicious applications is the fact that antivirus makers do not share their malware blacklists due to commercial disputes. Through Table 2 analyse, the proposed paper points to an aggravating factor of this adversity: the same antivirus vendor does not even share its databases between its different antivirus programs. Note, for example, that McAfee-GW-Edition and McAfee antiviruses belong to the same company. Their blacklists, though robust, are not shared with each other. Therefore, the commercial strategies of the same company hinder the confrontation with malware. It complements that antivirus vendors are not necessarily concerned with avoiding cyber-invasions, but with optimizing their business income.

Malware detection ranged from 0% to 99.11%, depending on the antivirus being investigated. On average, the 86 antiviruses were able to detect 54.84% of the evaluated virtual pests, with a standard deviation of 39,67. The high standard deviation indicates that the detection of malicious executables may suffer abrupt variations depending on the antivirus chosen. It is determined that the protection, against cybernetic invasions, is due to the choice of a robust antivirus with a large and updated blacklist.

As for the false negatives, the Zoner, Malwarebytes and SUPERAntiSpyware antiviruses, wrongly stated that malware was benign in more than 90% of cases. On average, antiviruses attested false negatives in 14.34% of the cases, with a standard deviation of 21.67. Tackling the benignity of malware can lead to irrecoverable damage. A person or institution, for example, would rely on a particular malicious application when, in fact, it is malware.

VirusBuster, NOD32, eSafe, eTrust-Vet, Authentium, Prevx, Sunbelt, PCTools, a-squared, WhiteArmor, Command, SAVMail, FileAdvisor,Ewido and Webwasher-Gateway antivirus companies have not omitted opinion on any of the 3136 samples malicious. Therefore, about 17% of antivirus softwares were not able to diagnose any of the malicious samples. On average, the antiviruses were missing in 30.82% of the cases, with a standard deviation of 40.97. The omission of the diagnosis points to the limitation of these antiviruses that have limited blacklists for detection of malware in real time.

It is included as adversity, in the combat to malicious applications, the fact of the commercial antiviruses do not possess a pattern in the classification of the malwares as seen in Table 3. We choose 3 of 3136 REWEMA malwares samples in order to exemplify the miscellaneous classifications of commercial antiviruses. The chosen malware are Backdoor.IRC.Darkirc.exe, Backdoor.Win32.Zomby.exe e Constructor.VBS.Alamar.20.exe. In this way, the time when manufacturers react to a new virtual plague is affected dramatically. As there is no a pattern, antiviruses give the names that they want, for example, a company can identify a malware as "Malware.1" and a second company identify it as "Malware12310". Therefore, the lack of a pattern, besides the no-sharing of information among the antivirus manufacturers, hinders the fast and effective detection of a malicious application.


###### Table 2 Results of 68 commercial antiviruses:

Antivirus | Deteccion (%) | False Negative (%) | Omission (%)
--------- | ------------- | ------------------ | -------------
Alibaba 99,9 0,1 0
Ad-Aware 99,75 0,25 0
Webroot 99,75 0,05 0,2
Panda 99,7 0,3 0
Comodo 99,7 0,05 0,25
MicroWorld-eScan 99,5 0,5 0
NANO-Antivirus 99,45 0,5 0,05
BitDefender 99,4 0,45 0,15
Kaspersky 99,2 0,45 0,35
MAX 99,15 0,5 0,35
AVG 99,15 0,05 0,8
ESET-NOD32 99,15 0,85 0
Emsisoft 99,1 0,6 0,3
McAfee 98,9 0,85 0,25
Fortinet 98,9 1,1 0
Avira 98,85 0,35 0,8
DrWeb 98,85 1,05 0,1
TrendMicro-HouseCall 98,75 0,95 0,3
GData 98,7 0,45 0,85
VBA32 98,1 1,8 0,1
TrendMicro 97,75 1,8 0,45
Sophos 97,65 2,05 0,3
SentinelOne 97,55 2,45 0
Cylance 97,45 0,45 2,1
Rising 97,15 2,15 0,7
Zillya 96,9 2,8 0,3
Ikarus 96,8 0,15 3,05
FireEye 96,75 0,3 2,95
Qihoo-360 96,6 3,2 0,2
Jiangmin 96,6 1,65 1,75
Avast 96,45 2,5 1,05
VIPRE 96,4 2,15 1,45
Microsoft 96,05 3,1 0,85
CrowdStrike 95,2 4,6 0,2
McAfee-GW-Edition 94,6 1,85 3,55
Cybereason 93,5 1,1 5,4
ALYac 92,6 3,75 3,65
APEX 92,6 7,35 0,05
Yandex 91,6 7,95 0,45
Symantec 91,25 3,15 5,6
K7GW 90,15 9,85 0
K7AntiVirus 89,75 10,25 0
Arcabit 89,7 10,3 0
BitDefenderTheta 89,45 1,55 9
AhnLab-V3 88,7 11,2 0,1
Cyren 84,1 15,8 0,1
ZoneAlarm 82,2 17,55 0,25
Acronis 75,15 24,8 0,05
F-Secure 73,55 26,15 0,3
CAT-QuickHeal 69,2 27,3 3,5
ClamAV 63,15 35,9 0,95
Endgame 58,75 0,9 40,35
Invincea 58,1 2,8 39,1
Paloalto 56,8 43,15 0,05
ViRobot 51,85 48,1 0,05
SUPERAntiSpyware 50,75 49,25 0
F-Prot 49,55 10 40,45
Tencent 47,35 51,45 1,2
Trapmine 46,7 6,3 47
MaxSecure 46,6 19 34,4
Malwarebytes 46,4 53,05 0,55
Bkav 45,4 48 6,6
Sangfor 44,75 0,6 54,65
Lionic 44,4 11,1 44,5
TotalDefense 43,6 48,95 7,45
Cynet 42,45 0,15 57,4
eGambit 38,55 13,7 47,75
Elastic 38,3 1,5 60,2
TACHYON 37,5 62,5 0
Antiy-AVL 33 22,8 44,2
CMC 27,8 72,15 0,05
Kingsoft 17,85 81,1 1,05
Baidu 12,7 86,85 0,45
Gridinsoft 11,2 28,05 60,75
Zoner 2,3 96,9 0,8
Kaspersky21 0,1 0 99,9
CyrenCloud 0,05 0 99,95
Avast-Mobile 0 59,65 40,35
Babable 0 0,2 99,8
Trustlook 0 0,1 99,9

###### Table 3 Miscellaneous classifications of commercial antiviruses:

Antivírus | VirusShare_001627d61a1bde3478ca4965e738dc1e | VirusShare_075efef8c9ca2f675be296d5f56406fa | VirusShare_0dab86f850fd3dafc98d0f2b401377d5
--------- | ------------------------------------------- | ------------------------------------------- | --------------------------------------------



## Materials and Methods

This paper proposes a database aiming at the classification of 32-bit benign and malware executables. The database is referred to as REWEMA (Retrieval of 32-bit Windows Architecture Executables Applied to Malware Analysis). There are 3136 malicious executables, and 3136 other benign executables. Therefore, the REWEMA base is suitable for learning with artificial intelligence, since both classes of executables have the same amount.

As for malicious executables, REWEMA is the junction of several malware databases. Virtual plagues were extracted from databases provided by enthusiastic study groups such as Vxheaven and TheZoo. As for benign executables, the acquisition came from benign applications repositories such as sourceforge, github and sysinternals. It should be noted that all benign executables were submitted to VirusTotal and all were its benign attested by the main commercial antivirus worldwide. The diagnostics, provided by VirusTotal, corresponding to the benign and malware executables are available in the virtual address of the REWEMA database.

The purpose of the creation of the REWEMA database is to give full possibility of the proposed methodology being replicated by third parties in future works. Therefore, the proposed article, by making its database freely available, enables transparency and impartiality to research, as well as demonstrating the veracity of the results achieved. Therefore, it is hoped that the methodology, to be reported in chapter 6, will serve as a basis for the creation of new scientific works.
