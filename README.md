# magento2-search-fix
Magento2 module for fixing hanging "insert to" search_tmp queries

# Installation
## via composer
Run the following command in Magento2 root folder:
```
composer require we-are-virtua/magento2-search-fix
php bin/magento setup:upgrade
php bin/magento setup:di:compile
```

#FAQ
- Module does not help, what to do?

If the module does not help it means that rewrites may not work. 
You can try to remove `generated/code` directory manually and re-run 
```
php bin/magento setup:upgrade
php bin/magento setup:di:compile
```