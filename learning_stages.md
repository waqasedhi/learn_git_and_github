# Git and GitHub learning steps and command cheat sheet
## Introduction
#### What is version control?
Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later.

#### Local version control system
While simply copying files into different directories is a common version-control method, it's prone to errors and accidental overwrites. To address this, programmers created local VCSs (version control systems) that store file changes in a database for better management. RCS is a popular local VCS that stores file changes as patches, allowing for file reconstruction at any point in time.

#### Centralized Version Control Systems
CVCSs address the collaboration issue by storing all files in a central server. This offers control and visibility, but comes with risks:

* Single point of failure: Server downtime prevents work and potential data loss.
* Data loss threat: Corrupted server disk or improper backups can erase project history.
* Similar to local VCSs: Both risk losing everything if the history is kept in one place.

While CVCSs provide advantages, their central server dependency creates significant vulnerabilities.

#### Distributed Version Control Systems (DVCSs):

DVCSs offer enhanced resilience and flexibility compared to CVCSs:

*    Full Repository Mirroring: Clients don't just retrieve latest snapshots, they store the entire repository history, ensuring backups.
*    Resilient to Server Failure: Any client repository can restore a lost server, preventing data loss.
*    Multiple Remote Repositories: Supports collaboration with different groups and workflows simultaneously, enabling diverse project structures.

DVCSs address the vulnerabilities of centralized systems by distributing data and enabling multiple collaboration paths.

#### What is Git?
**Git is a Distributed Version Control System (DVCS) that stands out for its unique approach to data storage and management.**

**Key points:**

- **Distinctive Approach:** Git's way of storing and managing information differs significantly from other VCSs like CVS, Subversion, or Perforce.
- **Clear Understanding Required:** Grasping Git's fundamentals will significantly ease its effective use.
- **Unlearning Previous Assumptions:** Setting aside knowledge of other VCSs is crucial to avoid confusion, as Git's distinct approach might lead to misunderstandings if viewed through the lens of other systems.
- **UI Similarities, Conceptual Differences:** While Git's user interface shares resemblances with other VCSs, its underlying concepts and data handling are unique.

**Understanding Git's unique approach is essential for smooth and effective use.**


## Installation step:

if you are new user we to install git bash for windows, and for mac user first we have to install and find terminal then install git,

### 1. Instalation Guide:
Download git installer for windows or mac or linux from this [link](https://git-scm.com/downloads),

Here's an expanded guide for installing Git on different Linux distributions:

##### A. Universal Method:

* After download the source code: Visit the Git download page at this [link](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and choose the desired version. Download the source tarball (.tar.gz) file.

* Extract the source code: Open a terminal in your preferred location and use tar -xf <filename>.tar.gz to extract the downloaded file.

* Configure and build Git: Navigate to the extracted directory and run ./configure. This checks your system for necessary dependencies. Install any missing dependencies via your package manager. Then, run make to build Git.

* Install Git: Execute sudo make install to install Git system-wide. This requires administrator privileges.

##### B. Distro-Specific Methods:

* Debian/Ubuntu: Use the package manager with 
```sudo apt install git```
* Fedora/CentOS: Use the package manager with 
```sudo dnf install git```
* Arch Linux: Install Git from the official repository with 
```sudo pacman -S git```
* OpenSUSE: Use the package manager with 
```sudo zypper install git```
* Gentoo Linux: Install Git from the Gentoo portage with 
```sudo emerge dev-vcs/git```


### 2. Verify Installation:

Once the installation completes or to check git in any pc or laptop, confirm it by checking the Git version ```git --version``` or only use command ```git```



## Start a working area (see also: git help tutorial)

### Local area

1. make a folder in your hard drive locally

2. go to that folder via command prompt or terminal
```git
cd <pathtofolder>
```

3. initialize git repository
```
git init
```

### Remote area clone

1. Copy the project from the remote repository

```
$ git clone [repository_path]
```


5. add changes to the stage changes in single file.

```
git add <path_to_file>
```
or, use this command to stage all changes at once in multiple files.
```
git add .
```

6. commit the changes if you are done with changes: 
(note: always write massage because it will help in tracking your commits history in future.)
```
git commit -m "yourmessage"
```

7. to sync changes use this:
```
git push <remote name> <branch name>
```
note:(defualt remote name is "origin" and also use as best practice too. and defualt branch name is "master" in git and "main" in github.
both remote and branch names can be change as per need.) 