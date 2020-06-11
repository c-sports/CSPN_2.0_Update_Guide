# CSPN Wallet 2.0 Update Guide

## Backing up your wallet.dat:

1. Open up your CSPN 1.0 wallet.

2. Go to **File->Backup Wallet**.

3. Choose a destination and save the file as **wallet.dat**.

**Tip: Back up your wallet frequently and keep it on an external storage device.**

***

## Installing and setting up the new CSPN 2.0 wallet

1. Download the CSPN 2.0 wallet for your operating system from **https://github.com/c-sports/CSPN/releases**.

2. Start the wallet, follow the wizard and then close it again.

3. Now we need to navigate to the CSPN 2.0 data folder which you will find here:

**Windows**

```
C:\Users\Username\AppData\Roaming\CSPN
```

Tip: It is easier to locate the folder when you have the displaying of hidden files activated (search in google for: show hidden files in windows [your version]).

**MAC**

```
/Users/Username/Library/Application Support/CSPN
```

Tip: It is easier to locate the folder when you have the displaying of hidden files activated. To show hidden files on MAC OS X open up the terminal and type:

```
defaults write com.apple.finder AppleShowAllFiles YES (NO to deactivate again)
killall Finder
```

4. Copy & paste your backed up CSPN 1.0 wallet.dat into the CSPN 2.0 data folder and override the existing file.

5. Now open up your CSPN 2.0 wallet. Your balances should be there.
