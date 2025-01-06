**1.1.1 Architecture of the CPU**

- **The purpose of the CPU:**  
  - The CPU:  
    - A chip within the computer which controls the operation of all parts of the computer and decodes then executes program instructions. This is the central processing unit, and executes the “fetch decode execute” cycle which is explained below.  
  - The fetch-execute cycle:  
    - The CPU repeats these steps: instructions and data are fetched from main memory and stored one-by-one in CPU registers, and then decoded and executed by the processor  
    - The address from the program counter will be transferred to the MAR and the program counter will count up one address. The CPU will fetch the data or instructions from RAM, according to the address indicated in the MAR, and will be stored in the MDR. This is the fetching part. Then, the control unit will decode the instruction and manage the flow of data/instructions to the correct “area”. If any instruction requires arithmetic, then the control unit will send the instruction to the ALU, where the arithmetic will be done. Then it will be stored in the accumulator. Lastly, any data required to be stored will be sent back to the MDR, to be written to the correct memory location in RAM. This is the executing part.

- **Common CPU components and their function:**  
  -  ALU (Arithmetic Logic Unit)  
    - The circuitry in the CPU which carries out arithmetic and logical operations  
  - CU (Control Unit)  
    - Circuitry within a computer's processor that directs operations and data flow  
  - (CPU) Cache  
    - High speed memory built into the CPU, allowing frequently used instructions and data to be accessed more quickly than from RAM  
  - Registers  
    - A tiny area of memory within the CPU where a single instruction or piece of data is stored temporarily

- **Von Neumann architecture:**  
  - Von Neumann architecture:  
    - The design on which modern computers are based: program instructions and data are both held in main memory, in binary, to be accessed by the CPU  
    - The instructions that are stored in binary to “manipulate” the data (only in Von Neumann architecture) (program instructions, but also operating system or drivers)

    

  - MAR (Memory Address Register)  
    - A register which contains the address of the instruction, or data, currently being read from, or written to, main memory.

    

    

  - MDR (Memory Data Register)  
    - A register which contains the data or instruction which has just been fetched from main memory.  
  - Program Counter  
    - A register which contains the address of the next instruction or data to be fetched from memory  
  - Accumulator  
    - A register which stores the results of arithmetic and logical operations.

**1.1.2 CPU performance**

- **How common characteristics of CPUs affect their performance:**  
  - Clock speed  
    - The higher the clock speed, the more instruction cycles the CPU can deal with in a second; typically measured in GHz.  
  - Cache size  
    - The larger the amount of cache the CPU has, the more instructions or data it can store without having to fetch from main memory, and therefore the faster it will perform.  
  - Number of cores  
    - Some CPUs have more than one core, each containing its own ALU and registers and therefore capable of carrying out instructions independently. The more cores it has, the more instructions the CPU can potentially process simultaneously

**1.1.3 Embedded systems**

- **Embedded Systems**  
  - A computer system (hardware and software) that has a dedicated function within another mechanical or electronic system, (rather than a "multipurpose" computer)  
- **The purpose and characteristics of embedded systems**  
  - Low power consumption (Designed to operate on batteries for long periods, minimizing energy usage) (Thermostats)   
  - Small size (Utilizes compact components to fit into limited spaces within devices) (Watches/Fitness trackers)  
  - Rugged operating ranges (Optimized for reliability in harsh environments with minimal maintenance) (Outdoor electronic thermometer)  
  - Low cost per unit (Specialised design reduces manufacturing costs, ideal for mass production (Microwaves))  
- Unable to upload custom software. They have their set software/function on ROM, where uploading a bootloader is not possible  
- They have a dedicated function (brew time/strength, timer), and cannot perform other tasks, like a multi-purpose computer  
- No HDD/SDDs, software on ROM  
- Built within another device


- **Examples of embedded systems**  
  - Smart Thermostat, Washing Machine, Pacemaker, Traffic Light, Router, Coffee Maker, Fitness Tracker

**1.2.1 Primary storage (memory)**

- **Primary Storage**  
  - Also known as memory, it holds data that can be directly accessed by the CPU, and includes CPU registers, CPU cache, RAM and ROM.  
- **The need for primary storage**  
  - Primary storage is required as it is storage that is directly accessed by the CPU, therefore it is faster to fetch data and instructions from both ROM and RAM, rather than a slow secondary storage, such as SSDs or HDDs  
- **The difference between RAM and ROM**  
  - ROM is non volatile (does not lose stored data/instructions when no power is supplied), while RAM is volatile  
  - ROM stores the firmware/boot up instructions (BIOS/UEFI) or sometimes the entire program on some embedded systems  
  - ROM cannot be written to, but RAM can be read and written to  
- **The purpose of ROM in a computer system**  
  - ROM (Read-Only Memory) is non-volatile memory used to store the initial instructions for starting a computer, such as the BIOS (Basic Input/Output System). It retains its data even when the power is turned off and cannot be altered or rewritten (Hence Read Only).  
- **The purpose of RAM in a computer system**  
  - RAM is used for temporarily storing data and instructions that are currently being used by the CPU. It allows for quick access of data (though slower than caches), making it much faster than secondary storage like hard drives or SSDs. RAM is volatile (loses its data when power is turned off)  
- **Virtual memory**  
  - Virtual memory is a “memory management technique” that uses secondary storage when the main memory is full.  
  - Data not currently in use is moved to a space on the hard drive, freeing up RAM for other (active) tasks. This allows larger programs to run and enables multitasking, even if the physical RAM is limited. Then gets transferred back to RAM when required by the CPU, because HDDs and SSDs are secondary storage and cannot be directly accessed by the CPU

  - Although this process helps manage memory efficiently, it can slow down performance because accessing data from the hard drive is slower than from RAM.   
  - Although accessing data from the hard drive is slower than from RAM, it is a better alternative to significant performance issues and applications crashing or failing to start.  
  - Increasing RAM will reduce the possibility of your computer system requiring the use of virtual memory, allowing your computer to run faster and encounter fewer performance issues.  
      
- **Cache**  
  - High speed memory built into the CPU, allowing frequently used instructions and data to be accessed more quickly than from RAM

**1.2.2 Secondary storage**

- **The need for secondary storage**  
  - Secondary storage is non-volatile memory used for high capacity, long-term “data retention”, used to store the physical OS and programs/applications  
  - Examples include, but are not limited to, HDDs, SSDs, Floppy disks, USB flash drives, SD cards  
- **Common types of storage:**  
  - Optical Storage  
    - Uses lasers to read/write data on discs (e.g., CDs, DVDs, Blu-ray).  
  - Magnetic Storage  
    - Uses magnetic fields to store data on spinning disks (e.g., hard drives).  
  - Solid State Storage  
    - Uses flash memory to store data without moving parts (e.g., SSDs, USB drives).  
- **The advantages and disadvantages of different storage devices and storage media relating to these characteristics:**  
  - Optical  
    - Capacity  
      - Lower compared to magnetic and solid-state storage (CD: 700 MB, DVD: 4.7 GB, Blu-ray: 25-50 GB)  
    - Speed  
      - Slower than magnetic and solid-state storage, especially for writing data  
    - Portability  
      - Highly portable and easy to transport due to compact-ness but fragile, because easily scratched, corrupting data  
    - Durability  
      - Susceptible to physical damage (scratches) and environmental conditions (heat, sunlight).  
    - Reliability  
      - Can degrade over time, especially if improperly stored or frequently used  
    - Cost  
      - Low cost per unit

  - Magnetic  
    - Capacity  
      - High capacity (HDDs: 500 GB to several TBs)  
          
    - Speed  
      - Moderate, faster read/write speeds than optical storage, but slower than solid-state storage  
    - Portability  
      - Heavier and bulkier compared to optical and solid-state storage.  
    - Durability  
      - Moving parts make HDDs more prone to damage and data loss if dropped, posing a risk during travel  
    - Reliability  
      - Can fail due to mechanical parts or wear over time, limited read/write cycles, but overall, very reliable  
    - Cost  
      - Low cost per unit, lower cost per gigabyte compared to solid-state storage.

  - Solid State  
    - Capacity  
      - Moderate to high capacity (SSDs: 120 GB to several TBs).  
          
    - Speed  
      - Very fast read/write speeds, much faster than magnetic and optical storage  
    - Portability  
      - Extremely portable, especially in USB drives and small SSDs  
    - Durability  
      - No moving parts, due to NAND flash technology. so they are very durable and resistant to shock  
    - Reliability  
      - Very reliable due to no mechanical parts, and more resistant to environmental factors  
    - Cost  
      - Still more expensive per GB than magnetic storage (about $0.03-0.06 per GB vs. $0.08-0.10 per GB)

**1.2.3 Units**

- **The units of data storage:**  
  - Bit  
  - Nibble (4 bits)  
  - Byte (8 bits)  
  - Kilobyte (1,000 bytes or 1 KB)  
  - Megabyte (1,000 KB)  
  - Gigabyte (1,000 MB)  
  - Terabyte (1,000 GB)  
  - Petabyte (1,000 TB)  
- **File size calculations**  
  - sound file size \= sample rate \* duration (seconds) \* bit depth  
  - image file size \= colour depth \* image height (pixels) \* image width (pixels)  
  - text file size \= bits per character \* number of characters

- **24 bit vs hex in colours**  
  - Compact and Easier to Interpret: Hexadecimal represents a 24-bit color value in just six digits (e.g., \#00ccff), making it shorter and simpler than using binary or decimal.  
  - Simplifies Color Adjustments: Each pair of hex digits directly corresponds to the RGB channels, allowing developers to quickly understand and adjust colors without dealing with complex binary or decimal values.

- **Overflow Errors**  
  - Overflow errors occur when a value exceeds the storage capacity of the allocated memory or data type (Binary: 1000 0000 \+ 1000 0000\)

Certainly\! Here's the same information with dashes and proper indentation:

### **Sample Rate**

* **Playback Quality**:  
  * Higher sample rate improves sound accuracy, especially for higher frequencies (e.g., treble).  
  * For most music, 44.1 kHz (CD quality) is sufficient.  
* **File Size**:  
  * A higher sample rate increases the file size because more data is captured per second.

### **Duration**

* **Playback Quality**:  
  * Doesn’t directly affect the quality, but longer files may suffer from compression if not managed properly.  
* **File Size**:  
  * Longer audio files are larger because they contain more data.

### **Bit Depth**

* **Playback Quality**:  
  * Higher bit depth improves sound detail and dynamic range, allowing for more volume levels and subtle sounds.  
* **File Size**:  
  * A higher bit depth results in a larger file, as each sample uses more data.

### **Summary**

* **Higher sample rate and bit depth** \= better sound quality but larger file size.  
* **Longer duration** \= bigger file size.

**The need for compression:**

- Reduces the file size of audio, video, and images, making them easier to store and share.  
- Minimizes the amount of data needed for transmission over the internet, improving loading times and streaming quality.  
- Helps save storage space on devices (e.g., phones, computers, servers).  
- Allows for quicker downloads and more efficient use of bandwidth.

**Lossy Compression:**

- Description: Removes some data from the original file, typically data that is less noticeable to the human ear or eye (e.g., removing some audio frequencies or reducing image quality)

- Advantages:  
  - Greatly reduces file size.  
  - Common in streaming, audio, and video formats (e.g., MP3, JPEG, MP4).  
- Disadvantages:  
  - Loss of some quality that cannot be recovered (irreversible).  
  - May result in visible or audible degradation after heavy compression.


#### 

#### **Lossless Compression**

- Description: Compresses the file without losing any data. The original file can be perfectly reconstructed from the compressed version  
     
- Advantages:  
  - No loss of quality \- everything is preserved exactly as it was.  
  - Ideal for archiving and professional work (PNG or TIFF for images)  
- Disadvantages:  
  - File sizes are still smaller than uncompressed files but larger than those with lossy compression.  
  - Less efficient in reducing file size compared to lossy compression.

