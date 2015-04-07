# Introduction #

This project represents an objective approach for validation of gene network modeling and identification by presenting an Artificial Gene Networks (AGNs) model generation through theoretical models of complex networks, which is used to simulate temporal expression data.

The proposed framework allows several types of AGNs to be generated and used in order to simulate temporal expression data.

The results of the network identification method can then be compared to the original network in order to estimate its properties and accuracy.

Some of the most important theoretical models of complex networks have been assessed:
  * the uniformly-random Erdos-Rényi (ER)
  * the small-world Watts-Strogatz (WS)
  * the scale-free Barabási-Albert (BA)
  * geographical networks (GG).

# Details #

The source code, java binary (jar file) and documentation are available here.

The source codes are packed in file **jAGN-source-code-vxxx.zip**.

The binary file (jar file) and libraries are packed in file **jAGN-vxxx.jar**.

Where "vxxx" specifies the version of the file.

You need the [Java Runtime Environment (JRE)](http://www.java.com/en/download/) to execute jAGN software.

The JRE is free and is available for different operating systems.

You can run JAR-packaged applications with the Java interpreter.

The basic command is:

**java -jar jAGN-vxxx.jar**

or just double click on jAGN-vxxx.jar, if the JRE is visible in your operating system.

## Running on the console ##

If you need to execute a console version with various simulations, you can use the following instructions to execute the jAGN software:

**java -jar jAGN-vxxx.jar -v {path-output} {number-of-networks} {number-of-genes} {signal-size} {average-degree} {network-topology} {probability-of-redistribution-edges}**

Use {probability-of-redistribution-edges} only for WS networks.

<br>

<b>Example for ER, BA and GG networks:</b>

<b>java -jar jAGN-v102.jar -v /home/jAGNs/ 10 100 30 2 BA</b>

<br>

<b>Example for WS networks:</b>

<b>java -jar jAGN-v102.jar -v /home/jAGNs/ 10 100 30 2 WS 0.28</b>

<br>

<b>where in these examples:</b>

<ol><li>path-output == /home/jANGs/ or could be c:\temp\ or any path you want.<br>
</li><li>number-of-networks == 10 different simulation of the same network topology.<br>
</li><li>number-of-genes == number of genes (nodes) of each network.<br>
</li><li>signal-size = number of instants of time or experiments, i.e., signal size.<br>
</li><li>average-degree = average degree of connection per gene.<br>
</li><li>network-topology = the available networks topology are: ER, WS, BA and GG.<br>
</li><li>probability-of-redistribution-edges = use only for WS network topology to select the probability of redistribution its connections.