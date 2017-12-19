# CSE 505 Project - Improving Adherence to Heart Failure Management Guidelines via Abductive Reasoning

## Student Details:

	Name		-	FNU Gaurav

## Main Project Folders/File Descriptions:

	- ./sasp
		s(ASP) program that functions as ASP solver for the given project.lp

	- ./project.lp
		Contains the sample implementation extracted from the paper for verification of implementation methodology as well result generation

	- ./README.md
		The file that you are reading right now

## Steps to setup:

	- On UNIX based systems (ubuntu, MacOSX)
		* `./sasp -i -la -s0 project.lp`
			-- This command will open the file 'project.lp' in Interactive Mode and option '-s0' enables the computation of all possible answer sets
		* `recommendation(diuretics, class_1).` or `recommendation(beta_blockers, class_2a).`
			-- This serves as the sample input for the sample rules and sample patient data that we have extracted from the paper that we are planning to use for the demonstration/verification of the workings of the paper.

## Help options for s(ASP) system

The available options are:

	-h, -?, {help Print this help message and terminate.
	-i, {interactive Run in user / interactive mode.
	-a, {auto Run in automatic mode (no user interaction).
	-sN Compute N answer sets, where N  0. 0 for all.
	Ignored unless running in automatic mode.
	-v, {verbose Enable verbose progress messages.
	-vv, {veryverbose Enable very verbose progress messages.
	-j Print proof tree for each solution.
	-n Hide goals added to solution by global consistency
	checks.
	-la Print a separate list of succeeding abducibles with each CHS. List will only be printed if at least one abducible has succeeded.

Reference:
	- https://sourceforge.net/projects/sasp-system/ for s(ASP)
	- https://arxiv.org/pdf/1707.04957.pdf for PDF version of above stated paper