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
