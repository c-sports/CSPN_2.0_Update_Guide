# CSPN Wallet 2.0 Update Guide

## Backing up your wallet.dat:

1. Open up your CSPN 1.0 wallet.

2. Go to **File->Backup Wallet**.

3. Choose a destination and save the file as **wallet.dat**.

**Tip: Back up your wallet frequently and keep the backup on an external storage device.**

***

## Installing and setting up the new CSPN 2.0 wallet

1. Download the CSPN 2.0 wallet for your operating system from **https://github.com/c-sports/CSPN/releases**.

2. Start the wallet, follow the wizard and then close it again.

3. Now we need to navigate to the CSPN 2.0 data folder which you will find here by default:

**Windows**

```
C:\Users\Username\AppData\Roaming\CSPN\wallets
```

Tip: You can quick navigate to the folder by pasting **%APPDATA%\CSPN\wallets** into the windows explorer navigation bar.

**MAC**

```
/Users/Username/Library/Application Support/CSPN
```

Tip: You can quick navigate to the folder by opening **Finder**, clicking on **Go -> Go to Folder** and pasting **~/Library/Application Support/CSPN**.

**Linux**

```
/home/username/.cspn
```

Tip: You can quick navigate to the folder by opening **File Explorer**, clicking on **Go -> Enter Location** and pasting **~/.cspn**.

4. Copy & paste your backed up CSPN 1.0 wallet.dat into the CSPN 2.0 data folder and override the existing file.

5. Now open up your CSPN 2.0 wallet. Your balances should be there.

Done.

## Temporary POS Display Bug Fix

When staking an orphaned block it happens that the staked coins are not being released automatically which looks like your balance decreased. Of course, this is not the case and just a display bug. As a temporary fix please add the following line to your **cspn.conf** file (which you will find in the data folder of the wallet) and save it:

```zapwallettxes=1```

Now whenever you realize that your balance seem to have decreased just restart your wallet and your balance should be correct again.
