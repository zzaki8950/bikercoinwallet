**Warning: Non-Latin users**

If you are using windows non-Latin language you need to force bikercoinwallet.exe to start in a Latin characters directory.

The usual location C:\Users\{username}\AppData\Roaming\bikercoin will not be able to create a wallet at this location on a non-Latin characters username.

(e.g. C:\bicblockchain - Not C:\БИКblockchain)

start with (bikercoinwallet.exe --data-dir C:\bicblockchain)

You have to understand that this program is a BETA release. (Use all Bikercoin software programs, apps, miners, exchanges at your own risk)


**1. Clone wallet sources**

```
git clone https://github.com/scriptexpert/bikercoinwallet.git
```


**2. Set symbolic link to coin sources at the same level as `src`. For example:**

```
ln -s ../bikercoin cryptonote
```

Alternative way is to create git submodule:

```
git submodule add https://github.com/scriptexpert/bikercoin.git cryptonote
```

**3. Build**

```
mkdir build
cd build
cmake -G "Visual Studio 12 Win64" ..

```
**And then do Build.**
