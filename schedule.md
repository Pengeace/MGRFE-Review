
# Questions

---
**Five star:**

## Reviewer1:

4.
> What is the rationale for using particularly t-test first and then MIC? Can any combination of other two filter methods be used in search space reduction task? Clarify in detail. Use any other combination of two filter methods and compare it to the proposed combination of t-test and MIC-based search space reduction.

5.
> The researchers have used t-test and then MIC. The gene selected after MIC is used in the proposed MGRFE algorithm. In table 5, why the t-test-based gene ranking has been compared? MIC based ranking should also be compared.

7.
> The comparative results of SRBCT, ALL-AML and ALL have been shown in table 7, 8 and 9. However, the tables are very similar to work in kar et al. [28]. The similar type of comparison should be given for all the dataset used i.e. 19 dataset in the present work.

8(description). 
> The proposed work has also been compared with Kar et al. [28] in computational performance. Kar et al. have applied a swarm intelligence-based method to the space of all genes. They have not reduced the search space prior to the optimization task. In contrast, the proposed method have applied MGRFE technique on the reduced search space. The reduce search space have been constructed by t-test and then by MIC technique. In my opinion the search space reduction is fixed. It is done once before the application of MGRFE. In that regard, the comparison of computational time would not significant because it has been computed in the reduced search space. The genes outside the reduced search space could carry valuable information towards classification accuracy.

## Reviewer2:

3. 
> The authors claim to compare their method on 17 data sets.  But I did not see any evidence that the finally determined feature set is validated on an independent data set of the same form of cancer for example.  All that the authors have done is five-fold cross-validation within the same data set.  Without this sort of validation on an independent data set, the claimed performance figures by themselves are not very persuasive.  This is because cross-validation within the same data set does not take into account factors such as batch effect, platform variation, and the like.

6.
> In Section 2.3.1 the authors use the T-test and MIC to achieve a first-cut reduction in the feature set.  I have found that using the so-called "volcano plot," which combines the T-test with a fold-change criterion, works better than just the T-test alone.

2(description).
> The paper is a mixture of techniques that are by now standard in the world of computational biology.  Given a very large number of features, first use some pre-filtering to eliminate perhaps 90% to 95% of the features, and then use recursive feature elimination (RFE) on the remaining features.  I could not find any compelling evidence that the proposed approach is superior to the existing methods.

4(description). 
> The authors' preferred method of genetic algorithms is known to lack theoretical foundations, to be very sensitive to various parameters in the algorithm, and to be extremely time consuming.  In contrast, the original paper where RFE was proposed, by Isabel Guyon, used the support vector machine (SVM) which is very fast and for which lots of theoretical results are available.  This is another reason for my not being overly enthusiastic about the paper.

---

**Three star:**

## Reviewer1

1.	
> In the introduction section author has mentioned the phrase "lack an explicit decline of the feature number". The particular phrase is not clear. Please elaborate and explain clearly the lacuna of swarm intelligence based gene selection approach.

2. 
> In algorithm 1, it has been mentioned to sort the optimal gene combination in GC and to preserve the top ranked genes. On what basis the top ranked gene would be sorted?  For sorting what procedure is used?

3. 
> In the search space reduction stage, it has been mentioned that top 1000 genes have been selected by a threshold of 0.05 in t-test technique and thereafter MIC has been applied on the 1000 genes to re-rank them. Is there any particular reason of selection 0.05 value as threshold? Is there any mathematical reason for selecting particularly this value for threshold in t-test? Or it has been selected experimentally and any other value can also be chosen? Clarify in detail.

6. 
> Elaborate the significance of '0' ranked gene in t-test.

9. 
> In the Conclusion section, the authors will need to clearly address the research contributions in theory. The research contributions in theory must be fully stated in at least one paragraph.

10.
> In the Conclusion section, the authors need to fully discuss insightful and practical implications. 

## Reviewer2

1. 
> First of all, the paper is described as "Survey/Tutorial," but it appears to describe a claimed original contribution by the authors, namely the MGRFE algorithm.  The proposed new algorithm is compared against several existing algorithms.  Therefore, if at all the paper is to be published, it should be as a regular research paper, and not as a survey/tutorial paper.

5. 
> There are several places where the authors do not appear to be aware of simple statistical facts.  For instance, the accuracy is a weighted average of the sensitivity and the specificity.  But the authors talk as though they are independent parameters.  Equation (1) in the right column of page 1 is too wide.
