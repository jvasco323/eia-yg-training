Boundary line analysis
======================

	
**Revisiting Fermont et al. (2009)**

Sustaining food production in the years ahead will require productivity gains in resource use. Specific challenges include estimating the magnitude and thus the value of yield gaps, identifying limiting factors, and implementing profitable and sustainable  strategies. Closing yield gaps in arable farming, while improving resource use  efficiency, is also expected to minimize the expansion of arable land and emissions while reducing other undesirable externalities. 

Over the last years, new methodological approaches have been evolving within the context of yield gap assessment, mostly due to advances in data engineering and programming languages. One clear example is the mathematical computation of boundary-lines over crop yield datasets to decompose yield gaps (INCLUDE SOME REFERENCES, e.g., Silva et al.). The boundary-line analysis (BLA), based on the Law of the Minimum, is a powerful concept in agronomy which can be used for quantitative decomposition of yield gaps. The BLA is considered a useful complement to more traditional data analysis techniques. From a conceptual point of view, different approaches to fit boundary lines on crop data have been proposed throughout the last century. Five different methodological families can be identified:

1.	Curves fitted “manually and by eye” (e.g., French & Schultz, 1984);
2.	The use of crop simulation modelling for benchmarking potential yields (e.g., Passioura & Angus, 2010);
3.	Empirically based methods: grouping data and use ‘splines’ (e.g., Fermont el al., 2009);
4.	Econometrics based on the use of quantile regression analysis (e.g., Grassini et al., 2015);
5.	Stochastic frontier analysis (e.g., Silva et al., 2017);

Herewith, we focused on the ‘groups and splines’ methodological family due to the following reasons:  

•	High popularity in literature (e.g., Casanova et al.);
•	Purely statistical and comprehensible approach (Fermont et al.) of plausible implementation with a R-notebook structure.
•	Not based on ’machine learning’ methods neither crop simulation modelling which would require more complex computation.
•	Easier adoption and implementation by agronomists and scientists working on crop production or research. 

The ‘group and spline’ BLA method is defined by the following general features:

•	To identify the boundary points;
•	To fit a continuous function at these points;
•	To estimate the yield gap for each production factor;
•	To identify the most limiting factor, by analogy with von Liebig’s law of the minimum, and decompose the yield gap for each field;

The yield gap decomposition can be implemented according to the method described by Wairegi et al. (2010). This method assumes responses according to von Liebig’s law of the minimum, and identifies the minimum predicted yield (Ymin) for each field as Ymin= Min(Yx1,Yx2,...,Yxn), where Yx is the corresponding BLA predicted yield for a given X-variable. The identified yield gap (IYG) is defined as the difference between the maximum attainable yield and the Ymin. The unexplained yield gap (UYG) is defined as the difference between Ymin and observed yield. The BLA serves to rank yield-constraints and to deliver a quantitative estimation of the technical issues causing yield gaps. In locations where biotic constraints are particularly important, the BLA seems to predict yields less accurately due to the higher interactions between constraints. Therefore, only the IYG can be associated with the variation of the corresponding independent variable X, which is determined by the lowest BLA-predicted yield as defined by the law of the minimum. 

This approach has been successfully used for yield gap assessment in cereal-based systems (e.g.Casanova et al., 1999; Shatar and McBratney,2004), but also for other crops such as Cassava (Fermont et al., 2009). Cassava yields in Africa are small and it remains unclear which factors most limit yields. Using a series of farm surveys and trials in Uganda and western Kenya, Fermont el al. (2009) evaluated the importance of abiotic, biotic and associated crop management constraints for cassava production. Fermont et al. (2009) started by sorting the independent variables and removing outliers. Then, BLA was used that represent the maximum yield response (the dependent variable) to the various independent variables considered. 

Here, we aim to replicate the concept of analysis conducted by Fermont et al. (2009) on the same original dataset by developing an automated analytical algorithm in R computing language. Clear boundary lines were identified in the scatter plots relating soil fertility, soil texture, pest and disease, weed management and selected rainfall variables to cassava yield. 

**References**

Casanova, D., Goudriaan, J., Bouma, J., Epema, G.F., 1999. Yield gap analysis in relation to soil properties in direct-seeded flooded rice. Geoderma 91, 191–216.

Casanova, D., Goudriaan, J., Forner, M.M.C., Withagen, J.C.M., 2002. Rice yield prediction from yield components and limiting factors. Eur. J. Agron. 17, 41–61.

French, R.J., Schultz, J.E., 1984. Water use efficiency of wheat in a Mediterranean-type environment. I. The relation between yield, water use and climate. Aust. J. Agric. Res. 35, 743–764.

Fermont, A.M., van Asten, P.J.A., Tittonell, P., van Wijk, M.T., Giller, K.E., 2009. Closing the cassava yield gap: An analysis from smallholder farms in East Africa. Field Crops Res. 112, 24–36.

Grassini, P., Torrion, J.A., Yang, H.S., Rees, J., Andersen, D., Cassman, K.G., Specht, J.E., 2015. Soybean yield gaps and water productivity in the western U.S. Corn Belt. Field Crops Res. 179, 150–163.

Passioura, J.B., Angus, J.F., 2010. Chapter 2 - Improving Productivity of Crops in Water-Limited Environments, in: Sparks, D.L. (Ed.), Advances in Agronomy. Academic Press, pp. 37–75.

Silva, J.V., Reidsma, P., Laborte, A.G., van Ittersum, M.K., 2017. Explaining rice yields and yield gaps in Central Luzon, Philippines: An application of stochastic frontier analysis and crop modelling. Eur. J. Agron. 82, 223–241.

Shatar, T.M., Mcbratney, A.B., 2004. Boundary-line analysis of field-scale yield response to soil properties. J. Agric. Sci. 142, 553–560.

Wairegi, L.W.I., van Asten, P.J.A., Tenywa, M.M., Bekunda, M.A., 2010. Abiotic constraints override biotic constraints in East African highland banana systems. Field Crops Res. 117, 146–153.

Webb, R.A., 1972. Use of the Boundary Line in the analysis of biological data. J. Hortic. Sci. 47, 309–319.  
