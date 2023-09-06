<img src="assets/logo.jpg" alt="logo" width="auto" height="auto" />
  <h1>High Performance Computing Course - 2022</h1>
</div>
<br />

<!-- Table of Contents -->
<br/><br/>

# **Table of Contents**

- [About this Project](#about-this-project)
  * [Course Overview](#course-overview)
  * [What are HPC's](#what-are-hpc's)
  * [Motivation](#motivation)
  * [Course Schedule](#course-schedule)
- [GitHub Intro](#github-intro)
  * [Markdown Basics](#markdown-basics)
- [Introduction to MAC](#introduction-to-mac)
- [Introduction to Linux](#introduction-to-linux)
  * [Navigation](#navigation)
    * `pwd`
    * `cd`
    * `ls`
  * [Folder & File Management](#folder-&-file-management)
    * `mkdir`
    * `touch`
    * `cp`
    * `mv`
    * `rm`
  * [File Content Management](#file-content-management)
    * `echo`
    * `head`
    * `tail`
    * `less`
    * `sort`
    * `cat`
    * `cut`
    * `uniq`
    * `grep`
    * `tr`
    * `wc`
  * [Access Rights Management](#access-rights-management)
- [HPC Remote Access](#hpc-remote-access)
  * [Bits and Bytes](#bits-and-bytes)
  * [Connecting to LETHE Server](#connecting-to-lethe-server)
  * [Working on the Server](#working-on-the-server)
  * [Hashes](#hashes)
  * [SLURM](#slurm)
- [Introduction to Shell Scripting](#introduction-to-shell-scripting)
  * [Basic Scripts](#basic-scripts)
  * [Challenge 1 . Alignment Tool Comparison](#challenge-1-.-alignment-tool-comparison)
  * [Challenge 2 . BacGenStat Project](#challenge-2-.-bacgenstat-project)
  * [Challenge 3 . Taxonomy Project](#challenge-1-.-taxonomy-project)
- [Docker](#docker)
- [License](#license)


---
<br/><br/>


# About this project

Intensive computing processes are becoming increasingly important in all fields of research and including biology. For that, the use of computational clusters or high-performance computing on supercomputers becomes necessary.

This requires experience in use of special interfaces, tools and methods as well as specialist knowledge, e.g. of bioinformatics or statistical modeling.

<br/>

### Course overview

This course deals with the most common supercomputer environment as found in scientific environments.

Navigating and working independently on supercomputers through Linux command lines, managing and transferring data, creating and using containers and virtual machines will become part of our toolset.

<br/>

### What are HPC's

High Performance Computing, HPC, summarizes technologies and processes with which complex computing tasks can be performed with high performance. For high-performance computing, tasks are parallelized and the computing power of multiple systems is aggregated. Typical areas of application are science and research, simulation technology, graphic calculations or business intelligence.

<br/>

### Motivation

**`1. What's your motivation?`**

Working proficiency in the HPC ecosystem. Future work prospects.

**`2. Goal and expectations of this course?`**

My goals are to familiarize myself and acquire working proficiency with the Linux ecosystem and learn how to successfully connect to supercomputers.

**`3. What inspires you mostly in Biology, and how will HPC computing help you?`**

Biology not so much, but deep learning and predictive AI technology fascinates me (the likes of OpenAI or ChatGPT). Connecting to supercomputer and managing graphic less interfaces is a must in such cases.

<br/>

### Course Schedule

| Date | Day | Topic |
|:-:|:-:|:--|
| 29.11.2022 | 1 | - HPC Basics <br /> - Github & Version Control <br /> - Documentation & Markdown |
| 30.11.2022 | 2 | - Linux |
| 01.12.2022 | 3 | - Linux |
| 05.12.2022 | 4 | - Remote Access <br /> - Scripting |
| 06.12.2022 | 5 | - Scripting |
| 07.12.2022 | 6 | - AliScale Project <br /> - HPC Etiquette |
| 14.12.2022 | 7 | - AliScale Project |
| 15.12.2022 | 8 | - BacGenStat Project <br /> - Taxonomy Project |
| 15.12.2022 | 8 | - Taxonomy Project <br /> - Docker |


---
<br/><br/>


<div align="center">
  <img src="assets/github.jpg" alt="logo" width="auto" height="auto" />
</div>


# GitHub Intro

<br/>

[Click Me for the Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

<br/>

| Git Command | Description |
|:-:|:--|
| git init <directory> | - creates empty git repository in a specified directory <br /> - no argument initializes the repository in the current directory |
| git clone <repo> | - clones a repository which is located on <repo> onto local machine |
| git config user.name <name> | - defines author name that is used for all commits in current repo |

<br/>

### Markdown Basics

| Element | Syntax |
|:-:|:--|
| Headings | `# H1 - largest header`<br /> `## H2` - becomes <br /> `### H3` - increasingly smaller|
| Ordered List | `1. first item` <br /> `2. second item` <br /> `3. third item` |
| Unordered List | `- first item` <br /> `- second item` <br /> `- third item` |
| Code block | ``` `code` ``` |
| Horizontal lines | `---` <br /> `___` <br /> `***` |
| Bold | `**bold text**` |
| Italic | `*italicized text*` |
| Strikethrough | `~~The world is flat.~~` |
| Emoji | `:emojishortcode:` |
| Link | - `[I'm an inline-style link](https://www.google.com)` <br /> - `[I'm an inline-style link with title](https://www.google.com "Google's Homepage")` <br /> - `[You can use numbers for reference-style link definitions][1]` <br /> - `Or leave it empty and use the [link text itself].` |


---
<br/><br/>  


<div align="center">
  <img src="assets/apple.png" alt="logo" width="auto" height="auto" />
</div>


# Introduction to MAC

| Shortcut / Command | Description |
|:-:|:--|
| Command-X | Cut the selected item and copy it to the Clipboard |
| Command-C | Copy the selected item to the Clipboard |
| Command-V | Paste the contents of the Clipboard into the current document or app |
| Command-A | Select All items |
| Command-F | Find items in a document or open a find window |
| Command-O | Open the selected item, or open a dialog to select a file to open |
| Command-P | Print the current document |
| Command-S | Save the current document |
| Command-Z | Undo the previous command |
| Option-Command-Esc | Force quit an app |
| [Alt] + N | tilde ~ |
| [Alt] + 5 <br /> [Alt] + 6 | square brackets open [ <br /> square brackets close ] |
| [Shift] + [Alt] + 8 <br /> [Shift] + [Alt] + 9 | curly braces open { <br /> curly braces close } |


---
<br/><br/>


# Introduction to Linux

Linux is a family of open-source Unix-like operating systems (OS) based on the Linux kernel and it was first released in 1991. This software directly manages the systems hardware, resources and it makes the connections between all of the software and physical resources that do the work. It has been ported to more platforms than any other operating system and is accessed through the command line.

Anyone can run, edit and redistribute the source code and as such it has become the largest open source project world wide.

It's a very powerful that we will learn to use in connection with supercomputers.

<br/>

### Navigation

| **Command** | **Description** |
|:-:|:--|
| `$ pwd` | show current working directory |
| `$ cd <directory>` | change to directory |
| `$ cd ..` | go up a directory |
| `$ ls` | list files in current directory |
| `$ ls <parameter>` | `-a` show all files including hidden files <br /> `-r` reverse order <br /> `-t` sort by last modified <br /> `-S` sort by file size <br /> `-1` ne file per line |

<br/>

### Folder & File Management

| **Command** | **Description** |
|:-:|:--|
| `$ mkdir <directory>` | create a directory in current working directory |
| `$ touch <file>` | create empty file in current working directory |
| `$ cp <file1> <file2>` | copy *file1* to *file2* |
| `$ mv <file1> <file2>` | move *file1* to *file2* |
| `$ rm <file1>` | delete *file1* |

<br/>

### File Content Management

| **Command** | **Description** |
|:-:|:--|
| `$ echo` | prints to command line |
| `$ echo $TEST` | prints/outputs value of $TEST variable |
| `$ head <file1>` | show first 10 lines of *file1* |
| `$ head -n 2 *` | prints first two lines of all files in working directory |
| `$ tail <file1>` | show last 10 lines of *file1* |
| `$ less <file1>` | view and paginate *file1* in read only editor screen |
| `$ less <parameter>` | `-i` activates insert mode to start writing to the file <br /> `-S` removes automatic linebreaks for very long sentences and adds option to sidescroll <br /> `-vim` opens in read and write stream <br /> [Esc] exits insert mode/editor <br /> [:qw] quits editor, write overrides and saves <br /> [:q!] quits editor and saves without editing |
| `sort <file1>` | sorts *file1* naturally alphanumerically e.g. words by first letter |
| `sort <parameter>` | `-n` sorts *file1* by numbers <br /> `-r` inverts the output <br /> `-rev` reverses the letter order |
| `$ cat <file1> <file2> > <outputfile>` | Like `less` but without the editor. Prints the entire content and concatenates *file1* and *file2* into an *output file* |
| `$ cut` | used for tabular data |
| `$ cut -f4 <filename>` | gives all data from fourth column |
| `$ cut -f1,4 <filename>` | gives all data from columns 1 and 4 <br /> `-d""` specifies a delimiter |
| `$ uniq` | removes duplicates but only works with adjacent values -> sort first |
| `$ uniq <parameter>` | `-c` counts items and moves data into a pivot table |
| `$ tr` | translates |
| `$ tr "T" "U"` | replaces all t's to U's |
| `$ wc <file1>` | counts the words in *file1* providing number of lines, words and bits <br /> `-l` counts all the lines |
| `$ wc -l *` | counts and provides lines of all files in current working directory |
| `$ grep <pattern> <file>` | searches for a pattern in *file* |
| `$ grep "pattern[a-z]*" <file1>` | square brackets for lookin up a selection, wildcard after that sets number of times |
| `$ grep <parameter>` | `-i` case insensitivesearch <br /> `-r` recursive search <br /> `-v` inverted search <br /> `-o` only show matched part of file |
| `$ sed` | search and replace stream editor |
| `$ sed "s/A/T/g"` | replaces all A's with T's globally |
| `$ sed "s/A[TC]/-/g"` | A followed by T or C is replaced by - |

<br />

### Access Rights Management

We can check access rights of any given folder by using the following command:

` $ ls -l -h   <-- -l listing -h human readable `

Output example:

|:-:|:-:|:-:|:-:|:-:|:-:|
| permissions | user | space | file size | creation date | file name |
| drwxr-xr-x | ru67vuy | ADS\Domänen-Benutzer | 288B | Nov 30 10:13 | unix_course_files |

Permissions can be edited with the `$ chmod` command. `$ chmod 777` adds full access rights to a folder.

<br />
---
<br/><br/>


# HPC Remote Access

Remote access is the ability for an authorized person to access a computer or network from a geographical distance through a network connection via the internet, by connecting hosts through a hard-wired network interface or Wi-Fi network interface or by using a secure software solution like a VPN.

<br/>

### Bits and Bytes

One byte is equivalent to eight bits. A bit is considered to be the smallest unit of data measurement. A bit can be either 0 or 1.

<br/>

### Connecting to our LETHE Server

The easiest method is to connect through our MACs Finder by using the shortcut `command + k`, specifying the host and enter our password.

SSH (secure shell protocol) is a network protocol that allows us to operate a network service securely over an unsecured network via the command line. This is our preferred method.

Windows and Apple products differ in the syntax they use. Below is the syntax used to create an SSH connection to our server via MAC.

`$ ssh -l ru67vuy -p 122 CON-compute1.it1.bio.lmu.de`

We had to provide the following parameters to successfully login:

| **Parameter** | **Description** |
|:-:|:--|
| `$ ssh` | protocol |
| `-l ru67vuy` | our login name (LRZ identifier)|
| `-p 122` | port number |
| `CON-compute1.it1.bio.lmu.de` | host name / IP address of the server |

<br/>

### Working on the Server

We can safely copy files from a source host to a destination host with the `$ scp` command. It uses ssh as a protocol.

`$ scp -p 122 [user@]SRC_HOST:]file1 [user@]DEST_HOST:]file2`

Alternatively `$ rsync` can be used aswell. This is however slower because it builds an index first. You can `$ rsync` twice, once with and once without checksum to be faster and safer.

An example for rsyncing into a server will look as follows:

`$ rsync -avz -e 'ssh -p 122' ./ ru67vuy@CON-compute1.it1.bio.lmu.de://LETHE/COURSES/students/aris-protopapas`

<br/>

### hashes

Copying and Transferring files can present a source problems and security risks. In order for us to check if two copies are the same, or if a copy of your file has been changed we can use the help of hashes.

> Hashing is the process of transforming any given key or a string of characters into another value. This is usually represented by a shorter, fixed-length value or key that represents and makes it easier to find or employ the original string. The most popular use for hashing is the implementation of hash tables
>
> -- <cite>https://www.techtarget.com/</cite>

We can create and compare hashes of two files to find out if they are identical: <br/>
`md5 <filename1>; md5 <filename2>`

<br/>

### SLURM

SLURM is workload manager / job scheduler used by many of the world's supercomputers. It allocates exclusive or non-exclusive access to computer resources and it manages the queue of pending jobs.

There's a number of very helpful commands:

`$ sinfo`             -> shows us overall information about our server <br/>
`$ htop`              -> shows us how many cores are used and what <br/> processes are running
`$ squeue`            -> lists all of the queued processes <br/>
`$ srun <command>`    -> runs a command on the host system <br/>
`$ srun <command> &`  -> the addition of `&` allows the command to run in the background <br/>
`$ scancel <jobid>`   -> cancels a queues job <br/>
`$ squeue -u $USER`   -> cancels all jobs queued by a user <br/>


---
<br/><br/>


# Introduction to Shell Scripting

A text file that contains a sequence of commands for a UNIX-based operating system is called a shell script. It combines a sequence of commands into a single script instead of having to type them in one by one.  

These scripts can be written and edited in an editor. Our personal choice is Atom, but there's a wide selection of other editors (Sublime, Visual Studio etc.).

Every script aimed at unix-like operating systems is initiated by a *shebang* which tells the program loader what interpreter program needs to be launched.

If a script is initiated with `#!/bin/sh`, then the program loader is instructed to run the program /bin/sh.

Commenting inside these scripts works by staring the line with a hash `#`. Anything after the hash is commented out and ignored by the interpreter.

<br/>

### Basic Scripts

<br/>

**Command 01 -> Print Hello World.**

```
#!/bin/sh
echo "Hello World"   # Prints Hello World
```

<br/>

**Command 02 -> Create variable and then print it.**

```
name="Aris"
echo "Hello $name"   # Here we print "Hello <NAME> to <STDOUT>"
```

<br/>

**Command 03 -> Overriding previous command and saving it as positional argument**

```
echo "What is your name?"
read name
echo "Hello $name"
# script executes sequentially in the shell, declaration in command 2 gets overridden by command 3

echo "Hello $1"      
# positional argument/parameter that can be saved and executed in command line ex. ./file "Alex"
```

<br/>

**Command 04 -> Assign course participants to multiple variables and then call on them individually.**

```
workdir=$(pwd)
files=$(ls)

echo "Current directory:" $workdir    # Prints current working directory to <STDOUT>
echo "With files:" $files

names[1]="Lukas"
names[2]="Jan"
names[3]="Annie"
i=1

echo "Some course participants: " ${names[*]}
echo "First one is: ${names[1]}"
```

<br/>

**Command 05 -> Prints the name of all course participants with a for loop.**

```
for name in ${names[*]};    # Iterates through course participants and assigns them to name
  do
    echo $name
  done;
```

<br/>

**Command 06 -> Prints the name of all course participants numbered, with a for loop.**

```
or name in ${names[*]};     # Iterates through course participants and assigns them to name
  do
    echo "Participant $i" $name;
    i=$((i+1))              # double bracket shows system that it is an integer
  done;
```

<br/>

**Command 07 -> Our first if/else loop.**

```
name=$1

if [ $name == "Alex" ]      # = equal is an operator but regular expressions can also go into it
  then
    echo "You are not a student. \n"    # backslash n on mac is a new line
  else
    echo "Good job making this script. "
fi

echo "You are $name! "
```

<br/>

**Command 08 -> Breaking the loop as soon as the count reaches 5 and print the result.**

```
for a in 1 2 3 4 5 6 7 8 9 10
do
  # If a is equal to 5 break the loop
  if [ $a == 5 ]
    then
      break

  fi
  echo "Iteration no $a"
  # Print the value
done
```

<br/>

**Command 09 -> Prints all values that are less than 10.**

```
a=0
while [ $a -lt 10 ]       # -lt means less then
do
  # Print the values
  echo $a
  # Increment the value
  a=$((a+1))
done
```

<br/>

**Command 10 -> Redirect a file into a standard input**

```
a=0
file=$1

while read -r line;         # requires line ending (extra line even empty), otherwise it ignores the last line
do
  # Print the values
  echo "Line Nr $a: $line"

  # increment the value
  a=$((a+1))
done < $file                # < redirects what comes after into standard input
```

Preparation for upcoming first challenge:

```
ls > all_directories
cat all_directories | sed "/[a-z._]*dir.*/d" > all_directories_2
split --number=l/4 all_directories_2
```

<br/><br/><br/>

## Challenge 1 . Alignment Tool Comparison

**Goals**
1. Comparison between four optimal global alignment Tools
2. Needleman-Wunsch - Emboss Package
3. BLAST
     - fasta vs. fasta DB
     - fasta vs. indexing DB
4. VSEARCH
5. plot 4 different scenarios - table (columns: Software used, time, DB size)
6. find out if multithreading helps (1 CPU, 5 CPUs 10CPUs)

**Steps**
1. Subsetting for DB sizes
2. Measure the time
     - call 4 different software's with different parameters
     -> parameters (threads and DB size) / loops (loop within loop) & later also input file 1.fa and 10.fa
3. srun from within the loop
     -> -c $threads
4. append the results to different files (for every group member)
     - predefined data structure
     -> delimiter ";" , time "" , DB: $(ls) , threads: threads.txt $(cat) -> $threads
5. call R --> plot

<br/>  

```
#!/bin/sh

sf="/LETHE/COURSES/bin/SeqFilter/bin/SeqFilter"        # setting absolute path as variable
n=100000                                               # to avoid mistakes while editing, setting number as variable

grep "^>" its2.viridiplantae.none.2019-07-16.tax.fa | head --lines=$n | sed -e "s/;.*$//" -e "s/^>//"  > $n.list        # sed "." means every character ,"^" means beginning ,"$" means ending , -e adds filters indefinitely

$sf -p --ids-pattern $n.list -o $n.fa its2.viridiplantae.none.2019-07-16.tax.fa &       # -p adds Seqfilter progressbar
```

<br/>  

```
#!/bin/sh
dbdir="/LETHE/COURSES/data/aliScale"
script=$1

rm -f arisspreadsheet.csv
for threads in 1;
  do
      looping through databases
      for dbs in $(ls $dbdir/*.fa );
        do
          #if [ "$dbs" == "$dbdir/10000.fa" ]
            then
              break
           else
           looping through input files
              for inputfile in 1 10 100;
                do
                  srun -c $threads sh $script $threads $dbs $inputfile $dbdir & # echo "i $inputfile t $threads d $dbs" >> output.csv       # double >> is for appending instead of overwriting
                  echo "t $threads, d $dbs, i $inputfile"
              done  # end for input file loop
          fi  # end for if condition
    done  # end for databases loop
  done  # end for threads loop
```

<br/>  

This second script is repeatedly executed inside the above script as `$inputfile` and the results are piped into an output file that we can then use in R so that we can plot our results:

```
#!/bin/sh

threads=$1
dbs=$2
inputfile=$3
dbdir=$4
software="Needle"

needle="/LETHE/COURSES/bin/python_scripts/needle2.py"

start=$(date +%s)
python3 $needle "$dbdir/$inputfile.fa" $dbs
end=$(date +%s)
runtime=$((end-start))

echo "$software; $runtime; $dbs; $threads; $inputfile" >> arisspreadsheet.csv
```

<br/>  

All of our groups results need to be entered into R and graphed:

```
getwd()

#set working directory
setwd("/Volumes/KELLER-COURSES/students")

#read in file
read.table("CombinedResults.csv", sep = ";") -> var

#show first 20 lines
head(var, n = 20)

#change column names
colnames(var) <- c("software", "runtime", "database", "threads", "input_size")

#remove unnessesary stuff
g <- grep(".fa$", var$database)
var <- var[g,]

#remove datapaths from database column
(var$database <- gsub(".*/", "", var$database))

var$database <- gsub(".fa", "", var$database)
var$database

(var$database <- gsub("its2\\..*", "300000", var$database))

(var$database <- gsub("tri.*", "900000", var$database))

#check class of data
class(var$database)
class(var$threads)

var$database2 <- as.numeric(var$database)

head(var)

#plotting
library(ggplot2)

ggplot(var, aes(x = database2, y = runtime, shape = factor(input_size), col = factor(threads))) +
       geom_point(size = 5) +
       ggtitle("Runtime data mixed results") +
       geom_smooth(method = "lm") +
       facet_grid(software~.)
```

<br/>

<div align="center">
  <img src="assets/runtimeresults.png" alt="logo" width="auto" height="auto" />
</div>


<br/><br/>  

All of our alignment softwares had their runtime increase linearly with increasing database sizes.

BLAST with indexing was able to multithread whereas BLAST without indexing was bottlenecked by single thread performance which resulted in slower runtimes.

Vsearch was the fastest software, able to use the given resources most efficiently.

Needle was by far the slowest alignment software which goes well with our expectation.


<br/><br/><br/>


## Challenge 2 . BacGenStat Project

```
#!/bn/sh

# working directory
bdir="/LETHE/COURSES/students/aris-protopapas/genomes"

script_fna=$1
script_gff=$2

rm -f aris_fna_output.csv
rm -f aris_gff_output.csv

# Initial loop through our .fna files
for file_fna in $(ls $bdir/fasta);
  do
    srun -c 1 sh $script_fna $file_fna & sleep 0.1
    #break
    #echo $file_fna
  done

# Secondary loop through our .gff files
for file_gff in $(ls $bdir/gff);
  do
    srun -c 1 sh $script_gff $file_gff & sleep 0.1
    #break
    #echo $file_gff
  done

#put into background slurm queue by adding & in command line
```

<br/>  

Script 2 provides us with data for gene size, number of chromosomes and G/C percentage and is output into a file for later processing with R in challenge 3:

```
#!/bn/sh

# working directory
bdir="/LETHE/COURSES/students/aris-protopapas/genomes"

usedfile=$1

# count chromosome number
numchrom=$(grep -c ">" $bdir/fasta/$usedfile)
#echo "test chrome number: $numchrom"

# count genome size
gensize=$(sed -e "s/;.*$//" -e "s/^>//" $bdir/fasta/$usedfile | wc -m)
#echo "test gene size: $gensize"

# establish gc percentage
gccount=$(sed -e "s/;.*$//" -e "s/^>//" $bdir/fasta/$usedfile | grep -Eo "C|G" | wc -l )
gcperc=$(echo "scale=5; $gccount/$gensize*100" | bc)
#echo "test gc percentage: $gcperc"

echo "$usedfile; $gensize; $numchrom; $gcperc" >> aris_fna_output.csv
```

<br/>

Script 3 that provides us with gene count data and is output into a file for later processing with R in challenge 3:

```
#!/bn/sh

# working directory
bdir="/LETHE/COURSES/students/aris-protopapas/genomes"

usedsecondfile=$1

# count number of genomes
gencount=$(grep -c "ID=gene" $bdir/gff/$usedsecondfile)
#echo "gene count test: $gencount"

echo "$usedsecondfile; $gencount" >> aris_gff_output.csv
```

<br/><br/><br/>

## Challenge 3 . Taxonomy Project

First part of the taxonomy script:

```
#!/bin/sh

# working directory
bdir="/LETHE/COURSES/students/aris-protopapas/genomes/gff"

script=$1

rm -f aris_tax_output.csv

for file_gff in $(ls $bdir/*.gff);
  do
    srun -c 1 $script $file_gff & sleep 0.1

  done


cat ./aris-protopapas/genomes/aris_tax_output.csv ./Lukas/genomes/lukas_tax_output.csv ./Jan/genomes/jan_tax_output.csv ./Annie/genomes/annie_tax_output.csv > complete_tax_output.csv


# sed /^[^;]$/s  --> the hat inside the square brackets

# pcg tree tool on github

# docker is unsafe for HPC singularity can be used with dockerfiles on HPCs
# Openstack is alternative for virtual machines on HPCs

# illumina sequencing best for bacteria and cheaper, nanopore for plants, hybrid approach with illumina data (loop them on top to get quality genom)
```

Second part of the taxonomy script:

```
#!/bin/sh

# working directory
bdir="/LETHE/COURSES/students/aris-protopapas/genomes/gff"

file_gff=$1

id=$(grep "##species" $bdir/$file_gff | head -n 1 | cut -d"=" -f2)
#echo "id_test: $id"

#var=$(docker run --rm ncbi/edirect /bin/bash -c "efetch -db taxonomy -id $id -format xml | xtract -pattern Taxon -block '*/Taxon' -tab '\n' -element Rank, ScientificName | grep '^phylum\|^family\|^genus' | cut -d$'\t' -f2 | tr -s '\n' ';' ")
#echo "var_test: $var"
var=$(grep "^$id[[:space:]]" /LETHE/COURSES/data/taxonomy/rankedlineage.dmp | cut -d"|" -f4,5,8 | tr "|" ";" | sed "s/[[:space:]]//g")
#echo "var_test $var"

echo "$file_gff; $var" >> aris_tax_output.csv

#grep "##species" *.gff | head | uniq | sed "s/:.*=/" > taxid.tmp
#grep "^587[[:space:]]" | rankedlineage.dmp | cut -d"|" -f4,5,8 | tr "|" ";" | sed "s/[[:space:]]//g"
#sed -e "s/.*;/^/" -e "s"
```


And finally, all previous output files can be used to create plots in R:

```
getwd()

# set working directory
setwd("/Volumes/KELLER-COURSES/students")

# read our table
var <- read.table("CombinedResults.csv", sep = ";")

head(var)

# assign names to columns
colnames(var) <- c("software", "runtime", "database", "threads", "inputsize")

# positive filtering
g <- grep(".fa$", var$database)

# subset our dataset - everything before comma lines we keep, after comma are columns
var[g,]
var <- var[g,]

var$database

# general expression substitution - remove datapaths from columns
(var$database <- gsub(".*/", "", var$database))

var$database <- gsub(".fa", "", var$database)
var$database

(var$database <- gsub("its2\\..*", "300000", var$database))

(var$database <- gsub("tri.*", "900000", var$database))

class(var$dataabse)
class(var$threads)

# as.numeric interpretates as numeric, numeric on it's own sets it as numeric
var$database2 <- as.numeric(var$database)

head(var)

library(ggplot2)

ggplot(var, aes(x = database2, y = runtime, shape = factor(inputsize), col = factor(threads))) +
  geom_point(size = 6) +
  ggtitle("Runtime data mixed results") +
  facet_grid(software~.) +      #rows - columns
  geom_smooth(method = "lm")     #lm means linear model
```

The analysis I applied did not generate any good plots that were worth presenting in the protocol.


---
<br/><br/>


<div align="center">
  <img src="assets/docker.jpg" alt="logo" width="auto" height="auto" />
</div>


# Docker

Dockers are lightweight containers that can be executed and contain the code, system tools, libraries and settings needed to run an application. Dockers are available for windows and Linux based applications and they'll always run the exact same way.


Here is an example where we execute a docker to fetch data from NCBI:

```
docker run --rm -it ncbi/edirect  /bin/bash -c  "efetch -db taxonomy -id 587 -format xml | xtract -pattern Taxon -block '*/Taxon' -tab '\n'  -element Id,Rank,TaxId,ScientificName"
```

---
<br/><br/>  


# License

We've reached the end of the protocol.

Distributed under the no License. See LICENSE.txt for more information.
