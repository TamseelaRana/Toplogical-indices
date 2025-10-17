We have selected the first Zagreb index M_1   as the primary topological descriptor for computing the triangular membership function. By applying the fuzzy triangular membership function to the normalized M_1  values, we aim to classify molecular structures into low, medium and high feature categories, enabling a nuanced and interpretable analysis of molecular behavior as seen in Table 4. Let M_1  = {312, 252, 458, 400, 376, 458, 324, 280, 190, 372, 286, 232, 290, 214, 256, 278, 400, 352, 212, 362} be a set of real values.

Step 1: Normalize M_1  Values

We use min-max normalization to scale the values of  M_1   to the range [0, 1]. The formula for normalization is :
m_i^norm = (m_i- min(M_1) )/(max(M_1 )- min(M_1) )
Where:
	min(M_1) = 190 
	max(M_1) = 458 

We compute the normalized values for the first two values as follows:

For  m_1= 312 :

m_1^norm = (312- 190 )/(458- 190 ) = 0.4552

For  m_(2 )= 252 :

m_2^norm =  (252- 190 )/(458- 190 )  = 0.2313

Step 2: Compute the Mean for Triangular Membership Functions

The mean of the normalized values is calculated as:

μ = (1 )/(20 )  ∑_(i=1)^20▒〖m_i^(norm   )≈〗 0.5037

We use this mean as the midpoint for the triangular membership functions.

 Step 3: Define Triangular Membership Functions

For each membership function (Low, Medium, High), we use the following formulations which is given in 1.2 Primary section:

Step 4: Apply Membership Functions to First Two Normalized Values

For m_1^norm  = 0.4552 :

	μ_Low (0.4552) = 0.0963

	μ_Med (0.4552) = 0.9037

	μ_High   (0..4552) = 0.0000 

For m_2^norm  = 0.2313 :

	μ_Low (0.2313) =  (0.5037 - 0.2313 )/(0.5037 )  ≈  0.5407

	μ_Med (0.2313) =  (0.2313  - 0)/(0.5037 )  ≈   0.4593 

	μ_High (0.2313) = 0

 Step 5: Final Output Table

Table 4: The normalized M_1   values and compute their corresponding Low, Medium and High membership function values.


m_i m_i^norm  μ_Low (m_i^norm)	μ_Med (m_i^norm)	μ_High (m_i^norm)
312 0.4552	0.0963	              0.9037	           0.0000
252	0.2313	0.5407	              0.4593	           0.0000
458	1.0000	0.0000	              0.0000	           1.0000
400	0.7836	0.0000	              0.4361	           0.5639
376	0.6940	0.0000	              0.6165               0.3835
458	1.0000	0.0000	              0.0000	           1.0000
428	0.8881	0.0000	              0.2256	           0.7744
280	0.3358	0.3333	              0.6667	           0.0000
190	0.0000	1.0000	              0.0000	           0.0000
372	0.6791	0.0000	              0.6466	           0.3534
286	0.3582	0.2889	              0.7111	           0.0000
232 0.1567  0.6645             	  0.3355           	   0.0000
290	0.3731	0.2593	              0.7407	           0.0000
214	0.0896	0.8222	              0.1778	           0.0000
256	0.2463	0.5111	              0.4889	           0.0000
278	0.3284	0.3481	              0.6519	           0.0000
400	0.7836	0.0000	              0.4361	           0.5639
352	0.6045	0.0000	              0.7970	           0.203
212	0.0821	0.8370	              0.1630	           0.0000
362	0.6418	0.0000	              0.7218	           0.2782

