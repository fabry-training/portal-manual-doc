---
slug: /portal-manual/france/configuration
title: Configuration
---

## Configuration

Before starting with the configuration, the master data of the enterprise and the outlet has to be completed and checked. For this see chapter [_Master data_](company.md#company-master-data) and [_Outlets_](company.md#outlets)

### CashBox<a name="Cashbox"></a>

#### Creation of a CashBox

[![https://portal-sandbox.fiskaltrust.fr/CashBox](images/CashBox/CashBox.png "http://portal.fiskaltrust.fr/CashBox")](http://portal.fiskaltrust.fr/CashBox)
Creating the configuration containers

By opening the menu _Configuration_![Number 1](../images/Numbers/circle-1o.png) and clicking on _CashBox_![Number 2](../images/Numbers/circle-2o.png) the overview of all configured CashBoxes (configuration containers) is shown.
Click on [+&nbsp;Add]![Number 3](../images/Numbers/circle-3o.png) to create a new configuration container.

#### Add a CashBox

[![https://portal-sandbox.fiskaltrust.fr/CashBox](images/CashBox/Create.png "http://portal.fiskaltrust.fr/CashBox")](http://portal.fiskaltrust.fr/CashBox)
Configuration container - Add

![Number 1](../images/Numbers/circle-1o.png) In this field, you can change the name of the configuration container. It should be unique so a CashBox can be identified in even a long list.

![Number 2](../images/Numbers/circle-2o.png) If you are working in a network mode, enter the IP address of the endpoint here.

![Number 3](../images/Numbers/circle-3o.png) Click on \[Save\] to save the changes to the configuration container ad go back to the overview.

![Number 4](../images/Numbers/circle-4o.png) Clicking \[Cancel\] cancels the operation without saving the changes and show the overview.

#### Overview first CashBox<a name ="overview-firstcashbox"></a>

[![https://portal-sandbox.fiskaltrust.fr/CashBox](images/CashBox/CashBox-Details.png "http://portal.fiskaltrust.fr/CashBox")](http://portal.fiskaltrust.fr/CashBox)
Overview - First configuration container

![Number 1](../images/Numbers/circle-1o.png) After creating a CashBox, it is initially empty, it only has the _CashBoxID_ and the _AccessToken_ which are required to access the CashBox. It can be seen by opening the information section by clicking on the chevron on the beginning of the line.

![Number 2](../images/Numbers/circle-2o.png) This area shows all the assigned queues, helpers and SCUs for the configuration container. Since the CashBox has just been created and nothing is stored yet, the fields are empty.

![Number 3](../images/Numbers/circle-3o.png) By clicking on ![dotnet Launcher](../images/Buttons/024.png "dotnet Launcher") you can download the _dotnet Launcher_. This must be used if there is an internet connection to the POS-System.

![Number 4](../images/Numbers/circle-4o.png) The _dotnet useOffline Launcher_ should be used if no internet connection can be established. This can be downloaded by clicking on ![Download](../images/Buttons/025.png "Download").

![Number 5](../images/Numbers/circle-5o.png) For using the fiskaltrust.Service with a MacOS or Linux system the _mono useOffline Launcher_ is needed. It can be downloaded by clicking on ![mono Launcher](../images/Buttons/026.png "mono Launcher"). This is set to _useOffline_ by default.

![Number 6](../images/Numbers/circle-6o.png) The CashBox can be edited with a click on ![Drag&Drop](../images/Buttons/027.png "Drag&Drop") by Drag & Drop.

![Number 7](../images/Numbers/circle-7o.png) The CashBox can also be edited in a list view by clicking on ![List](../images/Buttons/028.png "List").

![Number 8](../images/Numbers/circle-8o.png) By clicking on ![Trash](../images/Buttons/029.png "Trash") an empty configuration container can be deleted.

#### Edit CashBox by Drag & Drop

[![https://portal-sandbox.fiskaltrust.fr/CashBox](images/CashBox/Edit-DragDrop.png "http://portal.fiskaltrust.fr/CashBox")](http://portal.fiskaltrust.fr/CashBox)
Edit CashBox by Drag & Drop

![Number 1](../images/Numbers/circle-1o.png) The first widget shows all the created queues in this account. This corresponds to a data acquisition protocol and therefore a POS-System.

![Number 2](../images/Numbers/circle-2o.png) The second widget shows all created Helpers, which can be used in a CashBox. For further information see chapter [_Helpers_](../handbook-general/configuration.md#helper).

![Number 3](../images/Numbers/circle-3o.png) The last widget contains all the SCUs created in this account and can be used in a CashBox, further information can be found in chapter [_Signature creation unit_](#SCU).<br />A SCU must not be directly associated to a CashBox. Because the configuration container has a connection to the outlet and the SCU is coupled to an outlet, a loose coupling exists between them. It is essential for legal compliance to use the same outlet number in the SCU-configuration and the CashBox-configuration.<br />This loose coupling enables the usage of a single SCU for more than one queue in the **same** outlet.

![Number 4](../images/Numbers/circle-4o.png) The field _Outlet_ is mandatory and must contain the number of a valid outlet. For further information see chapter [_Outlets_](company.md#outlets).

![Number 5](../images/Numbers/circle-5o.png) This field contains the active CashBox. Using Drag & Drop, units from the three widgets on the right side can be integrated in this CashBox.

Clicking on \[Save\] stores the changes to the configuration container.

#### Edit CashBox by List

Furthermore, the CashBox can be edited via a list.
[![https://portal-sandbox.fiskaltrust.fr/CashBox](images/CashBox/Edit-List.png "http://portal.fiskaltrust.fr/CashBox")](http://portal.fiskaltrust.fr/CashBox)
Edit CashBox by list

![Number 1](../images/Numbers/circle-1o.png) The list view is divided into three sections showing the available objects (_Queues_, _Helper_, _Signature Creation Unit_).

![Number 2](../images/Numbers/circle-2o.png) The required objects can be added to the cashbox by ticking the checkbox at the beginning of the row.

![Number 3](../images/Numbers/circle-3o.png) Click ![Gear](../images/Buttons/030.png "Gear") on the ending of a row to display the settings for each object.

![Number 4](../images/Numbers/circle-4o.png) Each Queue owns a certificate from a SCU for signing all the data send to it. With the button ![Certificate download](../images/Buttons/039.png "Certificate download") the certificate of a assigned SCU can be downloaded and verified.

![Number 5](../images/Numbers/circle-5o.png) For filtering all the tables/sections in this window at least 3 characters have to be entered.

#### Ready configured CashBox

[![https://portal-sandbox.fiskaltrust.fr/CashBox](images/CashBox/Cashbox-Detail-Configured.png "http://portal.fiskaltrust.at/CashBox")](http://portal.fiskaltrust.fr/CashBox)
Ready configured CashBox

![Number 1](../images/Numbers/circle-1o.png) By clicking on \[+&nbsp;Add\] you can create a new configuration container (CashBox).

![Number 2](../images/Numbers/circle-2o.png) In the section _Queues_ the deposited POS-System identification number (_CashBoxID_) as well as the automatically generated AES-key (Base64 encryption) (_AccessToken_) can be found.<br /> By clicking on ![Gear](../images/Buttons/030.png "Gear") the configuration of the queue can be edited.

![Number 3](../images/Numbers/circle-3o.png) In this section the connected helpers as well as the package name and version is shown. By clicking on ![Gear](../images/Buttons/030.png "Gear") each helper can be configured in its own window.

![Number 4](../images/Numbers/circle-4o.png) The connected signature creation units can be displayed here. But it is not necessary to connect a CashBox one-to-one to a SCU. Because a SCU can be used more than once for an outlet there is a loose connection between SCU and CashBox.

#### Delete a CashBox

For legal reasons it is currently not possible to delete a CashBox. However, there is one exception, that if the CashBox was not yet in use and is completly empty, it can still be deleted.

Before deleting a CashBox it has to be ensured that all elements from the configuration container are removed. Removing the element from the CashBox does not delete them, they are only put back in the general section for further use.<br />If a CashBox is not empty it can not be deleted.<br />By deleting a CashBox only the wrapping configuration container gets removed from the system. No data, certificate, queue, archives or anything else is touched or deleted.
[![https://portal-sandbox.fiskaltrust.fr/CashBox](images/CashBox/Delete.png "http://portal.fiskaltrust.fr/CashBox")](http://portal.fiskaltrust.fr/CashBox)
Delete CashBox

#### Download Launcher

[![https://portal-sandbox.fiskaltrust.fr/CashBox](images/CashBox/CashBox-Download-Launcher.png "http://portal.fiskaltrust.fr/CashBox")](http://portal.fiskaltrust.fr/CashBox)
Download Launcher

![Number 1](../images/Numbers/circle-1o.png) By clicking on one of these buttons, the launcher needed for commissioning is downloaded. This is a ZIP file that you download into the download folder. The zip-file can be founded in the local download-folder and extracted there for further use on a POS-System.
Be aware, that after changement in the configuration the \[Rebuild\]-button should be click before a launcher is downloaded.

For further information see chapter [Overview first CashBox](#overview-firstcashbox)

### Queue<a name="queue"></a>

[![https://portal.fiskaltrust.fr/Queue/](images/Queue/Queue.png "https://portal.fiskaltrust.fr/Queue/")](https://portal.fiskaltrust.fr/Queue/)
Overview of queues

To get to the creation and _Configuration_![Number 1](../images/Numbers/circle-1o.png) of a queue, click on the menu item _Queue_![Number 2](../images/Numbers/circle-2o.png).

To find a specific queue, a text can be entered in the search field![Number 3](../images/Numbers/circle-3o.png). Starting with the second entered character, the table beneath gets filtered automatically.

A click on the button _+&nbsp;Create new_![Number 4](../images/Numbers/circle-4o.png) adds a new queue to the account.

#### Add a queue<a name="add-a-queue"></a>

[![https://portal.fiskaltrust.fr/Queue/](images/Queue/Create.png "https://portal.fiskaltrust.fr/Queue/")](https://portal.fiskaltrust.fr/Queue/)
Queue - Adding

![Number 1](../images/Numbers/circle-1o.png) This field, holds the name of the queue. It can be anything which helps to identify each single queue in the account.

![Number 2](../images/Numbers/circle-2o.png) The appropriate storage method depending on your operating system can be selected. This value cannot be changed after the creation of the queue.

![Number 3](../images/Numbers/circle-3o.png) The package version can also be selected using a dropdown menu. For updating the package version a click on ![Refresh](../images/Buttons/008.png "Refresh") is mandatory.<br />**To configure the POS-System with a law compliant fiskaltrust.Service the correct package has to be selected. The certified version for the used POS-System, is written on the certificate. Your PosDealer or PosCreator knows which version is certified and must be used.**

![Number 4](../images/Numbers/circle-4o.png) Sets a timeout in milliseconds for the connection attempt with the signature creation unit.

![Number 5](../images/Numbers/circle-5o.png) The country in which the queue is used can be selected in this dropdown list. This value can not be changed after creation of the queue.<br />**For a law compliant configuration _France (FR)_ has to be chosen.**

![Number 6](../images/Numbers/circle-6o.png) This identification value has to be unique in the account. This value can not be changed after creation of the queue.

![Number 7](../images/Numbers/circle-7o.png) The \[Save\]-button creates the queue and stores it.

#### Queue configuration<a name="configure-a-queue"></a>

The configuration has to be done directly after the creation of a queue. Nevertheless it can be changed afterwards with the ![Configuration](../images/Buttons/009.png "Configuration") button in the queue overview.

[![https://portal.fiskaltrust.fr/Queue/](images/Queue/Configuration.png "https://portal.fiskaltrust.fr/Queue/")](https://portal.fiskaltrust.fr/Queue/)
Queue configuration

![Number 1](../images/Numbers/circle-1o.png) This box can be ticked to activate the verification of the connected certificate.

![Number 2](../images/Numbers/circle-2o.png) Activating this option speeds up the signing of the first certificate, but slows down the queue starting.

![Number 3](../images/Numbers/circle-3o.png) This line gives the possibility to add a key-value-pair to the configuration of the queue.<br />![Number 4](../images/Numbers/circle-4o.png) The ![add line](../images/Buttons/042.png "add line") button adds another line for a new pair and the ![remove line](../images/Buttons/043.png "remove line") button removes the line from the configuration.

![Number 5](../images/Numbers/circle-5o.png) The name of the queue can be changed in this field.

![Number 6](../images/Numbers/circle-6o.png) The type of storage can only be defined upon queue creation and can not be changed later on.

![Number 7](../images/Numbers/circle-7o.png) The package version can also be selected using a dropdown menu. For updating the package version a click on ![Refresh](../images/Buttons/008.png "Refresh") is mandatory.<br />**To configure the POS-System with a law compliant fiskaltrust.Service the correct package has to be selected. The certified version for the used POS-System, is written on the certificate. Your PosDealer or PosCreator knows which version is certified and must be used.**

![Number 8](../images/Numbers/circle-8o.png) The URL to access the queue can be defined in this field. By clicking on ![net pipe](../images/Buttons/012.png "net pipe") a URL is used, which is suitable for local use without internet connection, because no firewall settings are required. By clicking on ![http](../images/Buttons/013.png "http"), the system generates a URL with which the POS-System can access the queue. The URL can be renamed, to have it like this: http://localhost.1200/Queuefiskaltrust.<br />The ![add URL](../images/Buttons/042.png "add URL") button adds another line for a new URL and the ![remove URL](../images/Buttons/043.png "remove URL") button removes the URL from the configuration.

![Number 9](../images/Numbers/circle-9o.png) \[Save\] or \[Save and close\] saves the configuration of the queue (and closes the configuration module).

#### Queue overview<a name="queue-overview"></a>

By opening the _Queue_-Module in the _Configuration_-menu an overview from all created queues are shown.

[![https://portal.fiskaltrust.fr/Queue/](images/Queue/Queue-New.png "https://portal.fiskaltrust.fr/Queue/")](https://portal.fiskaltrust.fr/Queue/)
Queue overview

![Number 1](../images/Numbers/circle-1o.png) Clicking on the _chevron right_ shows the base information for this queue and the used CashBox, if already configured.

![Number 2](../images/Numbers/circle-2o.png) This column shows the localisation (for which country the queue is used) and the _CashBox identification_.

![Number 3](../images/Numbers/circle-3o.png) The third column contains a checkmark ![Checkmark](../images/Buttons/044.png "Checkmark") when the queue is activated. A _start receipt_ has been sent and the queue is ready to sign and chain receipts or already contains some receipts.<br />If this column is empty no start receipt has been sent or a _stop receipt_ was sent and the queue does not accept any receipts for chaining and signing.

![Number 4](../images/Numbers/circle-4o.png) A queue contains two type of journals. Both of them are chained and secured against changes and contain already transmitted receipts.<br />By clicking on ![ReceiptJournal](../images/Buttons/017.png "ReceiptJournal") all transmitted receipts are displayed in a list, see chapter [_ReceiptJournal of a queue_](#receiptjournal-of-a-queue).<br />By clicking on ![ActionJournal](../images/Buttons/018.png "ActionJournal") all important actions and status changes of the queue are shown in a list, see chapter [_ActionJournal of a queue_](#actionjournal-of-a-queue).

![Number 5](../images/Numbers/circle-5o.png) To stop the transmission from the local POS-System to the queue the ![Disable upload](../images/Buttons/045.png "Disable upload") button can be clicked. Starting from this moment the queue does not save any receipt in the cloud. With ![Reset upload](../images/Buttons/046.png "Reset upload") the queue receives all the untransmitted receipts from the moment the button is clicked. This can be take several days because the check for missing receipts is started by the first receipt saved in the local queue.

![Number 6](../images/Numbers/circle-6o.png) The queue export can be started by pressing the button ![Export](../images/Buttons/019.png "Export"). For further information see chapter [_Export a queue_](#export-a-queue).

![Number 8](../images/Numbers/circle-8o.png) The last column contains the commands to manage a queue.<br /> By clicking on ![Used french signature creation unit](../images/Buttons/021.png "Used french signature creation unit") the connected SCUs can be displayed and managed. For further information see chapter [_SCUs used by a queue_](#scus-used-by-a-queue).<br />Here the configuration of the queue can be opened by clicking on ![Configure queue](../images/Buttons/009.png "Configure queue"), see [_Configure a queue_](#configure-a-queue).<br />Clicking on ![Edit](../images/Buttons/005.png "Edit") edits the description, package version and timeout of the queue, see [_Edit a queue_](#edit-a-queue).<br />Clicking on ![Trash](../images/Buttons/011.png "Trash") deletes the queue. However, the button for deleting the queue **is inactive for legal reasons**, so no queue can be deleted after creation. The possibility to delete a queue does not depend on the status or the content of a queue. Once created no deletion is possible. 

[![https://portal.fiskaltrust.fr/Queue/](images/Queue/Queue-Filter.png "https://portal.fiskaltrust.fr/Queue/")](https://portal.fiskaltrust.fr/Queue/)
Filter the list of queues

With a large list of configured queues the overview can be hard. For this the view can be filtered by status of the queue by a click on the corresponding radio button.

#### SCUs used by a queue<a name="scus-used-by-a-queue"></a>

[![https://portal.fiskaltrust.fr/Queue/](images/Queue/QueueFRSCUList/inactive.png "https://portal.fiskaltrust.fr/Queue/")](https://portal.fiskaltrust.fr/Queue/)
Queue - Connected Signature Creation Devices (SCU)

![Number 1](../images/Numbers/circle-1o.png) By setting a check mark the SCU to be connected to the queue is selected.
![Number 2](../images/Numbers/circle-2o.png) The SIRET of the attached outlet to the SCU is shown.
![Number 3](../images/Numbers/circle-3o.png) Shows the serial number of the certificate used by this SCU.
![Number 4](../images/Numbers/circle-4o.png) With the button ![Download certificate](../images/Buttons/047.png "Download certificate") the certificate of the SCU can be downloaded.

![Certificate detail](images/Queue/QueueFRSCUList/certificate-detail.png)
Detail of a certificate

The content of the certificate can verified with a double click on it.

#### Edit a Queue<a name="edit-a-queue"></a>

[![https://portal.fiskaltrust.fr/Queue/](images/Queue/Edit.png "https://portal.fiskaltrust.fr/Queue/")](https://portal.fiskaltrust.fr/Queue/)
Edit a queue

![Number 1](../images/Numbers/circle-1o.png) The name of the queue can be changed with this field.

![Number 2](../images/Numbers/circle-2o.png) Various package versions can be selected by using the drop-down menu. These can be updated by clicking on ![Refresh](../images/Buttons/008.png "Refresh"). To take this change in effect on the POS-Systems, this has to be restarted.<br />**To configure the POS-System with a law compliant fiskaltrust.Service the correct package has to be selected. The certified version for the used POS-System, is written on the certificate. Your PosDealer or PosCreator knows which version is certified and must be used.**

![Number 3](../images/Numbers/circle-3o.png) Sets a timeout in milliseconds for the connection attempt with the signature creation unit.

All other values shown on the page are read-only and cannot be changed. This value shows the current state of the queue and the saved counters of the different receipt types.

At the bottom of the page the buttons \[Save\] or \[Save and close\] saves the configuration of the queue (and closes the configuration module).

#### ReceiptJournal of a Queue<a name="receiptjournal-of-a-queue"></a>

[![https://portal.fiskaltrust.fr/Queue/](images/Queue/ReceiptJournal.png "https://portal.fiskaltrust.fr/Queue/")](https://portal.fiskaltrust.fr/Queue/)
Queue - Overview ReceiptJournal

This journal shows all receipt created by a POS-System connected to the fiskaltrust.Service. All _special receipt types_ like a closure receipt, an archive request or warnings are shown in the [ActionJournal](#actionjournal-of-a-queue).

![Number 1](../images/Numbers/circle-1o.png) This dropdown limits the shown rows of a journal to 50, 100, 500 or a full list. If the journal is long, a _full list_ can take some time to be shown.

![Number 2](../images/Numbers/circle-2o.png) This dropdown list defines the type of receipt shown.

![Number 3](../images/Numbers/circle-3o.png) The first column shows the date/time the receipt was created.

![Number 4](../images/Numbers/circle-4o.png) Shows the overall counter of all receipts in the queue.

![Number 5](../images/Numbers/circle-5o.png) Shows the receipt number created by the fiskltrust.Service.

![Number 6](../images/Numbers/circle-6o.png) The button ![Show Receipt](../images/Buttons/023.png "Show receipt") displays the respective receipt.

#### Detailed receipt

[![https://portal.fiskaltrust.fr/Queue/](images/Queue/ShowReceipt.png "https://portal.fiskaltrust.fr/Queue/")](https://portal.fiskaltrust.fr/Queue/)
Queue - Detailed receipt

After selecting a receipt, it is displayed as follows. This view makes it possible to verify the accuracy of the receipt content.

#### ActionJournal of a Queue<a name="actionjournal-of-a-queue"></a>

[![https://portal.fiskaltrust.fr/Queue/](images/Queue/ActionJournal.png "https://portal.fiskaltrust.fr/Queue/")](https://portal.fiskaltrust.fr/Queue/)
Queue - Overview ActionJournal

This list shows all _special receipt types_ of a queue. For regular receipts see [ReceiptJournal](#receiptjournal-of-a-queue). A click of the right chevron![Number 1](../images/Numbers/circle-1o.png) opens the detailed view of the data of the receipt.

#### Export a queue<a name="export-a-queue"></a>

[![https://portal.fiskaltrust.fr/Queue/Exports/](images/Queue/Exports.png "https://portal.fiskaltrust.fr/Queue/Exports/")](https://portal.fiskaltrust.fr/Queue/Exports/)
Queue - Overview Exports

An overview of all running and finished exports of the account can be seen in the menu _Tools_![Number 1](../images/Numbers/circle-1o.png) and submenu _Export_![Number 2](../images/Numbers/circle-2o.png).

![Number 3](../images/Numbers/circle-3o.png) A line of the table represents an export. By clicking on the chevron on the right more details of the export can be shown. If the export finished successfully, a list of downloadable archives is shown.

![Number 4](../images/Numbers/circle-4o.png) By clicking on the filename this file is transfered from the fiskaltrust.Storage to the local system. 

![Number 5](../images/Numbers/circle-5o.png) The column _Formats_ shows all exported journals and formats as its own icon. For information regarding which format and/or journal is included in the export a tooltip is shown by each icon.

![Number 6](../images/Numbers/circle-6o.png) In the third column the location of the files ![Location](../images/Buttons/048.png "Location") is shown or if the export is running ![Exporting](../images/Buttons/008.png "Exporting").

![Number 7](../images/Numbers/circle-7o.png) The column _State_ shows information to the export. Until the export is finished no detailed information is given. After the export is finished, the chains and paths are shown. In the second line the user is informed if errors occurred or exist in the chain.

![Number 8](../images/Numbers/circle-8o.png) In the last column the number of exported receipts are shown and which queue id is concerned.

![Number 9](../images/Numbers/circle-9o.png) To create a new export a click on [+&nbsp;Create&nbsp;new&nbsp;export] can be done. This function can be called directly with the button ![Export a queue](../images/Buttons/019.png "Export a queue") from the queue configuration too, see chapter [_Queue overview_](#queue-overview).

#### Create a new export for a queue

[![https://portal.fiskaltrust.fr/Queue/Exports/](images/Queue/ExportConfiguration/ExportConfiguration.png "https://portal.fiskaltrust.fr/Queue/Exports/")](https://portal.fiskaltrust.fr/Queue/Exports/)
Create new export for a queue

![Number 1](../images/Numbers/circle-1o.png) The first and the last receipt number for the export can be defined. By leaving the field open, the information about date and time will be shown at the end points of the slider![Number 4](../images/Numbers/circle-4o.png).

![Number 2](../images/Numbers/circle-2o.png) The date and time for the first receipt to export can be defined. By leaving the field open, the information about date and time will be shown at the end point of the slider![Number 4](../images/Numbers/circle-4o.png).

![Number 3](../images/Numbers/circle-3o.png) The date and time for the last receipt to export can be defined. By leaving the field open, the information about date and time will be shown at the start point of the slider![Number 4](../images/Numbers/circle-4o.png).

![Number 4](../images/Numbers/circle-4o.png) The range of exported receipts can be adjusted by sliding the end points of the slider.

![Number 5](../images/Numbers/circle-5o.png) The drop area holds all the export formats, journals and storages for an export. It can be filled by dragging the elements on the right side, to this area.

![Number 6](../images/Numbers/circle-6o.png) Formats and journals available for an export.<br />The element _Full export (xml)_ creates an archive in xml-format with all receipt types in the selected range. The export result at least two files. The file _XML.fileid.full.xml_ contains all the archived receipts and the file _XML.fileid.path#.xml_ contains the chain of the full journal. If there is more then one path in the queue, for each path a single xml-file is created.<br />All other elements create an archive of the mentioned receipt type. This archive is downloadable as zip-file and contains a single csv-file in plain text with the range of the exported receipts.<br />
With a click on ![Gear](../images/Buttons/030.png "Gear"), the used filename can be changed.

[![https://portal.fiskaltrust.fr/Queue/Exports/](images/Queue/ExportConfiguration/ExportConfiguration-ConfigFile.png "https://portal.fiskaltrust.fr/Queue/Exports/")](https://portal.fiskaltrust.fr/Queue/Exports/)
Change filename of an archive to export

Each element from the format section can be used only once per export.

![Number 7](../images/Numbers/circle-7o.png) This element defines the storage location of an export. This element can be used more than one time for an export. This offers the possibility to save an export in more than one place at the same time.<br />
The element _Database to Azure-Storage_ exports the database to the used Azure-Storage.<br />
With _Azure-Storage_ another personal storage at Azure can be used to save the export. To use this element the access credentials have to be defined with a click on ![Gear](../images/Buttons/030.png "Gear") this element.

[![https://portal.fiskaltrust.fr/Queue/Exports/](images/Queue/ExportConfiguration/ExportConfiguration-ConfigAzureStorage.png "https://portal.fiskaltrust.fr/Queue/Exports/")](https://portal.fiskaltrust.fr/Queue/Exports/)
Define credentials for the Azure Storage to save the export

The location element _FTP-Server_ offers a ftp-transfer of the exported archives. This element can be used when the ftp-credentials are entered after a click on ![Gear](../images/Buttons/030.png "Gear") this element.

[![https://portal.fiskaltrust.fr/Queue/Exports/](images/Queue/ExportConfiguration/ExportConfiguration-ConfigFTP.png "https://portal.fiskaltrust.fr/Queue/Exports/")](https://portal.fiskaltrust.fr/Queue/Exports/)
Define credentials for a FTP-Server to save the export

All entered credentials are not saved from the fiskaltrust.Portal. They are only used once for saving the export in the defined location.

![Number 8](../images/Numbers/circle-8o.png) The click on [Start export and close] queues the export and closes the window. The status of the export can be verified in the list of exports of the queue, see [_Export a queue_](#export-a-queue).

### Signature creation unit (SCU)<a name="SCU"></a>

The SCU is the part of the fiskaltrust.Service for securing all the receipts sent to it. In France the SCU is the holder of the certificate to guarantee the unalterability, securtiy, conservation and archiving of the transmitted data.

#### Overview of signature creation units

[![https://portal.fiskaltrust.fr/SignatureCreationUnit/](images/SignatureCreationUnit/SignatureCreationUnit.png "https://portal.fiskaltrust.fr/SignatureCreationUnit/")](https://portal.fiskaltrust.fr/SignatureCreationUnit/)
Overview - Signature Creation Units (SCU)

To find a specific SCU, a text can be entered in the search field![Number 1](../images/Numbers/circle-1o.png). Starting with the second entered character the table beneath gets filtered automatically.

![Number 2](../images/Numbers/circle-2o.png) Clicking on [+&nbsp;Create] opens the module for creating a new signature creation unit, see [_Creation of a SCU_](#creation-of-a-scu).

![Number 3](../images/Numbers/circle-3o.png) The SIRET used by the SCU is displayed here. This reflects the loose coupling of the SCU to the outlet, see for more information chapter [_Outlets_](company.md#outlets).

![Number 4](../images/Numbers/circle-4o.png) Shows the serial number of the certificate of the SCU. 

![Number 5](../images/Numbers/circle-5o.png) Each SCU holds a certificate for signing all the data send to it. With the button ![Certificate download](../images/Buttons/047.png "Certificate download") the certificate of this SCU can be downloaded and verified.

![Number 6](../images/Numbers/circle-6o.png) Click on ![Delete SCU](../images/Buttons/029.png "Delete SCU") to delete the SCU. However, the button to delete any signature creation unit is currently inactive for legal reasons, so no SCU can be deleted.

#### Creation of a SCU<a name="creation-of-a-scu"></a>

[![https://portal.fiskaltrust.fr/SignatureCreationUnitFR/](images/SignatureCreationUnitFR/Create.png "https://portal.fiskaltrust.fr/SignatureCreationUnitFR/")](https://portal.fiskaltrust.fr/SignatureCreationUnitFR/)
Adding a signature creation unit

To create the signature creation unit, command _Signature creation device_![Number 2](../images/Numbers/circle-2o.png) in the _Configuration_![Number 1](../images/Numbers/circle-1o.png) menu. A click on [+&nbsp;Create] opens the page for adding a new SCU to the company.

In the dropdown list all [outlets](company.md#outlets) of the company are shown. To create a SCU, an outlet has to be selected. It is not necessary to create more then one SCU for an outlet, but at least one per outlet has to be created. It is not possible to use one signature creation unit for more then one outlet because the SIRET of the selected outlet is used to created the certificate for each SCU.

#### Add signature creation unit

To connect a SCU to a CashBox or more specifically to a queue see [Outlets](company.md#outlets) and[SCUs used by a queue](#scus-used-by-a-queue)

#### Delete a signature creation unit

The button for deleting a signature creation unit is, for legal reasons, inactive. No created SCU can be deleted from the fiskaltrust.Service. In the future there will be a filter to hide unused or inactive SCUs.

### Template

[![https://portal.fiskaltrust.fr/Template/](images/Template/Template.png "https://portal.fiskaltrust.fr/Template/")](https://portal.fiskaltrust.fr/Template/)
List of available templates

Instead of creating and configuring a CashBox manually, a template (payable or free of charge) can be used. This preconfigured template can be purchased in the fiskaltrust.Shop. With this kind of template many similar CashBoxes can be created easily and further used as described in the chapter [_CashBox_](#cashbox).

If you are in need of templates for creating and configurating CashBoxes, do not hesitate to contact the support at contact@fiskaltrust.fr. fiskaltrust France is happy to help you to reach this goal.

The template management can be found in _Configuration_![Number 1](../images/Numbers/circle-1o.png) at the command _Template_![Number 2](../images/Numbers/circle-2o.png)

![Number 3](../images/Numbers/circle-3o.png) In the first column the template name is shown. More information regarding the template will be shown after a click on the chevron right.

![Number 4](../images/Numbers/circle-4o.png) Shows the status of the template. It can be completely deactivated, visible for everyone or only for connected PosDealers and/or PosOperators.

![Number 5](../images/Numbers/circle-5o.png) A click on [+&nbsp;Create new] creates a new template from scratch.

![Number 6](../images/Numbers/circle-6o.png) A click on ![Clone template](../images/Buttons/033.png "Clone template") clones the template and opens the newly created template for changes.

![Number 7](../images/Numbers/circle-7o.png) The button ![Edit](../images/Buttons/005.png "Edit") opens the template for changes.

#### Create template

[![https://portal.fiskaltrust.fr/Template/](images/Template/Create.png "https://portal.fiskaltrust.fr/Template/")](https://portal.fiskaltrust.fr/Template/)
Create a template

The first two fields give the template a clear name and description. In the field _Content_ the commands for this template are saved. This will be normally prefilled from the fiskaltrust.Support.<br />
In _ImageUrl_ an absolute URL to a kind of product image can be stored. For more description of this template an absolute URL can be entered in _LinkUrl_.<br />
The dropdown list in _Mode_ defines the access rights for a template by choosing one of the elements.

A template always start with

```
{ "ftCashBoxId": "|[cashbox_id]|",​
     "ftQueues": [​{​"Id": "|[queue0_id]|",
```

Then add queue type: `"Package": "fiskaltrust.service.azure",`
The type of packages can be found in the dropdown list of [creating a new queue](#add-a-queue).

Then introduce queue parameters, anew block has to be started: `"Configuration": {`

For example a connection string can be included `"connectionstring": "DefaultEndpointsProtocol=http://endpoint.cloud;AccountName=ftRealAccountName;AccountKey=TheACcountKey;",`

or other queue parameter, like `"asscdtretry": 2,`

Then beginning of the queue core starts with

```
"init_ftQueue": [{ "ftQueueId": "|[queue0_id]|",
                   "ftCashBoxId": "|[cashbox_id]|",
                   "CountryCode": "FR",
                   "Timeout": 15000 }],
```

and the specific of the country

```
"init_ftQueueFR": [ { "ftQueueFRId": "|[queue0_id]|",
```

but also the queue name

```
"CashBoxIdentification": "ChaîneCloud|[count]|" } ],
```

then the SCU that this queues connect to:

```
"ftSignaturCreationUnitFRId": "|[scu0_id]|",
```

and the SIRET used for this queue:

```
"Siret": "|[siret]|",
```

To initialize a SCU for a queue the following block can be used:

```
"init_ftSignaturCreationUnitFR": [{
        "ftSignaturCreationUnitFRId": "|[scu0_id]|",
        "Siret": "|[siret]|"
    }
```

As last parameter the endpoint for the ChaîneCloude product has to be defined:

```
"Url": ["https://signaturcloud-azure-sandbox.fiskaltrust.fr/"]
```

**Example of a standard template:**

```
{
    "ftCashBoxId": "|[cashbox_id]|",
    "ftQueues": [{
            "Id": "|[queue0_id]|",
            "Package": "fiskaltrust.service.azure",
            "Configuration": {
                "connectionstring": "|[signaturcloud-storage-connectionstring]|",
                "init_ftQueue": [{
                        "ftQueueId": "|[queue0_id]|",
                        "ftCashBoxId": "|[cashbox_id]|",
                        "CountryCode": "FR",
                        "Timeout": 15000
                    }
                ],
                "init_ftQueueFR": [{
                        "ftQueueFRId": "|[queue0_id]|",
                        "ftSignaturCreationUnitFRId": "|[scu0_id]|",
                        "Siret": "|[siret]|",
                        "CashBoxIdentification": "ChaîneCloud|[count]|"
                    }
                ],
                "init_ftSignaturCreationUnitAT": [],
                "init_ftSignaturCreationUnitFR": [{
                        "ftSignaturCreationUnitFRId": "|[scu0_id]|",
                        "Siret": "|[siret]|"
                    }
                ]
            },
            "Url": ["https://signaturcloud-azure-sandbox.fiskaltrust.fr/"]
        }
    ]
}```
