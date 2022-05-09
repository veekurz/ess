# Energy Sorting Script

Energy sorting Script allows you to discard unnecessary Gaussian log-files, possibly containing repeating structures using
energy criterion (∆Etot > 0.00001 Hartree by default). The Algorithm of ESS includes the following steps

1) Extraction of the most inmoptarnt data from a list of Gaussian-log files: filename, ZPE1, δH.1, δG.1, Etot, <S²>, 1-st
frequincy. Check than 1-st frequincy > 0.

2) Sorting the list of extracted data in ascending order of Etot.

3) Comparison by Etot. Each log-file will be compared with the previos one by Etot using the following criterion: If ∆Etot >
0.00001 Hartree (by default) then it makes sense to consider the current file. Otherwise: the current file is most likely a
“replicant/duplicate”, possibly containing the same structure as in previous file.

References:
Korotenko, V., Energy Sorting Script (ESS). https://github.com/vnkorotenko/ess 2022.

If you have questions, please ask.
Vasily Korotenko
vnkorotenko@gmail.com
