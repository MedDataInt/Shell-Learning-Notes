# Shell-Learning-Notes
This is for me to learn some Shell script
A .sh file is a shell script, which is a plain text file containing a series of commands written for shell (command-line interpreter) on Unix like operating systems (e.g., Linux, macOS). These commands are executed sequentially when the script is run.  
Shell scripts are used to automate repetitive tasks, execute mutiple commands in sequence, or create custom workflows.
* Run software tools with specific parameters
* Manage large datasets
* Automate pipelines for data preprocessing, alignment, analysis, and visualization.

  
## Structure of a Shell Script (.sh file)
Here is a typical structure of a .sh file:  
1. Shebang Line
   ```bash
   #!/bin/bash
2. Commands
   ```bash
   echo "Starting analysis..."
   mkdir results
   cd data
   bowtie2 -x genome_index -U sample.fastq -S sample.sam
3. Comments
   ```bash
   # This script aligns reads to the genome and calls peaks
4. Variables(optional)
   ```bash
   DATA_DIR="/path/to/data"
   echo "Data directory: $DATA_DIR"

## How to Run a .sh File
* if Window line exist
  ```bash
  dos2unix test.sh
  ```
* use bash or sh
```bash
bash script.sh
# sh script.sh
```
* Making the file executable
```bash
chmod +x script.sh
./script.sh
```

## How to View a .sh File
* command-line editors: nano, vim, less, cat.
  ```bash
  vi filter_blacklist.sh
  ```
* Graphical editors: VSCode, Sublime Text, Notepad++
## Common .sh File Use Cases
* Running alignment tools like **bowtie2** or **STAR**.
* Peak calling with tools like **MACS2**.
* Automating preprocessing steps like trimming with **Trimmomatic**.
* Performing batch analysis on clusters using job schedulers like **SLURM** or **SGE**.

  
