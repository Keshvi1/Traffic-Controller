# Traffic-Controller

# Objective 
The main objective of the system is to control traffic congestion problems. In this system, the traffic signal lights are controlled by PLC with reference to the vehicle density on the road. The system developed is able to sense the presence of vehicles within certain range and to set an appropriate duration for the traffic signals to react accordingly. By employing mathematical functions, appropriate time can be calculated for the signals to illuminate, and thus traffic can be controlled.


# Software requirements 
• Windows® 8.1 (32-bit or 64-bit) 
• Windows 2012 
• Windows 7 Professional (32-bit or 64-bit) 
• Windows Vista® with Service Pack, or later 
• RSLogix 500 and RSLogix Micro rely on RSLinx® Classic communication software.


# Installing

# Install RSLinx Classic Lite 

If you have RSLinx Classic installed, you do not need to install RSLinx Classic Lite.
RSLinx Classic Lite provides communication between the controller and the personal computer.
To install RSLinx Classic Lite: 
1. Log onto the computer as an administrator, or as a user with administrative privileges. 
2. Insert the installation CD into the disk drive. The installation program should start automatically. If not, open the installation disk and run AUTORUN.EXE.
 3. Click Required Steps, and then click Install RSLinx Classic Lite.
 4. Follow the screen directions.
Install the FactoryTalk Services Platform 
This section only applies to RSLogix 500. If you installed RSLinx Classic Lite, skip to the next step. FactoryTalk Services Platform gets installed along with RSLinx Classic Lite.



# To install the FactoryTalk Services Platform:

1. Log onto the computer as an administrator or as a user with administrative privileges. 
2. Insert the installation CD into the disk drive. The installation program starts automatically. If it does not, open the installation disk and launch AUTORUN.EXE. 
3. Click Required Steps, and then click Install FactoryTalk Components. 
4. Click Install FactoryTalk Services Platform. 
5. Follow the instructions.

Install FactoryTalk Activation Manager 
The FactoryTalk Activation Manager is used to activate RSLogix 500 and RSLogix Micro.
Before you begin: 
Your computer must be connected to the Internet to obtain activations directly using the FactoryTalk Activation Manager.

# To install FactoryTalk Activation Manager: 
1. Log onto the computer as an administrator or as a user with administrative privileges. 
2. Insert the RSLogix 500 or RSLogix Micro disk into the disk drive. The installation program starts automatically. If it does not, open the installation disk with Windows Explorer and run AUTORUN.EXE.
3. Click Required Steps, and then click Install FactoryTalk Components. 
4. Click Install FactoryTalk Activation Manager. 
5. Follow the instructions to install the FactoryTalk Activation Manager. 
6. After the installation is finished, you restart your computer. 
7. After the restart, use FactoryTalk Activation Manager to obtain your activation. Click Start > All Programs > Rockwell Software > FactoryTalk Activation > FactoryTalk Activation Manager. If you need help with obtaining activations, click Learn More or Help in FactoryTalk Activation Manager.

# Install RSLogix 500 or RSLogix Micro 

# To install RSLogix 500 or RSLogix Micro: 
1. Log onto the computer as an administrator or as a user with administrative privileges. 
2. Insert the installation CD into the disk drive and open the installation disk and launch AUTORUN.EXE. 3. Click Required Steps, and then click Install RSLogix 500 or Install RSLogix Micro. 
4. Follow the instructions that appear on the screen.
5. (RSLogix 500 only) If you installed the FactoryTalk Services Platform, during the installation, you are prompted to enable FactoryTalk Security.
If you do not want to use FactoryTalk Security, clear the Enable FactoryTalk Security check box, and then click Next. If you want to use FactoryTalk Security, select the Enable FactoryTalk Security check box.

# Import a security configuration
If you have used the Rockwell Automation Security Server to control access to user actions in RSLogix 500 and you have enabled FactoryTalk Security, you can import your security configuration from the Security Server into FactoryTalk Security.
To import the security configuration from the Rockwell Automation Security Server into FactoryTalk Security: 
1. Because the import process writes to the FactoryTalk Directory, it is important that you backup your FactoryTalk Directory before beginning the import. 
a. Run the FactoryTalk Administration Console by clicking Start > Programs > Rockwell Software > FactoryTalk Administration Console. 
b. Log onto the FactoryTalk Directory where you are using FactoryTalk Security. 
c. Right-click the top-level object in the Explorer tree (this is the Network or Local object, depending on whether you are viewing the Network or Local directory), and then click Backup. 
d. In the Backup dialog box, type a name for the backup file in the Specify archive name box. In the Specify archive location box, enter the path to where you want to save the backup file. Click the browse (...) button to browse for a folder. 
e. Click OK. 
2. In the Security Server Configuration Explorer, export your security database to a file by clicking File > Export Database. 
3. After exporting the database, close the Configuration Explorer.
4. Click Start > Programs > Rockwell Software > FactoryTalk Tools > Import RSSecurity Configuration. This starts the FactoryTalk Security Import utility. 
5. In the import utility, enter the path to the file you exported from the Security Server in the Select RS Security Server backup database to import box. If you prefer, click Browse and locate the file. 
6. From the Destination Directory list, select the FactoryTalk Directory that you are using with FactoryTalk Security. Select Network or Local. 
7. If you have actions in your Security Server database that do not have security rights granted or denied, you can grant access to those actions to users by default by selecting the Add implicitly grant access box. If you do not select this box, those actions will be denied to users by default. 
8. If you want to display a log file of what happens during the import, select the Display log on completion box. 
9. Click OK. 
10. The import utility warns that you should back up your FactoryTalk Directory. If you have backed up your FactoryTalk Directory, click Yes. 
11. Log onto the FactoryTalk Directory where you will be using FactoryTalk Security. 
12. The import process runs. Depending on the contents of the file you are importing and of your FactoryTalk Directory, you may receive a warning message during the import. If this happens, review the information and click OK to continue the import process. 
13. When the process is complete, the import utility displays a dialog box that indicates whether it was successful or unsuccessful. Click OK. 
14. If you chose to display a log file at the end of the import, the log file opens.



# Launch the application 
You can now launch RSLogix 500 or RSLogix Micro.
To start RSLogix 500, click Start > All Programs > Rockwell Software > RSLogix 500 > RSLogix 500. 
To start RSLogix Micro, click Start > All Programs > Rockwell Software > RSLogix Micro > RSLogix Micro .


# Configure a driver in RSLinx Classic
The RSLinx Classic driver provides the connection between your computer and the processor. You have to tell RSLinx Classic what driver you want to use to make that connection.


# Configure a driver in RSLinx Classic: 
1. Click Start > Programs > Rockwell Software > RSLinx > RSLinx. RSLinx Classic starts in a minimized mode,with an RSLinx icon in the Windows notification area. 
2. In RSLinx Classic, click Communications > Configure Driver, to open the Configure Drivers dialog box. 
3. In the Configure Drivers dialog box, select the driver. (depending on which driver is used eg: Ethernet cable, simulation, RS232driver, etc.)
4. Click Add New. 
5. RSLinx Classic prompts you to name the driver. You can use the default name, or enter a name. Click OK to open the driver's configuration dialog box. 
6. Configure the driver to match your connection to the processor. 
7. The driver appears in the Configured Drivers list of the Configure Drivers dialog box. Click Close. 
8. To verify that the driver is working properly, click Communications > RSWho. This function shows what processors and other communications devices are available through the driver.
9. In the RSWho tree, open the driver you configured and verify that the processor is one of the displayed devices. 
10. If you cannot see the processor, the driver is not configured correctly or there is a communication problem. Correct the problem before proceeding. 

# Configure system communications
To set the system communications parameters: 
1. From the Comms menu, click System Comms, to open the Communications dialog box. If RSLinx Classic is not running, it starts. 
2. Open the driver you configured. The processor you want to program should be visible. Click the processor, and then click OK.
Create a new project or open an existing project 
Create a new project 
To create a new project, click File > New. Enter the type of processor you communicate with and the system creates a project tree. The project tree provides access to the program, data table, and database files.
Open an existing project 
To open an existing project, click File > Open, and select the project to open.
Enter rungs in the program 
When you open a new program file, the ladder file opens in the right pane of the application window. Click the end rung and from the toolbar click the New Rung icon to add a rung. To place an instruction on the rung, click the button for the instruction. You can place several instructions on a rung.
To add addresses, click an instruction then type the address in the empty text box. You can also drag and drop addresses from a data table file onto instructions.
Syntax for input address- I:0.0/0, I:0.0/1, I:0.0/2….. depending on the input selected.
Syntax for output address- O:0.0/0, O:0.0/1, O:0.0/2…. Depending on the output selected.
Verify your project 
Before you can compile and download your project, you must validate, or verify, the project. You can verify a single program file or you can verify the project. To verify a file, click the Verify File icon or click Edit > Verify File. To verify the project, click the Verify Project icon or click Edit > Verify Project. The Verify Results output window provides information about errors that would prevent compilation. Click on a result item to go to that location in the program.


Configure communication channel, download and go online 
Before going online you must define processor communication settings, such as baud rate, and also decide certain system and protocol controls. Depending on the type of processor that you are using and the method of communication (direct, networked, or modem), the complexity of this procedure varies.
1. Double-click the channel configuration icon in the project tree to make these settings. If you need information about any parameter, click Help on the Channel Configuration dialog box. 
2. Click Download > Comms to download the current offline program into the controller. Click Yes to go online.
Addressing
There are several methods to address instructions. You can enter an address by: 
• Typing the address. 
• Dragging addresses from data files or the Custom Data Monitor. 
• Copying and pasting from program to program.

# Online editing
The online editing function lets you monitor and correct your ladder program when you are connected to an SLC 5/03, SLC 5/04, SLC 5/05, MicroLogix 1100, or MicroLogix 1400 processor. Online editing includes inserting, replacing, and deleting rungs in a program while sonline with the processor.
