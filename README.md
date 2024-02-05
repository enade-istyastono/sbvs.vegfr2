# sbvs.vegfr2
<p>
  A computer program works in the command line interface (CLI) to predict whether a compound is a potentially potent VEGFR2 inhibitor.
The program works on a machine running Ubuntu 22.04.2 LTS and with AutoDock Vina v1.2.3 (https://autodock-vina.readthedocs.io/en/latest/index.html) and PyPLIF HIPPOS v0.1.2 (https://pyplif-hippos.readthedocs.io/en/latest/) installed.
</p>
<p>
  Installation: (i) Download the program into a suitable machine; (ii) Make the files sbvs.vegfr2, ensplif.vegfr2, and dectree.vegfr2 executable with the chmod command; (iii) Copy the whole directory pyplif_hippos from the PyPLIF HIPPOS software to the directory source of this program.</p>
<p>
  Usage: Copy the tested compound(s) in the pdbqt format into the directory of this program, and then run the program by typing "./sbvs.vegfr2 [file-name-of-the-compound-without-the-extension]" in the CLI. For example, the file CHEMBL567475.pdbqt (https://www.ebi.ac.uk/chembl/g/#search_results/all/query=CHEMBL567475) is provided here. By typing "./sbvs.vegfr2 CHEMBL567475" in the CLI and pressing the Enter key, the compound CHEMBL567475 will be run to predict its activity for about one and a half minutes. 
</p>
<p>
  Advanced usage: Basically, the sbvs.vegfr2 command runs the commands ensplif.vegfr2 and dectree.vegfr2, subsequently. Therefore, in order to optimize the use of computer power by using parallel software (https://www.gnu.org/software/parallel/), it is highly recommended to predict several compounds at once. This can be done by running in parallel the ensplif.vegfr2 program and then followed by running in parallel the dectree.vegfr2 program.  
</p>

