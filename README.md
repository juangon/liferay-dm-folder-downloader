# Liferay Documents and Media Folder Downloader

*liferay-dm-folder-downloader*

This project provides a Liferay Portal plugin to download the contents of a Documents and Media folder (and subfolders) as a ZIP file.


## Supported Products

* Liferay Portal 6.2 CE GA1 (6.2.0+)
* Liferay Portal 6.2 EE GA1 (6.2.10+)


## Downloads

The latest release is available from [SourceForge - Documents and Media Downloader](https://sourceforge.net/projects/permeance-apps/files/liferay-documents-and-media-downloader/ "Documents and Media Downloader").

You can also download or install the hook from [Liferay Marketplace - Documents and Media Downloader](https://www.liferay.com/marketplace/-/mp/application/21674918?_7_WAR_osbportlet_backURL=%2Fmarketplace%2F-%2Fmp%2Fcategory%2F11232561 "Documents and Media Downloader")


## Usage

Step 1. Navigate to Liferay Portal page containing Documents and Media portlet.

![Documents and Media Portlet](/docs/images/01-liferay-dm-portlet-local-repos-root-folder-view-20130209-annot.png "Documents an Media Portlet")

Step 2. Click on the "Action" button for a folder and select the "Download Folder (ZIP)" menu item.

![Documents and Media Folder Action Menu](/docs/images/02-liferay-dm-portlet-download-folder-action-menu-20130131-annot.png "Documents an Media Folder Action Menu")

Step 3. Open ZIP file or save to local download folder in your web browser.

![Firefox Download File Dialog](/docs/images/03-firefox-download-file-dialog-20130209.png "Firefox Download File Dialog")


## Building

Step 1. Checkout source from GitHub project

    % md work
    % cd work
    % md -p liferay-dm-folder-downloader/branches/6.2.x
    % cd liferay-dm-folder-downloader/branches/6.2.x
    % git clone https://github.com/permeance/liferay-dm-folder-downloader
    Cloning into 'liferay-dm-folder-downloader'...
    remote: Counting objects: 475, done.
    remote: Compressing objects: 100% (199/199), done.
    remote: Total 475 (delta 151), reused 470 (delta 146)
    Receiving objects: 100% (475/475), 618.21 KiB | 161.00 KiB/s, done.
    Resolving deltas: 100% (151/151), done.
    Checking connectivity... done
    % cd liferay-dm-folder-downloader
    % git branch 6.2.x
    % git checkout 6.2.x
    Switched to branch '6.2.x'
    % git status
    # On branch 6.2.x
    nothing to commit, working directory clean

Step 2. Build and package

    % mvn -U clean package

This will build "liferay-dm-folder-download-hook-A.B.C.war" in the targets tolder.

NOTE: You will require JDK 1.6+ and Maven 3.


## Installation

### Liferay Portal + Apache Tomcat Bundle

eg.

Deploy "liferay-dm-folder-download-hook-A.B.C.war" to "LIFERAY_HOME/deploy" folder.


## Project Team

* Tim Telcik - tim.telcik@permeance.com.au
* Chun Ho - chun.ho@permeance.com.au


## Related Projects

* [GitHub - Sample Liferay Documents and Media Action Menu Extension](https://github.com/permeance/sample-liferay-dm-action-menu-extension "GitHub - Sample Liferay Documents and Media Action Menu Extension")
