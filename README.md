# WEKA (developer version)

Read-only git mirror of Weka's subversion repository.

## Source code

The official WEKA source code of the developer version is available from this URL:

https://svn.cms.waikato.ac.nz/svn/weka/trunk/

## Contributions/Bug fixes

Contributions and bug fixes an be contributed as patch file and posted to the
[WEKA mailing list](https://list.waikato.ac.nz/mailman/listinfo/wekalist).

## Links

* [WEKA Homepage](https://www.cs.waikato.ac.nz/ml/weka/)

Hey Maxence,

ligne 536 de 
weka-trunk/weka/src/main/java/weka/core/neighboursearch/NearestNeighbourSearch.java (utilisé par IBK!):
Remplacer l'affectation de la distance
"protected DistanceFunction m_DistanceFunction = new EuclideanDistance();"
par
protected DistanceFunction m_DistanceFunction = new ManhattanDistance();
ainsi que l'import
import weka.core.EuclideanDistance; -> import weka.core.ManhattanDistance;

