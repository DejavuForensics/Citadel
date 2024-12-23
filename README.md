# Citadel
Retrieval for Citadel Malware Analysis

```
Carlos Henrique Macedo dos Santos, Sidney Marlon Lopes de Lima.
Artificial Intelligence-Driven Antivirus in Pattern Identification of Citadel Malware.
Journal of Computational Science, 82 (2024): 102389.
```

## How to use our dataset in Python with ELM (Extreme Learning Machine)

python [melm.py](https://github.com/DejavuForensics/mELM/melm.py) -tall [Antivirus_Dataset_PE32_Citadel_mELM_format.csv](https://github.com/DejavuForensics/Citadel/blob/main/Antivirus_Dataset_PE32_Citadel_mELM_format.csv) 
-kfold 10 -virusNorm -ty 1 -nh 500 -af dilation -v

## Commercial Antivirus Limitation

Technically, the modus operandi for the identification of malicious files and servers refers to consult in named blacklist databases. The VirusTotal platform issues the diagnoses regarding malignant characteristics related to files and web servers.

When it comes to suspicious files, VirusTotal issues the diagnostics provided by the world's leading commercial antivirus products. Regarding suspicious web servers, VirusTotal uses the database responsible for sensing virtual addresses with malicious practices.

VirusTotal has Application Programming Interface (APIs) that allow programmers to query the platform in an automated way and without the use of the graphical web interface. The proposed paper employs two of the APIs made available by VirusTotal. The first one is responsible for sending the investigated files to the platform server. The second API, in turn, makes commercial antivirus diagnostics available for files submitted to the platform by the first API.

Initially, the executable malwares are sent to the server belonging to the VirusTotal platform. After that, the executables are analyzed by the 80 commercial antiviruses linked to VirusTotal. Therefore, the antivirus provides its diagnostics for the executables submitted to the platform. VirusTotal allows the possibility of issuing three different types of diagnostics: malware, benign and omission.

Then, through the VirusTotal platform, the proposed paper investigates 80 commercial antiviruses with their respective results presented in Table 1. We used 2,000 malicious executables for 32-bit architecture. The goal of the work is to check the number of virtual pests cataloged by antivirus. The motivation is that the acquisition of new virtual plagues plays an important role in combating malicious applications. Therefore, the larger the database of malwares blacklisted, the better it tends to be the defense provided by the antivirus.

As for the first possibility of VirusTotal, the antivirus detects the malignity of the suspicious file. In the proposed experimental environment, all submitted executables are public domain malwares. Therefore, in the proposed study, the antivirus hits when it detects the malignity of the investigated executable. Malware detection indicates that the antivirus provides a robust service against cyber-intrusions. As larger the blacklist database, better tends to be the defense provided by the antivirus.

In the second possibility, the antivirus attests to the benignity of the investigated file. Therefore, in the proposed study, when the antivirus attests the benignity of the file, it is a case of a false negative – since all the samples are malicious. That is, the investigated executable is a malware; however, the antivirus attests to benignity in the wrong way.

In the third possibility, the antivirus does not emit opinion about the suspect executable. The omission indicates that the file investigated has never been evaluated by the antivirus neither it has the robustness to evaluate it in real time. The omission of the diagnosis by the antivirus points to its limitation on large-scale services.

Table 1 shows the results of the evaluated 80 antivirus products. Malware detection indicates that these antivirus programs provide a robust service against cyber-intrusions.

A major adversity in combating malicious applications is the fact that antivirus makers do not share their malware blacklists due to commercial disputes. Through Table 1 analyse, the proposed work points to an aggravating factor of this adversity: the same antivirus vendor does not even share its databases between its different antivirus programs. Note, for example, that McAfee and McAfee-GW-Edition antiviruses belong to the same company. Their blacklists, though robust, are not shared with each other. Therefore, the commercial strategies of the same company hinder the confrontation with malware. It complements that antivirus vendors are not necessarily concerned with avoiding cyber-invasions, but with optimizing their business income.

Malware detection ranged from 0% to 99.9%, depending on the antivirus being investigated. On average, the 80 antiviruses were able to detect 71.79% of the evaluated virtual pests, with a standard deviation of 28.51%. The high standard deviation indicates that the detection of malicious executables may suffer abrupt variations depending on the antivirus chosen. It is determined that the protection, against cybernetic invasions, is due to the choice of a robust antivirus with a large and updated blacklist.

As for the false negatives, the Zoner antivirus wrongly stated that malware was benign in more than 90% of cases. On average, antiviruses attested false negatives in 14.68% of the cases, with a standard deviation of 17.39%. Tackling the benignity of malware can lead to irrecoverable damage. A person or institution, for example, would rely on a particular malicious application when, in fact, it is malware.

On average, the antiviruses were missing in 13.91% of the cases, with a standard deviation of 19.75%. The omission of the diagnosis points to the limitation of these antiviruses that have limited blacklists for detection of malware in real time.

It is included as adversity, in the combat to malicious applications, the fact of the commercial antiviruses do not possess a pattern in the classification of the malwares as seen in Table 2. We choose 3 of 2,000 malwares samples in order to exemplify the miscellaneous classifications of commercial antiviruses. In this way, the time when manufacturers react to a new virtual plague is affected dramatically. As there is no a pattern, antiviruses give the names that they want, for example, a company can identify a malware as "Malware.1" and a second company identify it as "Malware12310". Therefore, the lack of a pattern, besides the no-sharing of information among the antivirus manufacturers, hinders the fast and effective detection of a malicious application.


###### Table 2 Results of 80 commercial antiviruses:

Antivirus | Deteccion (%) | False Negative (%) | Omission (%)
--------- | ------------- | ------------------ | -------------
Alibaba	 | 	99.9	 | 	0.1	 | 	0
Ad-Aware	 | 	99.75	 | 	0.25	 | 	0
Webroot	 | 	99.75	 | 	0.05	 | 	0.2
Panda	 | 	99.7	 | 	0.3	 | 	0
Comodo	 | 	99.7	 | 	0.05	 | 	0.25
MicroWorld-eScan	 | 	99.5	 | 	0.5	 | 	0
NANO-Antivirus	 | 	99.45	 | 	0.5	 | 	0.05
BitDefender	 | 	99.4	 | 	0.45	 | 	0.15
Kaspersky	 | 	99.2	 | 	0.45	 | 	0.35
MAX	 | 	99.15	 | 	0.5	 | 	0.35
AVG	 | 	99.15	 | 	0.05	 | 	0.8
ESET-NOD32	 | 	99.15	 | 	0.85	 | 	0
Emsisoft	 | 	99.1	 | 	0.6	 | 	0.3
McAfee	 | 	98.9	 | 	0.85	 | 	0.25
Fortinet	 | 	98.9	 | 	1.1	 | 	0
Avira	 | 	98.85	 | 	0.35	 | 	0.8
DrWeb	 | 	98.85	 | 	1.05	 | 	0.1
TrendMicro-HouseCall	 | 	98.75	 | 	0.95	 | 	0.3
GData	 | 	98.7	 | 	0.45	 | 	0.85
VBA32	 | 	98.1	 | 	1.8	 | 	0.1
TrendMicro	 | 	97.75	 | 	1.8	 | 	0.45
Sophos	 | 	97.65	 | 	2.05	 | 	0.3
SentinelOne	 | 	97.55	 | 	2.45	 | 	0
Cylance	 | 	97.45	 | 	0.45	 | 	2.1
Rising	 | 	97.15	 | 	2.15	 | 	0.7
Zillya	 | 	96.9	 | 	2.8	 | 	0.3
Ikarus	 | 	96.8	 | 	0.15	 | 	3.05
FireEye	 | 	96.75	 | 	0.3	 | 	2.95
Qihoo-360	 | 	96.6	 | 	3.2	 | 	0.2
Jiangmin	 | 	96.6	 | 	1.65	 | 	1.75
Avast	 | 	96.45	 | 	2.5	 | 	1.05
VIPRE	 | 	96.4	 | 	2.15	 | 	1.45
Microsoft	 | 	96.05	 | 	3.1	 | 	0.85
CrowdStrike	 | 	95.2	 | 	4.6	 | 	0.2
McAfee-GW-Edition	 | 	94.6	 | 	1.85	 | 	3.55
Cybereason	 | 	93.5	 | 	1.1	 | 	5.4
ALYac	 | 	92.6	 | 	3.75	 | 	3.65
APEX	 | 	92.6	 | 	7.35	 | 	0.05
Yandex	 | 	91.6	 | 	7.95	 | 	0.45
Symantec	 | 	91.25	 | 	3.15	 | 	5.6
K7GW	 | 	90.15	 | 	9.85	 | 	0
K7AntiVirus	 | 	89.75	 | 	10.25	 | 	0
Arcabit	 | 	89.7	 | 	10.3	 | 	0
BitDefenderTheta	 | 	89.45	 | 	1.55	 | 	9
AhnLab-V3	 | 	88.7	 | 	11.2	 | 	0.1
Cyren	 | 	84.1	 | 	15.8	 | 	0.1
ZoneAlarm	 | 	82.2	 | 	17.55	 | 	0.25
Acronis	 | 	75.15	 | 	24.8	 | 	0.05
F-Secure	 | 	73.55	 | 	26.15	 | 	0.3
CAT-QuickHeal	 | 	69.2	 | 	27.3	 | 	3.5
ClamAV	 | 	63.15	 | 	35.9	 | 	0.95
Endgame	 | 	58.75	 | 	0.9	 | 	40.35
Invincea	 | 	58.1	 | 	2.8	 | 	39.1
Paloalto	 | 	56.8	 | 	43.15	 | 	0.05
ViRobot	 | 	51.85	 | 	48.1	 | 	0.05
SUPERAntiSpyware	 | 	50.75	 | 	49.25	 | 	0
F-Prot	 | 	49.55	 | 	10	 | 	40.45
Tencent	 | 	47.35	 | 	51.45	 | 	1.2
Trapmine	 | 	46.7	 | 	6.3	 | 	47
MaxSecure	 | 	46.6	 | 	19	 | 	34.4
Malwarebytes	 | 	46.4	 | 	53.05	 | 	0.55
Bkav	 | 	45.4	 | 	48	 | 	6.6
Sangfor	 | 	44.75	 | 	0.6	 | 	54.65
Lionic	 | 	44.4	 | 	11.1	 | 	44.5
TotalDefense	 | 	43.6	 | 	48.95	 | 	7.45
Cynet	 | 	42.45	 | 	0.15	 | 	57.4
eGambit	 | 	38.55	 | 	13.7	 | 	47.75
Elastic	 | 	38.3	 | 	1.5	 | 	60.2
TACHYON	 | 	37.5	 | 	62.5	 | 	0
Antiy-AVL	 | 	33	 | 	22.8	 | 	44.2
CMC	 | 	27.8	 | 	72.15	 | 	0.05
Kingsoft	 | 	17.85	 | 	81.1	 | 	1.05
Baidu	 | 	12.7	 | 	86.85	 | 	0.45
Gridinsoft	 | 	11.2	 | 	28.05	 | 	60.75
Zoner	 | 	2.3	 | 	96.9	 | 	0.8
Kaspersky21	 | 	0.1	 | 	0	 | 	99.9
CyrenCloud	 | 	0.05	 | 	0	 | 	99.95
Avast-Mobile	 | 	0	 | 	59.65	 | 	40.35
Babable	 | 	0	 | 	0.2	 | 	99.8
Trustlook	 | 	0	 | 	0.1	 | 	99.9

###### Table 3 Miscellaneous classifications of commercial antiviruses:

Antivirus | VirusShare_00011bf7484b730cf304265d57db8d77 | VirusShare_000c15cfd50adc583f86031deb0d33e4 | VirusShare_000c4f7bd4b256fad1c16d4b3acf8c8a
--------- | ------------------------------------------- | ------------------------------------------- | -------------------------------------------
Acronis | suspicious | suspicious | suspicious
Ad-Aware | Generic.StealerA.A1981AC9 | Trojan.Dropper.Zbot.O | Gen:Trojan.ProcessHijack.jyX@am!lRad
AhnLab-V3 | Trojan/Win32.Tepfer.R93111 | Spyware/Win32.Zbot.R23206 | Downloader/Win32.Avalod.R20872
Alibaba | TrojanPSW:Win32/Tepfer.feba1b1c | TrojanSpy:Win32/FAKEAV.c84419ca | VirTool:Win32/CeeInject.cebf4812
ALYac | Generic.StealerA.A1981AC9 | Trojan.Dropper.Zbot.O | Gen:Trojan.ProcessHijack.jyX@am!lRad
Antiy-AVL | Trojan[PSW]/Win32.Tepfer.fuph | false negative | false negative
APEX | Malicious | Malicious | Malicious
Arcabit | Generic.StealerA.A1981AC9 | Trojan.Dropper.Zbot.O | false negative
Avast | Sf:Crypt-AS [Trj] | Win32:Karagany | Win32:Kryptik-IDX [Trj]
Avast-Mobile | false negative | antivirus scan not found | antivirus scan not found
AVG | Sf:Crypt-AS [Trj] | Win32:Karagany | Win32:Kryptik-IDX [Trj]
Avira | TR/Kryptik.avp.8 | TR/Inject.11 | TR/Buzus.44589745
Baidu | Win32.Trojan-PSW.Fareit.a | false negative | false negative
BitDefender | Generic.StealerA.A1981AC9 | Trojan.Dropper.Zbot.O | Gen:Trojan.ProcessHijack.jyX@am!lRad
BitDefenderTheta | Gen:NN.ZexaF.34122.fmW@aOkYQG | Gen:NN.ZexaF.34628.sO1@aWSVnOni | AI:Packer.D062BC161E
Bkav | false negative | W32.AIDetect.malware1 | W32.AIDetect.malware1
CAT-QuickHeal | Trojanpws.Tepfer.20303 | TrojanPWS.Zbot.Y | false negative
ClamAV | Win.Trojan.Fareit-403 | Win.Trojan.Zbot-20285 | Win.Trojan.Avalod-202
CMC | Trojan-PSW.Win32.Tepfer!O | false negative | false negative
Comodo | TrojWare.Win32.PWS.Fareit.GS@5t8zib | TrojWare.Win32.Kazy.FOF@4pekmj | Malware@#2qfqryp9eidtz
CrowdStrike | win/malicious_confidence_100% (W) | win/malicious_confidence_100% (D) | win/malicious_confidence_100% (W)
Cybereason | malicious.7484b7 | antivirus scan not found | malicious.bd4b25
Cylance | Unsafe | Unsafe | Unsafe
Cynet | antivirus scan not found | Malicious (score: 100) | Malicious (score: 100)
Cyren | W32/Bloop.A.gen!Eldorado | W32/Zbot.DQ.gen!Eldorado | W32/CeeInject.AK.gen!Eldorado
DrWeb | Trojan.PWS.Stealer.1932 | Trojan.PWS.Panda.1698 | Trojan.DownLoad3.530
eGambit | Unsafe.AI_Score_100% | false negative | false negative
Elastic | antivirus scan not found | malicious (high confidence) | malicious (high confidence)
Emsisoft | Generic.StealerA.A1981AC9 (B) | Trojan.Dropper.Zbot.O (B) | Gen:Trojan.ProcessHijack.jyX@am!lRad (B)
Endgame | malicious (high confidence) | antivirus scan not found | antivirus scan not found
ESET-NOD32 | a variant of Win32/PSW.Fareit.D | Win32/Spy.Zbot.AAN | a variant of Win32/Injector.PBO
F-Prot | W32/Bloop.A.gen!Eldorado | antivirus scan not found | antivirus scan not found
F-Secure | Trojan.TR/Kryptik.avp.8 | false negative | false negative
FireEye | Generic.mg.00011bf7484b730c | Generic.mg.000c15cfd50adc58 | Generic.mg.000c4f7bd4b256fa
Fortinet | W32/Agent.NTM!tr | W32/ZBOT.HL!tr | W32/Injector.OEC!tr
GData | Win32.Trojan-Stealer.Zbot.AB | Trojan.Dropper.Zbot.O | Gen:Trojan.ProcessHijack.jyX@am!lRad
Gridinsoft | antivirus scan not found | Malware.Win32.Gen.bot!n | Trojan.Win32.Downloader.sa
Ikarus | Trojan-Spy.Fareit | Trojan-Spy.Win32.Zbot | Trojan-Downloader.Win32.Avalod
Invincea | heuristic | antivirus scan not found | antivirus scan not found
Jiangmin | Trojan/PSW.Tepfer.asun | TrojanSpy.Zbot.bory | TrojanDownloader.Avalod.kys
K7AntiVirus | Password-Stealer ( 0040f4f51 ) | Trojan ( 0040f02a1 ) | false negative
K7GW | Password-Stealer ( 0040f4f51 ) | Trojan ( 0040f02a1 ) | false negative
Kaspersky | Trojan-PSW.Win32.Tepfer.fuph | Trojan-Spy.Win32.Zbot.dmna | HEUR:Trojan.Win32.Generic
Kingsoft | false negative | Win32.Heur.KVM011.a.(kcloud) | Win32.TrojDownloader.Avalod.(kcloud)
Lionic | false negative | Hacktool.Win32.Krap.lKMc | Trojan.Win32.Generic.4!c
Malwarebytes | Spyware.Pony | Trojan.Zbot.Gen | false negative
MAX | malware (ai score=100) | malware (ai score=100) | malware (ai score=100)
MaxSecure | Trojan.Malware.5237142.susgen | Trojan.Packed.Krap.iu | Trojan.Malware.3919469.susgen
McAfee | PWS-Zbot.gen.ate | PWS-Zbot.gen.re | PWS-Zbot.gen.rz
McAfee-GW-Edition | BehavesLike.Win32.PWSZbot.nh | BehavesLike.Win32.ZBot.dc | BehavesLike.Win32.ZBot.cc
Microsoft | PWS:Win32/Fareit | PWS:Win32/Zbot.gen!AF | VirTool:Win32/CeeInject.CY
MicroWorld-eScan | Generic.StealerA.A1981AC9 | Trojan.Dropper.Zbot.O | Gen:Trojan.ProcessHijack.jyX@am!lRad
NANO-Antivirus | Trojan.Win32.Siggen.evgeyh | Trojan.Win32.Panda.kwuka | Trojan.Win32.Avalod.tmlkw
Paloalto | generic.ml | false negative | false negative
Panda | Trj/Genetic.gen | Bck/Qbot.AO | Trj/Genetic.gen
Qihoo-360 | Win32/Trojan.512 | Win32/Trojan.Zbot.HxQBEpsA | Win32/Trojan.Buzus.HwEBvHsA
Rising | Stealer.Fareit!1.B777 (CLOUD) | Spyware.Zbot!8.16B (CLOUD) | Trojan.Injector!8.C4 (CLOUD)
Sangfor | Malware | Trojan.Win32.Save.a | Trojan.Win32.Save.a
SentinelOne | DFI - Malicious PE | Static AI - Malicious PE | Static AI - Malicious PE
Sophos | Mal/Pony-A | ML/PE-A + Troj/Zbot-DHN | ML/PE-A + Mal/EncPk-AEE
SUPERAntiSpyware | false negative | Trojan.Agent/Gen-Nultsk | Trojan.Agent/Gen-Injector
Symantec | Infostealer!im | antivirus scan not found | antivirus scan not found
TACHYON | Trojan-PWS/W32.Tepfer.93184.U | Trojan-Spy/W32.ZBot.297472.O | false negative
Tencent | Malware.Win32.Gencirc.114beb02 | Malware.Win32.Gencirc.10b428b9 | Malware.Win32.Gencirc.114bcb54
TotalDefense | antivirus scan not found | Win32/Zbot.FKD | false negative
Trapmine | malicious.moderate.ml.score | antivirus scan not found | antivirus scan not found
TrendMicro | BKDR_PONY.SM | TROJ_FAKEAV.SMFW | TROJ_INJECTO.BXZ
TrendMicro-HouseCall | BKDR_PONY.SM | TROJ_FAKEAV.SMFW | TROJ_INJECTO.BXZ
VBA32 | SScope.Malware-Cryptor.Ponik | BScope.Malware-Cryptor.SB.01798 | Malware-Cryptor.Inject.gen
VIPRE | Trojan.Win32.Fareit.gi (v) | Trojan-Spy.Win32.Zbot.dmna (v) | Trojan.Win32.Generic!BT
ViRobot | false negative | Trojan.Win32.A.Zbot.297472.A | Trojan.Win32.A.Downloader.13504.A
Webroot | W32.Fareit | W32.Rogue.Gen | W32.Rogue.Gen
Yandex | Trojan.PWS.Tepfer!38TJ04+WEuY | TrojanSpy.Zbot!iI828LHQoJ4 | Trojan.GenAsa!bOLEW3pnOuY
Zillya | Trojan.Tepfer.Win32.46435 | Trojan.Zbot.Win32.54180 | Downloader.Avalod.Win32.10878
ZoneAlarm | Trojan-PSW.Win32.Tepfer.fuph | Trojan-Spy.Win32.Zbot.dmna | false negative
Zoner | false negative | false negative | false negative

##### Table legend:
- false negative: The file is infected and the antivirus wasn't able to detect it
- positive: The file is infected, the antivirus managed to detect it but the virus does not have a name
All the other labels were given by the antivirus company.

## Materials and Methods


This paper proposes a database aiming at the classification of 32-bit benign and malware executables. There are 2,000 malicious executables, and 2,000 other benign executables. Therefore, our dataset is suitable for learning with artificial intelligence, since both classes of executables have the same amount.

Virtual plagues were extracted from databases provided by enthusiastic study groups as VirusShare. As for benign executables, the acquisition came from benign applications repositories such as sourceforge, github and sysinternals. It should be noted that all benign executables were submitted to VirusTotal and all were its benign attested by the main commercial antivirus worldwide. The diagnostics, provided by VirusTotal, corresponding to the benign and malware executables are available in the virtual address of our database.

The purpose of the creation of the database is to give full possibility of the proposed methodology being replicated by third parties in future works. Therefore, the proposed article, by making its database freely available, enables transparency and impartiality to research, as well as demonstrating the veracity of the results achieved. Therefore, it is hoped that the methodology will serve as a basis for the creation of new scientific works.

## Executable Feature Extraction

The extraction of features of executables employs the process of disassembling. Then, the algorithm, referring to the executable, can be studied and later classified by the neural networks described in the next section. In total, 430 features of each executable are extracted, referring to the groups mentioned above. The pescanner tool are employed in order to extract the features of executables. Next, the groups of features extracted from the executables investigated are detailed.
######	Histogram of instructions, in assembly, referring to the mnemonic.
######	Number of subroutines invoking TLS (Transport Layer Security).
######	Number of subroutines responsible for exporting data (exports).  
######	APIs (Application Programming Interface) used by the executable.
######	Features related to clues that the computer has suffered fragmentation on its hard disk, as well as accumulated invalid boot attempts.  
######	Application execution mode. There are two options:
-	software with a graphical interface (GUI);
-	software running on the console.
######	Features related to the Operating System. Our digital forensics examines if the tested file tries to:
-	identify the current operating system user name;
-	access APIs in order to create and manage current OS user profiles;
-	detect the number of milliseconds since the system was initialized;
-	execute an operation in a specific file;
-	identify the version of the Windows Operating System in use;
-	monitor internal message traffic among system processes;
-	alter the Windows startup settings and contents (STARTUPINFO);  
-	allow applications to access functionality provided by shell of the operating system, as well as alter it; 
-	change the logon messages at Windows OS startup; 
-	change native applications linked to standard dialog boxes in order to open and save files, choosing color and font, among other customizations;
-	configure Windows Server licensing ; 
-	configure Windows Server 2003;
-	change the system's power settings;
-	open a process, service, or native library of the Operating System; 
-	exclude the context of certificates linked to the Operating System; 
-	copy an existing file to a new file; 
-	create, open, delete, or alter a file;
-	create and execute new process(s); 
-	create new directory(s); 
-	search for specific file(s);  
-	create a service object and add it to the control manager database for a certain service; 
-	encrypt data. It is a typical strategy of ransomwares which sequester the victim's data through cryptography. To decrypt the data, the invader asks the user for a monetary amount so that he victim can have all his data back;
-	access file systems, devices, processes, threads and error handling of the system;
-	change the sound and audio device properties of the system;
-	access graphical content information for monitors, printers, and other Windows OS output devices; 
-	use and/or monitor the USB port;
-	control a driver of a particular device; 
-	investigate if a disk drive is a removable, fixed, CD / DVD-ROM, RAM or network drive;
######	Features related to Windows Registry (Regedit). It is worth noting that the victim may not be free from malware infection even after its detection and elimination. The persistence of malefactions, even after malware exclusion, occurs due to the insertion of malicious entries (keys) in Regedit. Then, when the operating system boots, the cyber-attack restarts because of the malicious key invoking the vulnerability exploited by malware (eg: redirect Internet Explorer home page). Then, our antivirus audits if the suspicious application tries to:
-	detect the NetBIOS name of the local computer. This name is established at system startup, when the system reads it in the registry (Regedit);
-	terminate a key of a specific registry; 
-	create a key from in a specific registry. If the key already exists in Regedit, then it will be read; 
-	delete a key and its values in Regedit; 
-	enumerate and   open subkeys of a specific open registry. 
######	Features related to spywares such as keyloggers (capture of keyboard information in order to theft of passwords and logins) and screenloggers (screen shot of the victim). Our antivirus audits if the analyzed file tries to:
-	detect in which part of the victim's screen there was an update;
-	identify the screen update region by copying it to a particular region;
-	capture AVI movies and videos from web cameras and other video hardware; 
-	capture information on electronic voting, specifically from the company Optical Vote-Trakker;
-	copy an array of keyboard key states. Such strategy is typical of keyloggers
-	monitor user's Internet activity and private information;
-	collect online bank passwords and other confidential information and to send the data to invader creator;
-	access a computer from remote locations, stealing passwords, Internet banking and personal data; 
-	create a BHO (Browser Helper Object) which is executed automatically every time when the web browser is started. It fits to emphasize that BHOs are not impeded by personal firewalls because they are identified as part of the browser. In a distorted way, BHOs are often used by adware and spyware in order to record keyboard and mouse entries
-	locate passwords stored on a computer.
######	Features related to Anti-forensic Digital which are techniques of removal, occultation and subversion of evidences with the goal of reducing the consequences of the results of forensic analyzes. Our antivirus investigates if the file tries to:
-	Suspend its own execution until a certain timeout interval has elapsed. A typical malware strategy that maintains itself inactive until the end of commercial antivirus quarantine;
-	Disable the victim's defense mechanisms, including Firewall and Antivirus;
-	disable automatic Windows updates;
-	detect if the own file is being scanned by an debugger of the Operating System;   
-	retrieve information about the first and next process found in an Operating System snapshot. Such strategy is typical of malwares that aim to corrupt backups and restore points of the Operating System;
-	hide one file in another. This strategy is named, technically, steganography which aims to hide malware in a benign program in the Task Manager;
-	disguise its own name in the Task Manager;
-	make use of libraries associated with Hackers Encyclopedia 2002;
-	Create a ZeroAcess cyber-attack type through firmware updates of hardware devices (eg, hard drive controlled).
######	Features related to the creation of GUI (Graphical User Interface) of the suspicious program. Our antivirus audits if the suspect file tries to: 
-	create a GUI at runtime; 
-	use DirectX which allows multimedia applications to draw 2D graphics; 
-	create a module that contains bitmap compression and decompression routines used for Microsoft Video for Windows;
-	create 3D graphics related to utilitarian functions used by OpenGL; 
-	detect shapes through computer vision and digital image processing;
-	access functionalities in order to create and to manage screen windows and more basic controls such as buttons and scrollbars, receive mouse and keyboard input, and other functionalities associated with the Windows GUI. This includes widgets like status bars, progress bars, toolbars, and guides; 
######	Features related to the illicit forensic of the RAM (main memory) of the local system. Our antivirus investigates if the suspicious application tries to:
-	access information in specific regions of main memory;
-	read data from an area of memory occupied by a specific process;
-	write data to a memory area in a specific process;
-	reserve, confirm or alter the status of a page region in the virtual address space of a process.
######	Features related to network traffic. It is checked if the suspect file tries to:
-	query DNS servers;
-	send request to an HTTP server; 
-	monitor information of the headers of computer data packets associated with an HTTP request;
-	send an ICMP IPv4 echo request; 
-	send an SNMP request used to monitor LAN equipment;
-	terminate the Internet connection;
-	create an FTP or HTTP session at runtime; 
-	fragment a URL at runtime; 
-	query a server in order to determine the amount of traffic data available; 
-	identify the connection state of the local system in relation to the Internet; 
-	initialize the use of an application of the WinINet functions (Windows API for creating and using the application using the Internet); 
-	read data from network packets made from previous local system requests (typical behavior of sniffers); 
-	overwrite data in a local system network packet; 
-	manage local and remote network systems; 
-	create a network socket on the local system. In a conventional application, the server sends data to the client (s). In an opposite way, in malware, the victim sends the data (images, digits) to the server. Therefore, malware can create sockets on the local system waiting (listen) for a remote malicious computer to request a connection and, then, receive the victim's private information;
-	receive data of a socket. Typical strategy of backdoors when the victim starts receiving remote commands; 
-	send data to a socket. Typical strategies of spywares which, after capturing innermost information, they send them to a malicious remote computer; 
######	Features related to utility applications programs. Our created antivirus checks if the suspicious file tries to:
-	reproduce videos/audios through Windows Media Player; 
-	change the shortcut icon and Internet default settings exhibited in the Explorer toolbar address bar; 
-	alter the Wordpad configurations;
-	alter the configurations of sockets, specifically, managed by Internet Explorer; 
-	alter Outlook Express configurations and to access the victim’s  e-mail list; 
-	access information linked to the Microsof Office; 
-	alter the configurations of the Adobe System’s suite;
-	change the system's disk cleanup configurations; 
-	alter the settings of native digital electronic games and others linked to companies Tycoon and Electronic Arts;
-	change Google Inc updates settings; 
-	use Visual Basic. Such strategy is typical of macro viruses that are intended to infect applications that support macro language such as web browsers, Microsoft Office, and Adobe Systems.
-	alter the access settings to Wikipedia.

