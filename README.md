
# comp-arch-lab-1
A repository containing code files and reports for the first lab of the Advanced Computer Architecture course.

### Ερώτημα 1
Για να έχουμε πρόσβαση στα αποτελέσματα των προσομοιώσεων, αρχικά δημιουργούμε τον φάκελο _sim_results_, στον οποίο θα αποθηκεύονται. Τρέχουμε την εντολή

	./build/ARM/gem5.opt -d sim_results configs/example/arm/starter_se.py	--cpu="minor" "tests/test-progs/hello/bin/arm/linux/hello"
	
για να εκτελεστεί το _hello_ και τα αποτελέσματά του να αποθηκευτούν στον _sim_results_. 
Η συχνότητα αλλάζει με το argument _--cpu-freq=VALUE_ στην εντολή. Τρέχουμε π.χ. την εντολή

	./build/ARM/gem5.opt -d sim_results configs/example/arm/starter_se.py	--cpu="minor" --cpu-freq="2GHz" "tests/test-progs/hello/bin/arm/linux/hello"
για να κάνουμε την συχνότητα 2 GHz (το default είναι 1GHz). 
