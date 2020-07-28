# blockproject


Bitcoin, Ripple, Bitcoin Cash, Litecoin, Monero, and EOS all primarily use C++ to write the core blockchain.

EOS notably also uses C++ for their smart contracts, which compile to WebAssembly.

Ethereum is written in Go, and their smart contracts are written in Solidity.

NEO uses C#. Their smart contracts can currently be written in C#, F#, Java, Kotlin, and Python currently, with more options on the way.

Cardano is written in Haskell, and soon their smart contracts will be able to be written in any language.

Stellar is written in C++.

Topl uses Scala for our blockchain, and JavaScript for our smart contracts.

It appears C++ is currently leading the way for blockchain development. This is not the truth. Solidity is the real leader for now. Extending beyond the top ten, we see 91% of the market share actually rests in ERC20 tokens written in Solidity on the Ethereum platform. We’re even using Solidity at Topl to implement side-chaining to bring Ether onto our platform.

The fact of the matter is, you will most likely need to know multiple programming languages to excel in this space. The space is small but growing, and most crypto businesses are still in the startup stages. This means wearing many hats, and performing a variety of tasks.

Solidity is, well, a solid place to start if you are looking to gain experience. To get your feet wet, try writing basic smart contracts and generally interacting with a working blockchain to learn its quirks and behaviors.

We specifically look for and are looking for people that have worked on varied projects and can switch between languages effectively. Our developers mainly work with JavaScript and Scala, and should be able to use both. More importantly, they have built things before coming to work for us.

Building Things
Basic projects, little widgets, full fledged businesses. We want to see them all. This is especially true when it comes to blockchain because there are not many things to build yet. So roll out your own blockchain following a guide in Python or C++. Write some Solidity contracts. That experience will be immensely helpful. There isn’t really room to get too crazy with your projects yet though. That’s fine, most people realize that.

At Topl, we aren’t searching for overly experienced talent. What does 5+ years of blockchain experience even look like? The space is new enough that we can up-skill people quickly, as long as they have some knowledge and plenty of drive.

Things are changing quickly in this space, especially the technologies behind it. This is why it’s increasingly important to have malleable programmers who can change quickly with each paradigm shift. Like with web programming, there’s a new way to do things practically every month.




These are instructions for running MoneyPot locally on a Mac using homebrew.

Install homebrew packages
brew install git node npm postgresql
Getting the sources
cd moneypot
Create a database user and setup the tables
Create a user. It will prompt you for a password.

createuser -P moneypot
Create the database and setup the tables. The second command will prompt you for the password again.

createdb -O moneypot moneypotdb
psql -W -U moneypot -d moneypotdb -h localhost -f server/schema.sql
Configuration
Installing node.js dependencies locally.
This will download and install all dependencies in the node_modules subdirectory.

now start test

npm install
Database
Export the database link as an environment variable

export DATABASE_URL=postgres://moneypot:<YOURPASSWORD>@localhost/moneypotdb

export DATABASE_URL=[@"host:"xhttp://89.44.9.118/main/", port: 8080"];
export DATABASE_URL=[@"host:"xhttp://89.44.9.118/main/", port: 8080"];
export DATABASE_URL=[@"host:"xhttp://89.44.9.118/main/", port: 8080"];
BIP32 Key
You will need to create a BIP32 key pair. You can do at your own risk online at bip32.org. Export the public key as an environment variable

export BIP32_DERIVED_KEY=xpub6AH.....
