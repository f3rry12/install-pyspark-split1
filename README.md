# Install PySpark in pythonanywhere
Because free user [pythonanywhere](https://www.pythonanywhere.com) have limited space.
So its bit tricky to install PySpark to pythonanywhere. <br>
In this repository i will tell you how to install PySpark in pythonanywhere step by step. <br>
I use PySpark Version 3.1.2 in this repository <br>
Reminder: not every Machine Learning project use Spark, so install it if you need it <br>
![about](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/spark.jpg)
 
## Installation
### Prerequisites
What you need to prepare:
* Have already make web app [pythonanywhere](https://www.pythonanywhere.com)
* Make sure you still have plenty free space
here my scrrenshot of my web app environtment <br>
![webenvirontment](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/pre.jpg)
  
### Install PySpark
1. Go to Files section, then create new directory named spark-3.1.2-bin-hadoop3.2 <br>
![ss1](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss1.jpg)

2. Back to main directories, then create new directory named tar <br>  
![ss2](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss2.jpg)

3. Open new tab, go to Consoles section, and open bash <br>
![ss3](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss3.jpg)

4. Clone this repo into your tar directories by following this command
   ```sh
   git clone https://github.com/f3rry12/install-pyspark-split1.git /home/yourusername/tar/
   ```
![ss4](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss4.jpg)

5. Untar the file to spark directories
   ```sh
   tar -xf /home/yourusername/tar/split1.tar -C /home/yourusername/spark-3.1.2-bin-hadoop3.2
   ```
![ss5](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss5.jpg)

6. Go to tar directory, clear some storage space by deleting all file in this tar directory (refresh tab to make sure it deleted)
![ss6](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss6.jpg)

7.Go to spark-3.1.2-bin-hadoop3.2directory then create new directory named jars
![ss7](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss7.jpg)

8.Clone my other repo into your tar directories by following this command
   ```sh
   git clone https://github.com/f3rry12/install-pyspark-split2.git /home/yourusername/tar/
   ```
![ss8](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss8.jpg)

9. Untar the file to jars directories <br>
 ```sh
   tar -xf /home/yourusername/tar/jars_a_i.tar -C /home/yourusername/spark-3.1.2-bin-hadoop3.2/jars
   ```
![ss9](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss9.jpg)   

10. Go to tar directory, clear some storage space by deleting all file in this tar directory (refresh tab to make sure it deleted)
![ss10](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss10.jpg) 

11. Clone the other repo into your tar directories by following this command
   ```sh
   git clone https://github.com/f3rry12/install-pyspark-split3.git /home/yourusername/tar/
   ```
![ss11](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss11.jpg) 

12. Untar the file to jars directories <br>
 ```sh
   tar -xf /home/yourusername/tar/jars_j_r.tar -C /home/yourusername/spark-3.1.2-bin-hadoop3.2/jars
   ```
![ss12](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss12.jpg) 

13. Go to tar directory, clear some storage space by deleting all file in this tar directory (refresh tab to make sure it deleted)
![ss13](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss13.jpg) 

14. Clone the other repo into your tar directories by following this command
   ```sh
   git clone https://github.com/f3rry12/install-pyspark-split4.git /home/yourusername/tar/
   ```
![ss14](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss14.jpg) 

15. Untar the file to jars directories <br>
 ```sh
   tar -xf /home/yourusername/tar/jars_s_z.tar -C /home/yourusername/spark-3.1.2-bin-hadoop3.2/jars
   ```
![ss15](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss15.jpg) 

16. Go to main directory, and delete tar directory to clear some storage space
![ss16](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss16.jpg) 

### Set Up PySpark Environment
1. Install findspark module
 ```sh
   pip3.7 install --user findspark
   ```
![ss17](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss17.jpg) 

2. Download bashrc from my other repo with console by followng this comand
 ```sh
   wget https://raw.githubusercontent.com/f3rry12/EasyDeployFlask/main/.bashrc
   ```
![ss18](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss18.jpg) 

3. Go to main directory, edit bashrc (it depend on your bashrc name, in my case i download it with name bashrc.1)
![ss19](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss19.jpg) 
![ss20](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss20.jpg) 
Dont forget to save file after edit it

4. Run this command (it depend on your bashrc name, in my case i download it with name bashrc.1)
 ```sh
   source ~/.bashrc.1
   ```
5. Run pyspark to check if it success <br>
 ```sh
   pyspark
   ```
![ss21](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss21.jpg) 

### Connect PySpark Environment to your .py
1. Download findspark.py from my other repo https://raw.githubusercontent.com/f3rry12/EasyDeployFlask/main/findspark.py
   Then upload it to your main web directory
   (you can skip this if you follow my repo [EasyDeployFlask](https://github.com/f3rry12/EasyDeployFlask) because this repo include this file)
![ss22](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss22.jpg) 

2. Edit findspark.py <br>
![ss23](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss23.jpg) 

3. Make sure to import findspark in.py file if you use spark <br>
![ss24](https://github.com/f3rry12/install-pyspark-split1/blob/main/readMeAsset/ss24.jpg) 

## Acknowledgements
Special thanks to my Instructur [Imam Cholissodin](https://github.com/imamcs19), S.Si., M.Kom. <br>
Thanks to my friend [Hanifa](https://github.com/H4nifa) for helping me to upload this file with my limited internet <br>
