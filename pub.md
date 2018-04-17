<table width="100%" align="center" border="0" cellspacing="0">
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
        <div style = "text-align: justify"> <h6> In this work, we focus on the task of generating natural language descriptions from a structured table of facts containing fields (such as nationality, occupation, etc) and values (such as Indian, {actor, director}, etc). One simple choice is to treat the table as a sequence of fields and values and then use a standard seq2seq model for this task. However, such a model is too generic and does not exploit task specific characteristics. For example, while generating descriptions from a table, a human would attend to information at two levels: (i) the fields (macro level) and (ii) the values within the field (micro level). Further, a human would continue attending to a field for a few timesteps till all the information from that field has been rendered and then never return back to this field (because there is nothing left to say about it). To capture this behavior we use (i) a fused bifocal attention mechanism which exploits and combines this micro and macro level information and (ii) a gated orthogonalization mechanism which tries to ensure that a field is remembered for a few timesteps and then forgotten.  We experiment with a recently released dataset which contains fact tables about people and their corresponding one line biographical descriptions in English. In addition, we also introduce two similar datasets for French and German. Our experiments show that the proposed model gives 21% relative improvement over a recently proposed state of the art method and 10% relative improvement over basic seq2seq models. The code and the datasets developed as a part of this work will be made publicly available.</h6></div>
        <ul>
        <li><a href="https://github.com/PrekshaNema25/StructuredData_To_Descriptions"> [Data + Code] </a></li>
        </ul></td></tr>
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
