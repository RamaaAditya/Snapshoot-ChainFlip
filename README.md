# Snapshoot-ChainFlip
Tutorial Faster to Syncronize To Latest Block

# Introduction
Big Very Thanks You Very Much For ChainFlip Team For Give me a Chance Explore in the ChainFlip COmmunity
And Here I Want To Share out about How To Faster Sync In ChainFlip


ChainFlip Data
```
Total Block : 1433924
Size Of Data 15Gb++
```
Note : Make Sure if u have stoped ur node first 
# sudo systemctl stop chainflip-node

# Step 1 
``` 
git clone ....

```

# Step 2
Make Sure You Have Remode db folder you have create before
``` 
cd /etc/chainflip/chaindata/chains/Chainflip-Perseverance/
sudo rm -rf db
cd
```

# Step 3
Empety The Old Logs and Recreate New Logs 
``` cd /var/log/chainflip-engine.log
sudo rm -rf chainflip-engine.log
sudo cat chainflip-engine.log
cd
```


# Step 3 
Extract database file of chainflip
``` 
tar -xvzf chainflip.tar.gz 
```

# Step 4
copy db file to folder Chainflip-Perseverance
```
cp -r db /etc/chainflip/chaindata/chains/Chainflip-Perseverance/
```

# Step 5
Start The ChainFlip Node
```
sudo systemctl start chainflip-node
```
Check The Logs
-> tail -f /var/log/chainflip-node.log
