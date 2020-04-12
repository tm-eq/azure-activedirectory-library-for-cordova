#Instructions to re-build *ADAL.framework*

1. Clone or download [azure-activedirectory-library-for-objc](https://github.com/AzureAD/azure-activedirectory-library-for-objc)
2. Navigate to `azure-activedirectory-library-for-objc`and open *ADAL.xcworkspace* in *Xcode*
3. In settings change *ADAL iOS* -> *Mach-O Type* build setting from *Dynamic Library* to *Static Library*
![ADAL Static Library](http://i.stack.imgur.com/6yKzU.png)
4. Copy `azure-activedirectory-library-for-cordova/src/ios/tools/build_sdk.sh` to `azure-activedirectory-library-for-objc` root and run. You may need to [make the file executable](https://support.apple.com/en-gb/guide/terminal/apdd100908f-06b3-4e63-8a87-32e71241bab4/mac) before it can be run.
5. Upon successful execution updated version of *ADAL.framework* will be available in `azure-activedirectory-library-for-objc/build` folder.
