# gaia-dr3-photometric-uncertainties
Tool to reproduce the median DR3 photometric uncertainty for G, BP and RP instruments and scale them to different number of observations.

The process to derive this median behaviour is explained in the GAIA-C5-TN-UB-JMC-031 Technical note. 
The code needs an input file with the B-spline knots and coefficients also provided here.
The same tool is also able to scale the fitted B-splines to sources with different numbers of observations.

Note that these uncertainties do not take into account systematic effects remaining in the data that originate in the properties 
of the source e.g. magnitude and colour. Systematic effects remaining in the data that vary with each CCD or FoV are accounted for 
by this tool and can be scaled to future releases with the understanding that these systematic effects will be reduced. 
We recommend reading [Riello et al. (2021)](https://doi.org/10.1051/0004-6361/202039587) and [Fabricius et al. (2021)](https://doi.org/10.1051/0004-6361/202039834) for getting a better understanding of the remaining 
systematics within the (E)DR3 photometry.

This code was developed by CU5 calibration unit, under Gaia Data Processing and Analysis Consortium (DPAC). In particular, it was 
developed by the authors of the technical note (J.M. Carrasco, F. De Angeli, M. Riello, C. Jordi) and some helpful comments were 
provided by J. de Bruijne and D.W. Evans.

If your research benefits from the use of this code, we would appreciate if you could include the following acknowledgement in 
your publication:

> This research has made use of the tool provided by Gaia DPAC (https://www.cosmos.esa.int/web/gaia/dr3-software-tools) to reproduce (E)DR3 Gaia photometric uncertainties described in the GAIA-C5-TN-UB-JMC-031 technical note using data in Riello et al (2021).


### References

* [https://www.cosmos.esa.int/web/gaia/dr3-software-tools](https://www.cosmos.esa.int/web/gaia/dr3-software-tools)
* [Gaia Early Data Release 3. Photometric content and validation](https://doi.org/10.1051/0004-6361/202039587) - Riello et al (2021)
```
@ARTICLE{2021A&A...649A...3R,
       author = {{Riello}, M. and {De Angeli}, F. and {Evans}, D.~W. and {Montegriffo}, P. and {Carrasco}, J.~M. and {Busso}, G. and {Palaversa}, L. and {Burgess}, P.~W. and {Diener}, C. and {Davidson}, M. and {Rowell}, N. and {Fabricius}, C. and {Jordi}, C. and {Bellazzini}, M. and {Pancino}, E. and {Harrison}, D.~L. and {Cacciari}, C. and {van Leeuwen}, F. and {Hambly}, N.~C. and {Hodgkin}, S.~T. and {Osborne}, P.~J. and {Altavilla}, G. and {Barstow}, M.~A. and {Brown}, A.~G.~A. and {Castellani}, M. and {Cowell}, S. and {De Luise}, F. and {Gilmore}, G. and {Giuffrida}, G. and {Hidalgo}, S. and {Holland}, G. and {Marinoni}, S. and {Pagani}, C. and {Piersimoni}, A.~M. and {Pulone}, L. and {Ragaini}, S. and {Rainer}, M. and {Richards}, P.~J. and {Sanna}, N. and {Walton}, N.~A. and {Weiler}, M. and {Yoldas}, A.},
        title = "{Gaia Early Data Release 3. Photometric content and validation}",
      journal = {\aap},
     keywords = {catalogs, surveys, instrumentation: photometers, techniques: photometric, Galaxy: general, Astrophysics - Instrumentation and Methods for Astrophysics},
         year = 2021,
        month = may,
       volume = {649},
          eid = {A3},
        pages = {A3},
          doi = {10.1051/0004-6361/202039587},
archivePrefix = {arXiv},
       eprint = {2012.01916},
 primaryClass = {astro-ph.IM},
       adsurl = {https://ui.adsabs.harvard.edu/abs/2021A&A...649A...3R},
      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
}
```
* [Gaia Early Data Release 3. Catalogue validation](https://doi.org/10.1051/0004-6361/202039834) - Fabricius et al (2021)
