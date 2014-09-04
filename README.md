C5
==
___ C5 decision tree algorithm for java. ___

There are only four steps for c5 scoring.

>* Parse your names file.

>* Parse your tree file.

>* Construct your Scoring instance by Names and Trees.

>* Call Scoring score with your input variables.

>>

		NamesParser namesAnalyzer = new NamesParser(namesFile);
		Names names = namesAnalyzer.parse();

	    TreeParser treeParser = new TreeParser(treeFile);
		Node[] trees = treeParser.parse();

		Scoring scoring = new Scoring(trees, names);

		Result result = scoring.score(inputVariables);
