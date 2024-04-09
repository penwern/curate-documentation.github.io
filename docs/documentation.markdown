<link rel="stylesheet" href="/style.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@mdi/font@7.4.47/css/materialdesignicons.min.css">
<script>
document.addEventListener('DOMContentLoaded', function() {
  // Find all nav links with submenus
  document.querySelectorAll('.md-nav--secondary .md-nav__link').forEach(function(link) {
    const parentLi = link.closest('.md-nav__item');
    const submenu = parentLi.querySelector('.md-nav');
    if (submenu) {
      // Initially collapse all submenus
      submenu.style.display = 'none';

      // Add expand/collapse button
      let chevron = document.createElement('span');
      chevron.classList.add('mdi', 'mdi-chevron-down');
      chevron.style.cursor = 'pointer';
      link.appendChild(chevron);

      // Attach click event to toggle submenu
      chevron.addEventListener('click', function(e) {
        e.preventDefault();

        // Toggle the mdi-chevron icon
        chevron.classList.toggle('mdi-chevron-down');
        chevron.classList.toggle('mdi-chevron-up');

        // Toggle only the direct submenu visibility
        if (submenu) {
          submenu.style.display = submenu.style.display === 'none' ? '' : 'none';
        }

        // Collapse nested submenus when parent is expanded to ensure only the first layer is visible
        if (!chevron.classList.contains('mdi-chevron-down')) {
          const nestedSubMenus = submenu.querySelectorAll('.md-nav');
          nestedSubMenus.forEach(nestedSubMenu => {
            nestedSubMenu.style.display = 'none';
            // Find and reset chevrons in nested menus
            const nestedChevrons = nestedSubMenu.closest('.md-nav__item').querySelectorAll('.mdi-chevron-up');
            nestedChevrons.forEach(nestedChevron => {
              nestedChevron.classList.remove('mdi-chevron-up');
              nestedChevron.classList.add('mdi-chevron-down');
            });
          });
        }
      });
    }
  });
});

</script>

<img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image1.png" style="width: 10em;"></img>

# Penwern Curate <span style="font-size: 8pt;vertical-align: super;">TM</span>

Penwern Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> is a comprehensive software platform that addresses
the fundamental issues with existing Digital Archiving solutions,
allowing organisations of any size to build, preserve and manage
best-practice Digital Archives with ground-breaking speed and
simplicity.

## Why is eArchiving important for any organization?

Valuable digital content can be become inaccessible, unusable, or
untrustworthy due to a number of factors, such as:

-   Files have been damaged or made inaccessible by viruses or malware.

-   Files are corrupted.

-   File types have become obsolete or software to read them is not
    available.

-   The authenticity of the data is in question as you cannot prove that
    a file hasn't changed.

-   You cannot find specific files due to a lack of understandable
    organisation or description.

Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> helps to fix these problems by:

-   Removing threats due to viruses and malware through a system or
    virus checks and quarantine.

-   Checksumming all files and regularly checking the integrity of files
    in its store.

-   Characterising file types by MIME type and Pronom ID so that you can
    monitor your holdings and take decisions on strategies to manage
    file type and software obsolescence.

-   Automatically extracting technical metadata.

-   Allowing you to organize your file-store any way you wish, but also
    to add descriptive metadata to files and folders so that you can
    search on multiple attributes.

-   Allowing you to retain all meta-information, and uniquely associate
    it with each object.

-   Allowing you to perform format migration on your objects to
    normalise their types to archival standards.

-   Preparing your content into standards-conformant information
    packages.

## Is Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> Useful for Archivists and Digital Curators?

Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> is a platform that can be used to provide a number of
critical functions within an electronic archiving system discretely or
can form a complete and effective system itself. Individually,
Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> can perform the following roles:

Upload and Accession

Smart Deposit System

Metadata Extraction

Transcriber

Fixity Agent

Appraisal System

Selection and Arrangement Workspace

Reporting System

Unified Description Tool

Digital Preservation System

OAIS Information Packaging

Document Editing

Advanced Access System

Public Access Portal

In combination, these services mean that Curate comprises a
comprehensive and highly capable electronic archiving system all on its
own.

## Is Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> Useful for Business?

Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> is a file sharing platform that integrates the features
required for the preservation of data that go beyond basic data
protection (back-up, integrity checking, disaster recovery).

The standards-based principles of digital preservation and eArchiving
that Curate is built upon are rapidly becoming critical functions for
all businesses to practice. Curate removes many of the significant
barriers to entry that prevent businesses from effectively implementing
digital preservation and eArchiving.

It is cost effective, allowing you to create an archive for inactive
data that doesn't take up valuable storage on your primary storage
systems and allows you to consolidate data into a single platform.
Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> works in a way your users understand, with a best-in-class
user experience. You don't have to train all your users on new, complex
digital preservation applications.

## Curate User Manual

## General

### Devices

Curate is supported on any device: computers, phones, and tablets.
Simple navigate to your Curate instance via your device's web-browser.
You may find compatibility issues with older or unsupported operating
systems.

### Log In

After navigating to your Curate instance, you will be asked to log in.
Curate can be configured to use external SSO providers, if desired by
your organisation. It can also integrate with LDAP/Active directory. If
multi-factor authentication is enabled (hardware and software
supported), you will be prompted to provide it. Your SSO and log-in
security requirements will have been discussed and integrated during
your signup.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image2.png" style=""></img>
</div>

## Application Areas

### Home Screen

When you log in to Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> you will see the home screen as shown
below and you will be guided through a short welcome tour. The home
screen provides you with links to recent content, and ways to navigate
through the rest of the application.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image3.png" style=""></img>
</div>

In the centre-top of the home screen, you will find the search bar. At
the far left, you can see the navigation panel.

You can find your account settings and preferences, as well as the
option to log out, by clicking on the profile icon in the navigation
panel.

Beneath that is the home button, which will return you to this screen.

At the bottom of the navigation panel, you can find your notifications
centre by hovering over the bell icon.

You can also switch between light and dark colour modes with the toggle
at the very bottom of the navigation panel.

### Bookmarks


The bookmarks tab can be accessed from the icon in the navigation panel. 
The bookmarks tab keeps references to all the files and folders you have 
saved using the "bookmark" feature [(*see bookmarking a file or folder*)](#bookmarking-a-file-or-folder). 
Clicking one of the items will navigate you to its location in Curate. 
If you want to remove an item from your bookmarks, click the <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image4.png" class="text-icon"style=""></img> icon 
next to the item you wish to remove.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image5.png" style=""></img>
</div>

### Workspaces

To open your workspaces panel, hover over the "All Files" button in the
navigation panel.

You will see the following spaces:

-   Personal files

-   Quarantine Space

-   Appraisal Space

-   Archive Space

-   Common Files

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image6.png" style=""></img>
</div>

Workspaces are where you perform your eArchiving workflow within Curate,
and where you'll be able to describe, arrange and eventually preserve
your objects.

Each workspace can be individually encrypted at the data source and
given its own independent fixity checking schedule.

Each workspace has a defined function, here is a quick explanation of
what each workspace is for:

#### Personal Files

This is a workspace that is only visible to you and not to other members
of your workgroup. You can upload files or folders to this space for
your own personal content, which would not normally be part of a group
archive.

Files uploaded into Personal are virus checked once and cannot be moved
out into any other area of Curate <span style="font-size: 8pt;vertical-align: super;">TM</span>.

If you have files in Personal that you later want to add to the archive,
you will need to re-upload into Quarantine, or if you don't have a local
copy, download from Personal and then re-upload into Quarantine.

Files in Personal are not characterised, but you do have basic file
information available and you can add descriptive metadata. Note that
file downloads do not include descriptive metadata so the Personal
workspace should not be used for appraisal or arrangement of archival
content.

#### Quarantine Space

Content that is to be appraised and arranged in Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> should be
uploaded into the Quarantine workspace [*see upload and ingest for more
information*](#upload-and-ingest). This is a shared workspace and so is visible to all
members of a workgroup. Uploaded files are virus checked and quarantined
for 30 days. It is recommended that files should not be moved from the
Quarantine workspace until the quarantine period is up, however
Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> is not prescriptive and you can do this.

If the virus scanner detects a virus or malware then the affected file
will be moved to a folder called Infected within the Quarantine
workspace.

After the 30-day quarantine period and a second successful virus scan,
files are moved automatically into the Appraisal space into a folder
called Released (but note that this folder will not appear until it is
needed).

#### Appraisal Space

Files moved to the Appraisal space are characterised by the open-source
file characterisation tool Siegfried, which generates a file type unique
identifier from the PRONOM registry of filetypes maintained by the
National Archive (see <https://www.nationalarchives.gov.uk/PRONOM/>).

If you search in PRONOM by a file's unique identifier you will be able
to see detailed information on the file format. Within the Appraisal
workspace you can move, copy and delete files, create folders and add
descriptive metadata. Using detailed file information you can make
appraisal decisions. From the appraisal space, you can also preserve and
package your objects in any configuration you wish. [*See preserving and
packaging objects for more information.*](#)

#### Archive Space

Files and folders can be moved to the Archive workspace for long-term
retention. The organisation of the workspace is up to you, but the
search function can help any system you have by allowing simple searches
on filenames or advanced searches on descriptive metadata. Files,
folders or packages moved to the Archived File workspace are read only
(you cannot delete or edit them) and cannot be moved, but you can create
a copy into another workspace.

#### Common Files Space

The Common Files space is a shared area within a workgroup that can be
used to store shared reference documents and files, for example: user
guides, references, submission agreements, metadata schemas etc.

### Object information area

The object information area provides you with all the critical details
about a file or object inside Curate. The object information area will
appear on the right-hand side of the screen when you select a single
file or folder.
<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image7.png" style=""></img>
</div>
#### Object information area panels

##### File actions panel

The first panel in the object information area is file actions, which
shows a preview of the object you have selected and presents options to
share, download, or open the file in one of Curates rendering tools.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image8.png" style=""></img>
</div>

##### File information panel

The file information panel lists all the basic characteristics of the
selected object, along with the quarantine status, scan results and
detailed characterization information when the file has been appraised.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image9.png" style=""></img>
</div>

##### Extracted metadata panels; EXIF etc

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image10.png" style=""></img>
</div>

When you select a file that includes some
additional technical metadata, like a photograph with EXIF, Curate will
automatically extract it and display it in a new card in the object
information area. Click on "more" to view the full extracted EXIF data.

##### Metadata panel

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image11.png" style=""></img>
</div>

Clicking on any file or folder in Curate
will summon the metadata panel in the object information area. The
Curate metadata panel comes with simple 15 field Dublin Core and 26
field ISAD(G) schemas built in. Any additional standardised or
customized schemas can be supported upon request. There is also a field
for custom tags, which are displayed as colourful tags in the file list.

The metadata panel also contains the "import" and "export" sections. The
import section allows you to import external DC, ISAD or any other
associated meta file to an object. It also provides fields for entering
the details of an external OAI-PMH record, from which you can harvest
and import its metadata. See [*importing metadata*](#) for more. The export
section allows you to make an object harvestable via your Curate systems
OAI-PMH server. See [*exporting records*](#) for more detail.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image12.png" style=""></img>
</div>

##### Comments

Each object in Curate has its own comments section that lets you leave
notes or comments for yourself or your colleagues.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image13.png" style=""></img>
</div>

##### File activity

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image14.png" style=""></img>
</div>

The final panel in the object information area, when a file or folder is selected in the file list, 
is the file activity panel. The file activity panel records and displays a log of
all the actions and modifications taken that relate to the selected
object. Please note that the activity stream does not record PREMIS
preservation events. Those are recorded internally. See [*PREMIS in
Curate*](#) for more information.

## Upload and Ingest

### Uploading Files and Folders into Quarantine

Files and Directories can be simple and quickly uploaded into
Curate <span style="font-size: 8pt;vertical-align: super;">TM</span>, but only into the Personal and Quarantine workspaces. If
files are uploaded into the Personal workspace they cannot be moved out
into any other workspace. Any file which is uploaded or moved into the
Quarantine workspace will be virus checked and a visual indication given
if the virus check was successful and the file virus free. Any file that
is found with a virus is immediately moved to a folder within the
Quarantine workspace called Infected. Files will be automatically
re-scanned for viruses after 30 days if they are left in the Quarantine
workspace, after which time they are then labeled Virus Free and
available for Release. Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> does not stop you from moving files
out of Quarantine at any time you wish.

### Advanced Web-uploader

The advanced web-uploader is the main ingest tool in Curate. It's fast,
efficient and offers several useability benefits over other, lower level
upload methods. The advanced web-uploader can handle ingests of
thousands of files and tens of gigabytes, making it capable of
processing most common ingest workloads.

<div class="tip"><span class="mdi mdi-information-outline"></span><span>If you have thousands of files to upload, you can compress your
objects into an archive package locally and then upload that instead.
This will greatly improve your upload performance.</span></div>

We would strongly recommend using the advanced web-uploader for the
majority of your ingests, where the size and volume is appropriate.

*If you need to ingest content using another protocol, either to adhere
to institutional policy or for workloads that are larger than the
webuploader is able to handle, please read the* *Curate Mission Control
and SFTP sections*

Try uploading files and folders (you can upload any complex folder
structure) using the advanced web-uploader. You can do this by selecting
'New' at the top of the screen, and then Upload.

You can drag and drop into the pop-up box or select to upload files or
folders. If you are uploading a large file or folder you can minimize
the upload window by clicking the X in the top right. You can then carry
on working and see the progress of the upload at any time by clicking
the 'Jobs Running' area at the bottom left of the window. New upload
jobs can be added at any time and will just be added to the upload
queue.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image15.png" style=""></img>
</div>

You can also simply drag your objects into the Curate window with the
appropriate location open and the content will be uploaded directly.

#### Web-uploader Options

When using the Curate web-uploader, you can also set configuration
options that dictate how Curate handles certain situations that can be
dangerous to an archiving workflow.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image16.png" style=""></img>
</div>

**Start uploading automatically**

Selecting this option means that each file you add to the uploader will
begin to upload immediately. If you disable this option, you can begin
to load all of the parts of an upload before beginning pieces of it at a
time. This can help you manage complex or large uploads on a sub-optimal
connection.

**Close panel after upload is finished**

Enabling this option will close the upload panel as soon as the final
file has finished uploading to Curate. Leaving this option disabled will
allow you to browse your completed uploads in the panel and at-a-glance
verify that they have valid integrity checks [*see pre-upload integrity
verification*] (#Pre-upload-integrity-verification).

**If a file with the same name exists**

These exclusive options allow you to dictate how Curate handles uploads
of files with duplicate names. Note that this does not check for
duplicates based on their content, only their name. You should generally
avoid uploading multiple files with the same name to a single folder or
area intentionally. If you select "rename files", each file with a
duplicated name will have a numbered suffix. "merge folders" means that
files inside a folder with a duplicated name will instead be uploaded to
the original folder. Any duplicated files within the merged folder will
be treated with the "rename files" process.

#### Pre-upload Integrity Verification

When uploading objects using the Curate web-uploader, it automatically
generates and compares pre and post-upload checksums. A label indicating
the result of each files integrity check will appear underneath each
item in the uploader window.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image17.png" style=""></img>
</div>

Each of your files will also have a label attached which permanently
records the result of the integrity check.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image18.png" style=""></img>
</div>

### SFTP

Curate offers a connection to your workspaces over SFTP, allowing you to
ingest more massive uploads of content into your quarantine space than
the advanced web-uploader can handle. The SFTP protocol is more capable
for massive uploads than HTTPS used in the advanced web-uploader, but
uploading through SFTP in Curate necessitates a system reindex.

As a result, you will either need to schedule your planned SFTP upload
with us ahead of time or, if the workload is not time critical, feel
free to contact us once the upload has completed.

If you require SFTP upload in your Curate instance, please let us know
when you procure Curate for your organisation, or send us a support
ticket.

*Remember, we'd strongly advise you to use the advanced web-uploader for
most ingest usecases. It's best to only use sftp if your institution
explicitly requires it.*

#### Connecting to and Uploading Through SFTP

You can connect to your Curate workspaces over SFTP using any common FTP
client. If SFTP is enabled for your Curate instance, you will be
supplied the relevant connection details by email when they are
provisioned.

#### SFTP Integrity Verification

Warning: it is difficult to maintain integrity verification for all your
ingested files when uploading through SFTP. Many FTP clients offer often
poor support for checksum features integrated with the protocol, as a
result Curate is unable to automatically verify your SFTP uploads
integrity.

To resolve this, you will need to generate a JSON manifest of checksums
for your ingest content before you perform your SFTP upload, and then
perform manual ingest integrity verification once it is complete. *See
Manual Ingest Integrity Verification for more information.*

<div class="tip"><span class="mdi mdi-information-outline"></span><span>
mission control features powerful uploading capabilities, as
performant as SFTP, as well as checksum generation. It's always strongly
recommended to use mission control over SFTP for massive ingests for a
faster, more robust, less fragmented and more pleasant user experience.
</span></div>

Once you have generated your checksum manifest, you may proceed to
upload your content via SFTP. Once your content is uploaded, and we have
completed the necessary reindex, you can upload your checksum manifest.
*See Manual Integrity Verification for more information*

### Curate Mission Control

For massive ingest workloads that exceed the capabilities.

### Ingest Integrity Verification

Curate offers powerful methods for ingesting content into the system
which come with automated facilities for verifying that your files were
not compromised as they were uploaded to the system.

Uploads using either the Advanced Web-uploader or mission control will
have their integrity verified completely automatically. Curate will
notify you with status tags attached to the respective object if any
items in your ingest workload are found to have been compromised during
the upload process.

Uploads using SFTP require manual checksum verification, which you can
read more about below.

###  Manual Ingest Integrity Verification

If you spot an inconsistency in the checksums or verification results
generated by Curate during your ingest upload, if you'd like to manually
verify that the automatic validation was completed successfully, or if
you have chosen to upload your content using SFTP, you might need to
perform manual ingest integrity verification.

To perform manual ingest integrity verification, follow these steps:

#### Generating a checksum manifest

There are free several tools available to do this, but we would strongly
recommend using our companion tool "mission control". *See Curate
mission control for more information.*

<div class="tip"><span class="mdi mdi-information-outline"></span><span>
For best practice, we recommend uploading your checksum manifest
separately through the advanced web-uploader. This ensures the manifest
itself was uploaded without issue.
</span></div>


### Quarantine

#### Results

Once a file has been uploaded, the initial quarantine virus scan will
run and you will see a tag appear on the file listing. You can find
detailed results for each scan in the quarantine process in the file
information panel, see *file information panel* for more detail.

##### Quarantined

"Quarantined" indicates that the file has been successfully scanned and
no immediate threats were detected. The file has now begin it's 30 day
quarantine period.

##### Risk

Files that are found to be compromised or infected are labeled "Risk"
and are immediately relocated to the infected directory.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image19.png" style=""></img>
</div>

##### Released

After 30 days has passed, the second virus scan will be performed. If no
further threats are found, the quarantined files status label will
change to "Released".

### Uploading File and Folders into Personal

The upload process into the Personal Workspace is functionally
identical, but note two major differences:

-   Files will be virus scanned once only.

    -   If safe, the file is tagged "Passed".

    -   If compromised, the file is moved to an infected directory.

-   You cannot move files out of the personal workspace.

### Other Upload Methods

You can also get content into Curate using SFTP, webdav and with
physical data transport devices when on-cloud.

### Creating and Using a Deposit Space

Curate allows you to share any file, folder or other area (see *Sharing
files or folders* for more detail). By allowing users of a shared area
upload permissions, you can easily create a secure space for your
submitters to deposit their content.

Be sure to create your deposit space in the Quarantine workspace, so
that your deposited files are automatically quarantined. You are also
unable to upload files in to workspaces other than Quarantine and
Personal.

#### Setup

First create and share a folder for your deposit space. This folder is
where your depositors will upload their content. *See sharing a file or
folder.*

Once shared, you can enable "Upload files" under the permissions tab.
You should typically disable download permissions unless you want your
depositors to be able to download content from other depositors.

Under the "Access restrictions" tab, you can choose to set a password
for the space, and even specify an expiry period for the sharing link.
NB: once your sharing link has expired, nothing will happen to your
shared files or folders, the public URL will simply become inaccessible.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image20.png" style=""></img>
</div>

#### Usage

You may then share your deposit URL with your collaborators. They will
be presented with a simple interface into which they can upload their
deposit.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image21.png" style=""></img>
</div>

#### Simple upload interface

You can also choose to give your depositors an ultra-simple "drop files
here" style interface instead. Not only does this simplify the process
of uploading files for your submitters even further, but it also ensures
that they are unable to see any other content that has been uploaded
into the space. To change the deposit space interface, open the "link
label" section in the sharing configuration. Select "Drop Files Here"
for the simple upload interface. *Hint: make sure to save your changes.*

### Creating and Using a Smart Deposit Space

Smart Deposit Spaces allow you to require specific files, formats,
contents, documentation and even metadata from your depositors. You can
even leave them personalized messages upon submission, or chain
additional actions in your workflow.

Just like other Deposit spaces, make sure to create it in your
Quarantine workspace. You are unable to upload files into other
workspaces, and it will ensure that all your deposits are automatically
quarantined.

To create a Smart Deposit Space, first create a deposit space (see
creating and using a deposit space). Then, open your new deposit space
and right click in the empty space. You should then select the "Smart
Form" option.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image22.png" style=""></img>
</div>

The Smart Form builder will allow you to select what file formats you
require in your deposits in the "Expected Files" section. This will also
allow you to describe the required files, add authorized extensions and
size limitations.

You can then define what other information or metadata you require in
the "Submission Form" section.

Follow on actions and submission messages can be configured in the
"Legends and Completion" section.

In the "Creating and Using a Deposit Space" section, you can find more
information about the configuration options for your shared space,
including password protection, file visibility, access restrictions and
more.

Once you have created your Smart Deposit Space, you can save it and
disseminate the URL. Users accessing the link will be presented with a
form requesting the information you have described. Their uploads will
be rejected without any processing if the requirements are not met. The
users are unable to submit their deposit until they have completed all
your mandatory requirements.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image23.png" style=""></img>
</div>

## Appraisal, selection and arrangement

### Move Content into Appraisal

Files will be moved into the Appraisal workspace when they have
completed quarantine and two successful virus scans. Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> is not
prescriptive however and you can move data early. The Appraisal
workspace is used to create arrangements (folder structures containing
your files), conduct content appraisal helped by the file information
available and to create descriptions.

Try moving files and folders from the Quarantine workspace into
Appraisal. You can do this by selecting, right clicking and selecting
Move or by dragging and dropping to a different workspace in the listing
in the lefthand column. Multiple files or folders can be selected for
each move using the usual Control or Shift operations.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image24.png" style=""></img>
</div>

Note that if files are moved into Appraisal early (i.e. before the
quarantine period is up) then the Quarantine Status tag changes to Risk
to indicate that full quarantine conditions were not met.

Once you have files in the Appraisal workspace, Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> runs
comprehensive file characterisation programmes. To access the generated
characterization information, select a file and check the file
information panel in the object information area. (*see File Information
Panel*). Characterised objects will include these fields in their
information area:

-   File MIME type

-   PRONOM ID

In Appraisal you can try creating folders ('New/New Folder') and moving
files between folders to create an arrangement.

You can also move, copy, rename, delete, lock and bookmark files with
right mouse click functions. Certain media and text files can be
viewed/rendered by double clicking the file.

The Compress option allows you to create a compressed package of a
folder in .zip, .tar or .tar.gz format. The original folder is retained
when you do this. You can use this to compress your archive packages, or
for any other general utility purpose.

Note that you can also move files from Quarantine into Personal, but you
will not be able to move them back out!

### Creating Descriptive Records

While you can begin to describe your files and folders from the moment
they are uploaded to Curate, many users choose to wait until the objects
have completed their Quarantine period successfully and have been
characterized in the appraisal space. This approach gives you the most
complete understanding of the object before describing it, it also
ensures you do not spend time describing files that have been deemed
unsafe.

Note that any description you apply to files in their quarantine period
will be retained, all metadata is retained with a file no matter where
it goes in the system.

#### Describing a Single File or Folder

Descriptive metadata is used to annotate a file, folder or group of
files in a folder structure. All descriptive metadata in Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> is
indexed and searchable (*see search*). Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> provides both the
Dublin Core simple 15 element schema which you can read about in detail
(if you want to) at:
<https://www.dublincore.org/specifications/dublin-core/dcmi-terms/#section-3>
and the full General International Standard Archival Description ISAD(G)
descriptive metadata schema which you can read more about at:
https://www.ica.org/en/isadg-general-international-standard-archival-description-second-edition.

You can be as precise as you wish with the use of metadata elements by
following the specifications and controlled vocabularies. Alternatively,
you can just use those elements you wish, in the way that suits you,
(for example by putting a title in for each file). Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> does not
impose rules.

To begin to describe any file or folder in Curate, select the object you
would like to describe. On the right hand side of your screen, in the
object information area, you will see the file metadata panel. (*see
object information area, metadata panel*).

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image25.png" style=""></img>
</div>

Next, click the dropdown for your chosen
record schema. Curate features simple DC and ISAD(G) out of the box, but
can easily support most any other standardized schema.

Enter the metadata for each field you would like to modify, and you will
then see the "save" button appear at the bottom of the panel.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image26.png" style=""></img>
</div>

Note that the save button will appear as
soon as any changes are made to the selected files descriptive metadata.
If you select another file before saving or without reverting your
changes, the changes will move to the next selected file and await you
to "save" again.

#### Batch Describing Files and Folders

To describe multiple files and or folders at once, first select all the
objects you would like to create or modify descriptive records for.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image27.png" style=""></img>
</div>

In the object information area, you will see only the file actions panel
(*see file actions panel*) which will contain options to download the
multiple selection of objects, or "meta data" to modify the descriptive
records of all the files.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image28.png" style=""></img>
</div>

You can also right click any of the
objects in your selection, and you will see the "meta data" option in
the context menu.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image29.png" style=""></img>
</div>

You will then be prompted to select the
fields that you would like to modify.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image30.png" style=""></img>
</div>

As you tick each field you would like to
modify, a text area will appear in which to enter your new data.

Once you've modified all your chosen fields, click "ok" and all the
files in your selection will be updated.

### Creating a Report on File Types

Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> identifies file types via a MIME type and a PRONOM ID. You
can generate detailed reports of the MIME types, for example to create a
digital asset register, for any aggregation of files or folders. Try
going to a high-level folder that contains other folders and files,
click New and select 'Generate MIME type Report'. A popup will appear
with a pie chart showing the filetypes in your selection. You can float
over the chart to see the numbers. You can also download the MIME type
report as a CSV file.

<div class="main-content-img-container">
    <img src="/vertopal_205d29a8e99241c0a1d0e3064ad58f44/media/image31.png" style=""></img>
</div>

### Creating a Transfer Package or SIP

Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> can create packages or SIPs for submission to repositories or
digital preservation platforms such as: Archivematica, Preservica and
EARK compliant systems using the templates in the Package Templates
workspace. We can give you a demonstration of package creation if you
are interested, just send us a message via the support channel.

## Miscellaneous

### Bookmarking a File or Folder

Any file or folder can be bookmarked by selecting and choosing the
option in the right mouse click or More menus. Bookmarked files and
folders appear in the Bookmark listing which you can access via the Star
icon at the top of the left-hand column. The Bookmark listing gives you
quick access to files you may be working with.

The option to make a 'New Folder from Bookmarks' is a feature that
allows you to copy an existing folder which has been bookmarked. Using this you can
create templates for commonly used folder structures, including the files within them, and replicate them by creating a new folder from
the bookmark.

### File Locking

You can choose to lock any file or folder in Curate to prevent
modification by any other user.

For files, this will prevent direct modification of the files content.
For folders, it will prevent any modification to the contents of the
folder itself.

This option does not prevent modification to the metadata of the locked
object.

Locked files will have a icon in the file list to indicate that they are
locked.

### Compress

Any file or folder can be compressed from the right click or More menus.
Options are given for Zip, Tar or Tar.gz packages and the compressed
object is added as an additional item in the same folder.

## Search and Access

### Creating a Link

You can create a public or secure, private link for any file or folder
in your account. When clocking the link, guest users can view, download,
view metadata and even upload content. Start by selecting Share by
either right clicking on a file or folder or from the top

### Searching for Files

You can do simple searches across all of Curate <span style="font-size: 8pt;vertical-align: super;">TM</span> using the search box
at the top right of the screen. The simple search is conducted over file
names and folder names only (not metadata). Complete names or fragments
of filenames can be used, for example a file called myphotograph.jpg can
be found searching on: myphotograph.jpg, myphotograph, my, photograph or
even photo.

If you click in the simple search box you will see a filter icon to the
right, which opens the Advanced Search dialogue. Within this area you
can specifically search in filename, in any of the descriptive metadata
fields and basic file properties. Within the Advanced Search you can
also use the wildcard \* character to enter partial terms, such as
myphoto\*.

menu. You will get a new popup box and can select Enable Public Share
form here. You will now see a url that has been created and is unique
for your share. You can copy this using the Copy icon and you can send
it to anyone you wish. Other options in the Shares popup are:

-   You can send the link to another use in your group using the Send
    Invitation button

-   You can customise the last 12 digits of the link to be anything you
    want and so can make the link meaningful

-   Disable link

-   Change permissions:

    -   For files, by default invited users can download and preview
        content, but you can disable either of these options.

    -   For folders, an option is added to give permission to upload
        files into your folder

-   Access Restrictions: you can add a password and password expiry date
    to the link to make it private

-   Link Label: when the object is viewed from the link it will have a
    label on the top of the page, this is normally the file or folder
    name, but you can customise it here together with the link
    description which is normally the created date and the presentation
    of the link contents. By default the user is presented with a
    preview of the file (if enabled) or a big download button (if
    preview is disabled), but you can make the download button the
    default.

-   \[Advanced Visibility\]: by default the link can only be edited by
    you, but if you enable this option you can allow other users within
    your group to edit the link.

All of your shares can be viewed and edited by selecting the My Shares
option in the menu under your username.

# Support

If you need help, click the pull-down menu at the top left of the
window, which should be labelled with a truncated version of your user
ID and select Support. This will take you to a contact form which goes
directly to the Penwern support team.

# Suggestions

Curate is a very flexible platform on which it is relatively easy for us
to add functionality over time. We have a lot of ideas already and will
put a list up on the website soon. However, we would really like to know
your needs for new functions so that we can prioritise. Please drop us a
line and also indicate if we can contact you in case we have questions.

[^1]: ar Future functionality, expected mid 2023