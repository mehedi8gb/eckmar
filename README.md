# Eckmar, also known as Eckmar's Marketplace Script

Cryptocurrency-friendly marketplace on Laravel.

![](https://github.com/nomiac-mobile/peralta/blob/master/demo/1.png)

# Features
**Vendor Accounts**

Any user can register and buy products on the marketplace but in order to create a listing you need to have vendor account status. Vendor status can be obtained in two ways. You can apply and get it for free after admin reviews your request or you can pay for it (the amount is set in admin panel).

**Autofill**

Autofill system is created for users that sell many items (cd-keys for example). They can populate field where each line represents one item to be sold. In the case that product is autofilled delivery state is skipped when user purchases a product and he gets what is on the first line automatically.

**Messaging System**

Users can send private messages to each other.

Mnemonic Password ResetWhen an user registers, he receives an unique mnemonic that can be used to reset the password.

**Wallet System**

When an user wants to deposit new deposit address will be generated for him every time (deposits on old addresses generated by user will still be valid). Current system in place is that user have to click check balance button in order for system to check if he has any balance to be added on his account (Please note that this system can be changed so server will auto-check every minute but this may be intensive task to run every minute if you got a lot of users).

**Escrow**

When user purchase any item there is a fee (that can be configured) and automated escrow. In case the seller did not delivered goods or goods are not what they are supposed to be, buyer can open a dispute. Both users and the admin have access to dispute discussion (you will see example where one of the users is in fact the admin so he can reply as disputed party or admin).

**Feedback**

There are two parts in this system. Feedback score and trust rating. Feedback score is basically percentage of positive feedback and Trust rating can be Very Low, Low, Average or High (Unproven if the user has less then five feedbacks).

**News**

Basically a blog that will appear on the first page. You can use it in case you want to inform your users.

**Auction System**

Products can be sold normally or as auction. You can specify end date, minimum bid and buyout prices. After that process is automatic. The system will automatically update the minimum bid (in case users actually bid on product of course) and when time reaches end date of an auction and no one bought it (buyout) user with largest bid will be the auction winner and all other users will be refunded.

**Admin Panel**

In the admin panel you can create categories, respond to vendor applications, disputes or create news.

# [Installation](https://github.com/nomiac-mobile/peralta/blob/master/INSTALLATION.md)

# Server requirements
```
VPS with at least 256MB of RAM
Daemon for each coin that is enabled on marketplace
```
# Software Requirements
```
PHP7 (7.2 recommended)
SQL Database (MySQL,PostgreSQL, SQLite, SQL Server)
Elasticsearch (Search interface that will keep track of search records and provide great search performance)
Redis (Optional, but will greatly increase app performance)
```
