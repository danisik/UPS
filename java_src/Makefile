JC=javac

all: client jar del

client:
	ant build

jar:
	mv bin/draughts ../java_src/draughts
	echo Main-class: draughts.main.Draughts > manifest.txt
	jar cvfm Draughts.jar manifest.txt draughts/connection/*.class draughts/constants/*.class draughts/enums/*.class draughts/field/*.class draughts/main/*.class draughts/messages/*.class draughts/piece/*.class draughts/windows/*.class img/*.png
	mv Draughts.jar ../

del:
	rm -f manifest.txt
	rm -Rf bin
	rm -Rf draughts
