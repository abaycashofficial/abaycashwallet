#**1. Clone wallet sources**

```
git clone https://github.com/cryptonotefoundation/abaycashwallet.git
```

**2. Modify `CryptoNoteWallet.cmake`**
 
```
set(CN_PROJECT_NAME "abaycash")
set(CN_CURRENCY_DISPLAY_NAME "AbayCASH")
set(CN_CURRENCY_TICKER "ACH")
```

**3. Set symbolic link to coin sources at the same level as `src`. For example:**

```
ln -s ../abaycash cryptonote
```

Alternative way is to create git submodule:

```
git submodule add https://github.com/abaycashofficial/abaycash.git cryptonote
```

Replace URL with git remote repository of your coin.

**4. Build**

```
mkdir build && cd build && cmake .. && make
```
