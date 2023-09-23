---
title: "Why Don't Poor Families Move? A Spatial Equilibrium Analysis of Parental Decisions with Social Learning"
author: ''
date: '2023-01-15'
slug: neighborhoods
tags:
  -  Publications and working papers
summary: "In the United States, childhood neighborhood quality shapes adulthood economic opportunities. However, most children raised in bottom-quality neighborhoods still live in low-quality neighborhoods in adulthood. Could childhood neighborhood directly affect adulthood choices? I develop a quantitative spatial model of parental decisions that incorporates a novel mechanism: social learning about the technology of skill formation. Segregation generates information frictions that systematically distort parents' subjective beliefs and behavior. I calibrate the model using several United States representative datasets. The calibrated model matches targeted and non-targeted parental behavior and generates an endogenous distribution of subjective beliefs. I find a relatively modest level of delusion that increases the income Gini index by 3% and the intergenerational rank-rank slope by 12%. A housing voucher policy improves the neighborhood quality of eligible families, raising children's future earnings. When scaling up the policy, long-run and general equilibrium responses in subjective beliefs amplify the policy effects. Inequality reduces, and intergenerational mobility improves."
featured: yes
full_abstract: false
paper_link: research/neighborhoods/Bellue_JMP_Neighborhoods.pdf
links:
/*- icon: 
  icon_pack: fa
  name: working paper
  url: research/neighborhoods/Bellue_JMP_Neighborhoods.pdf€÷
show_post_date: false
show_links: yes
images:
  - ../../img/nbh.png
---

Parents' neighborhood choices shape children’s economic opportunities in the United States. But, most children raised in bottom-quality neighborhoods still live in low-quality neighborhoods in adulthood. 

<div>                        
        <script type="text/javascript">window.PlotlyConfig = {MathJaxConfig: 'local'};</script>
         <script src="../../js/matrixmobData11.js"  ></script>                
        <div id="d1b212c1-b722-400f-b05f-8ee77950a910" class="plotly-graph-div" style="height:100%; width:100%;"></div>           
         <script src="../../js/matrixmobData21.js" ></script>           
        <div style="text-align: justify;" class="f7"> Note: Probability of moves conditionnal on childhood neighborhood quality. Quality is proxied by census tract household median income. Each neighborhood represents a decile of the census tract quality distribution. Almost half of the children raised in the bottom-decile of the neighborhood quality distribution live in the bottom-quintile of the neighbohood quality distibution in adulhood. </div>
        <div style="text-align: right;" class="f7"> Source: AddHealth</div>
    </div>


Do parents' neighborhood choices also affect their children's future choices?

I propose a novel mechanism to help understand parents' decisions across generations and socioeconomic groups: social learning about the technology of skill formation in the neighborhood. 


<table>
<caption>Social Learning in the Neighborhood</caption>
<tr><td><div class="f6"> Consider a world in which success depends on parental inputs -neighborhood quality and parental time- and ability shocks -which can be interpreted to some extent as luck. 

Information is imperfect; people are unaware of the returns to parental inputs and must learn about them. Young adults learn by observing older adults in their neighborhoods (social learning). They see average local successes and past parental inputs but only perceive their neighbors' ability shocks. 

Young adults' inference of the returns crucially depends on the accuracy of their perception. If they underestimate local ability shocks, they implicitly attribute too little of the local successes to those shocks and too much to parental inputs: they become over-optimistic about the returns to parental inputs. Conversely, if they overestimate them, they become pessimistic about the returns.

Ability shock perceptions are unbiased but bounded, which leads to moderate perceptions of ability shocks. Therefore, the larger the ability shocks in a given neighborhood, the more young adults underestimate local ability shocks and become over-optimistic. Conversely, the smaller the ability shocks in a given neighborhood, the more young adults overestimate local ability shocks and become pessimistic.  

With residential income segregation --a form of spatial sorting partly based on ability shocks--, persistent delusion arises endogenously. In high-quality neighborhoods, live, on average, over-optimistic and wealthy parents with high-ability shocks. Their children become over-optimistic and tend to stay. In low-quality neighborhoods live, on average, pessimistic and low-income parents with low-ability shocks. Their children become pessimistic and tend to stay.</div ></td></tr>
</table>




I depart from the perfect information assumptions and develop a quantitative spatial model of parental decisions in which I incorporate the novel mechanism: social learning about the returns to parental inputs.
In the model, segregation generates information frictions that systematically distort parents' subjective beliefs and behavior.

Using several United States representative datasets, I calibrate the model to the average commuting zone in the country. The calibrated model matches targeted and non-targeted parental behavior and generates an endogenous distribution of subjective beliefs.


<div>                        
        <script type="text/javascript">window.PlotlyConfig = {MathJaxConfig: 'local'};</script>
        <script src="../../js/matrixmobModel12.js"></script>                
        <div id="fe863b8b-acc1-4457-897f-08497b532913" class="plotly-graph-div" style="height:450px; width:100%;"></div>            
        <script src="../../js/matrixmobModel22.js"></script> 
      <div style="text-align: justify;" class="f7"> Note: Model generated probability of moves conditionnal on childhood neighborhood quality. Each neighborhood represents a decile of the census tract quality distribution in the data. In the model too, almost half of the children raised in the bottom-decile of the neighborhood quality distribution live in the bottom-quintile of the neighbohood quality distibution in adulhood. </div>
         <div style="text-align: right;" class="f7"> Source: Model generated data</div>
  </div>   
    

The model generates a relatively modest delusion level --consistent with micro-studies-- that significantly affects the economy. Delusion is asymmetric across the income distribution. Under perfect information, low-income parents' perceived returns would be 17% higher while those of high-income parents would be 7% lower. This deviation from perfect information has large effects on the american dream. Under perfect information, inequality would be 3% lower and social mobility 12% higher.


<table class="f6  mw7" stye="max-width: 100%;display: flex;">
<caption>Effects of Social Learning - Changes Due to Perfect Information Relative to Baseline Model</caption>
  <tr>
  	<th></th>
    <th></th>
    <th></th>
    <th colspan="3">Income Quartile</th>
  </tr>
  <tr>
  	<th></th>
    <th>All</th>
    <th>1st</th>
    <th>2nd</th>
    <th>3rd</th>
    <th>4th</th>
  </tr>
  <tr>
    <td>Perceived Returns</td>
    <td>+3%</td>
    <td>+17%</td>
    <td>+6%</td>
    <td>0%</td>
    <td>-7%</td>
  </tr>
    <tr>
    <td>Parental Time</td>
    <td>+7%</td>
    <td>+31%</td>
    <td>+10%</td>
    <td>+3%</td>
    <td>-5%</td>
  </tr>
      <tr>
    <td>Social Mobility</td>
    <td>+12%</td>
    <td></td>
    <td></td>
    <td></td>
     <td></td>
  </tr>
  <tr>
    <td>Inequality</td>
    <td>-3%</td>
    <td></td>
    <td></td>
    <td></td>
     <td></td>
  </tr>
      <tr>
    <td>Poverty</td>
    <td>-17%</td>
    <td></td>
    <td></td>
    <td></td>
     <td></td>
  </tr>
</table>
<div style="text-align: right; margin-top:-30px;" class="f7 mt0"> Source: Model generated data</div>

Segregation distortion effects motivate a government intervention. I use the calibrated model to evaluate a housing voucher policy. In line with empirical evidence, the model predicts that housing vouchers improve the neighborhood quality of eligible families, raising children's future earnings. When scaling up the policy, general equilibrium responses in local prices and subjective beliefs amplify the effects on eligible households, reducing inequality and improving social mobility. However, ignoring the change in the information frictions significantly undermines the housing voucher policy effects.


<table class="f6  mw7" stye="max-width: 100%;display: flex;">
<caption>Effects of a Housing Voucher Policy</caption>
  <tr>
  	<th></th>
    <th></th>
    <th></th>
    <th></th>
    <th colspan="3">Income Quartile</th>
  </tr>
  <tr>
  	<th></th>
  	<th></th>
    <th>All</th>
    <th>1st</th>
    <th>2nd</th>
    <th>3rd</th>
    <th>4th</th>
  </tr>
  <tr>
    <td rowspan=5>Baseline Model</td>
    <td >Perceived Returns</td>
    <td>+2.8%</td>
    <td>+7.1%</td>
    <td>+3.3%</td>
    <td>+2.2%</td>
    <td>+0.2%</td>
  </tr>
  <tr>
    <td>Parental Time</td>
    <td>+2.6%</td>
    <td>+8.0%</td>
    <td>+2.2%</td>
    <td>+1.2%</td>
    <td>+1.3%</td>
  </tr>
  <tr>
    <td>Social Mobility</td>
    <td>+3.8%</td>
    <td></td>
    <td></td>
    <td></td>
     <td></td>
  </tr>
  <tr>
    <td>Inequality</td>
    <td>-0.8%</td>
    <td></td>
    <td></td>
    <td></td>
     <td></td>
  </tr>
  <tr>
    <td>Poverty</td>
    <td>-6.3%</td>
    <td></td>
    <td></td>
    <td></td>
     <td></td>
  </tr>
  <tr>
  	<td rowspan=5>Ignoring Information Friction Change</td>
  	<td >Perceived Returns</td>
    <td>-0.0%</td>
    <td>+0.5%</td>
    <td>-0.2%</td>
    <td>-0.2%</td>
    <td>+0.0%</td>
  </tr>
  <tr>
    <td>Parental Time</td>
    <td>-1.2%</td>
    <td>-1.6%</td>
    <td>-2.4%</td>
    <td>-1.5%</td>
    <td>+0.8%</td>
  </tr>
  <tr>
    <td>Social Mobility</td>
    <td>-0.5%</td>
    <td></td>
    <td></td>
    <td></td>
     <td></td>
  </tr>
  <tr>
    <td>Inequality</td>
    <td>+0.0%</td>
    <td></td>
    <td></td>
    <td></td>
     <td></td>
  </tr>
    <tr>
    <td>Poverty</td>
    <td>+1.3%</td>
    <td></td>
    <td></td>
    <td></td>
     <td></td>
  </tr>
</table>
<div style="text-align: right; margin-top:-30px;" class="f7"> Source: Model generated data</div>
