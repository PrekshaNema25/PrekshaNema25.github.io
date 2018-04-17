<head>
<title> Preksha Nema </title>
</head>

# About Me
<div style = "text-align: justify"> I am currently pursuing my Ph.D. under Dr. Mitesh M. Khapra and co-guided by Dr. Balaraman Ravindran at IIT Madras. I joined IIT Madras as an M.Tech in July 2015, and then converted to Ph.D. programme in March 2017. My area of research is Deep learning for NLP. Currently my work is focussed on modelling better attention mechanism techniques for different Natural Language Generation tasks.
</div>

# Awards
Google India Ph.D. Fellowship, 2017

# Publications
<table width="100%" align="center" border="0" cellspacing="0">
 <tr>
  <td width ="100%" colspan="2">
    <h3>ElimiNet: A Model for Eliminating Options for Reading Comprehension with Multiple Choice Questions</h3>
    <font color="grey"><h5><i><b>  International Joint Conference on Artificial Intelligence (IJCAI), 2018</b></i></h5></font>
   <font color="black"><h5> Soham Parikh, Ananya Sai, Preksha Nema, Mitesh M Khapra </h5></font>
    </td>
   </tr>
 <tr>
      <td width="30%">
      <img src='/images/eliminet.png'>         
      </td>
      <td valign="top" width="70%"> 
        <div style = "text-align: justify"> <h6>  The task of Reading Comprehension with Multiple Choice Questions, requires a human (or machine) to read a given *{passage, question}* pair and select one of the *n* given options. The current state of the art model for this task first computes a query-aware representation for the passage and then *selects* the option which has the maximum similarity with this representation. However, when humans perform this task they do not just focus on option selection but use a combination of *elimination* and *selection*. This process could be repeated multiple times till the reader is finally ready to select the correct option. We propose *ElimiNet*, a neural network based model which tries to mimic this process. Specifically, it has gates which decide whether an option can be eliminated given the {*passage, question*} pair and if so it tries to make the passage representation orthogonal to this eliminated option (akin to ignoring portions of the passage corresponding to the eliminated option). The model makes multiple rounds of partial elimination to refine the passage representation and finally uses a selection module to pick the best option. </h6></div></td></tr>
 <tr>
  <td width ="100%" colspan="2">
    <h3>Generating Descriptions from Structured Data Using a Bifocal Attention Mechanism and Gated Orthogonalization</h3>
    <font color="grey"><h5><i><b> North American Chapter of the Association for Computational Linguistics (NAACL), 2018</b></i></h5></font>
   <font color="black"><h5> Preksha Nema, Shreyas Shetty M, Parag Jain, Anirban Laha, Karthik Sankaranarayanan and Mitesh M. Khapra </h5></font>
    </td>
   </tr>
 <tr>
      <td width="30%">
      <img src='/images/nlb.jpg'>         
      </td>
      <td valign="top" width="70%"> 
        <div style = "text-align: justify"> <h6> In this work, we focus on the task of generating natural language descriptions from a structured table of facts containing fields (such as nationality, occupation, etc) and values (such as Indian, {actor, director}, etc). One simple choice is to treat the table as a sequence of fields and values and then use a standard seq2seq model for this task. However, such a model is too generic and does not exploit task specific characteristics. For example, while generating descriptions from a table, a human would attend to information at two levels: (i) the fields (macro level) and (ii) the values within the field (micro level). Further, a human would continue attending to a field for a few timesteps till all the information from that field has been rendered and then never return back to this field (because there is nothing left to say about it). To capture this behavior we use (i) a fused bifocal attention mechanism which exploits and combines this micro and macro level information and (ii) a gated orthogonalization mechanism which tries to ensure that a field is remembered for a few timesteps and then forgotten.  We experiment with a recently released dataset which contains fact tables about people and their corresponding one line biographical descriptions in English. </h6></div>
        <ul>
        <li><a href="https://github.com/PrekshaNema25/StructuredData_To_Descriptions"> [Data + Code] </a></li>
        </ul></td></tr>
 <tr>
   <tr>
  <td width ="100%" colspan="2">
    <h3>A Mixed Hierarchical Attention based Encoder-Decoder Approach for Standard Table Summarization</h3>
    <font color="grey"><h5><i><b> North American Chapter of the Association for Computational Linguistics (NAACL), 2018 (Short Papr) </b></i></h5></font>
   <font color="black"><h5> Parag Jain, Anirban Laha, Karthik Sankaranarayanan and Preksha Nema, Mitesh M. Khapra and  Shreyas Shetty </h5></font>
    </td>
   </tr>
 <tr>
      <td width="30%">
      <img src='/images/table2text.png'>         
      </td>
      <td valign="top" width="70%"> 
        <div style = "text-align: justify"> <h6> Structured data summarization involves generation of natural language summaries from structured input data. In this work, we consider summarizing structured data occurring in the form of tables as they are prevalent across a wide variety of domains. We formulate the standard table summarization problem, which deals with tables conforming to a single predefined schema. To this end, we propose a mixed hierarchical attention based encoder-decoder model which is able to leverage the structure in addition to the content of the tables. Our experiments on the publicly available weathergov dataset show around 18 BLEU  improvement over the current state-of-the-art. </h6></div>
</td></tr>
<tr>
  <td width ="100%" colspan="2">
    <a href="https://arxiv.org/abs/1704.08300"><h3>Diversity driven Attention Model for Query-based Abstractive Summarization</h3></a><font color="grey"><h5><i><b> Association of Computational Linguistics (ACL), 2017</b></i></h5></font>
   <font color="black"><h5> Preksha Nema, Mitesh M. Khapra, Anirban Laha, Balaraman Ravindran </h5></font>
    </td>
  
   </tr>
 <tr>
      <td width="30%">
      <img src='/images/query.png'>         
      </td>
      <td valign="top" width="70%"> 
        <div style = "text-align: justify"> <h6> Abstractive summarization aims to generate a shorter version of the document covering all the salient points in a compact and coherent fashion. On the other hand, query-based summarization highlights those points that are relevant in the context of a given query. The encode-attend-decode paradigm has achieved notable success in machine translation, extractive summarization, dialog systems, etc. But it suffers from the drawback of generation of repeated phrases. In this work we propose a model for the query-based summarization task based on the encode-attend-decode paradigm with two key additions (i) a query attention model (in addition to document attention model) which learns to focus on different portions of the query at different time steps (instead of using a static representation for the query) and (ii) a new diversity based attention model which aims to alleviate the problem of repeating phrases in the summary. In order to enable the testing of this model we introduce a new query-based summarization dataset building on debatepedia. Our experiments show that with these two additions the proposed model clearly outperforms vanilla encode-attend-decode models with a gain of 28\% (absolute) in ROUGE-L scores.</h6></div>
        <ul>
        <li><a href="https://github.com/PrekshaNema25/diversity_based_attention"> [Data + Code] </a></li>
        </ul></td></tr>
 </table>


   
# Work Experience
I worked in Nvidia Graphics Pvt. Ltd. from June 2012 - June 2015 as a System Software Engineer in Resource Manager- Professional Soultions Group team.

# Academic Details
I have completed my B.Tech from Visvesvaraya National Institute of Technology, Nagpur in Computer Science and Engineering in 2012.

# Contact:

[Resume](pdfs/resume.pdf)

preksha [at] cse[dot]iitm[dot]ac[dot]in
