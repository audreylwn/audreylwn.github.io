---
layout: archive
title: Peer-reviewed Publications
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% assign pubs = site.data.publications | sort: 'year' | reverse %}
{% assign years = pubs | map: 'year' | uniq %}

{% for year in years %}

### {{ year }}

{% for pub in pubs %}
  {% if pub.year == year %}

  {% assign has_link = pub.url != nil and pub.url != '' %}
  <p style="margin: 0.4em 0 0.2em 0; font-size: 0.9em">
    {% if has_link %}
      🔗 <a href="{{ pub.url }}" style="text-decoration: none; color: inherit;"><strong>{{ pub.title }}</strong></a>
    {% else %}
      <strong>{{ pub.title }}</strong>
    {% endif %}
  </p>
  <p style="margin-top: 0; font-size: 0.9em;">
    {{ pub.authors }}.<br/>
    <em>{{ pub.venue }}.</em>
    {% if pub.notes %}<br/>{{ pub.notes }}{% endif %}
  </p>

  {% endif %}
{% endfor %}

{% endfor %}


<!-- ---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}


## Peer-reviewed publications

* Burke J, Gibbon S, **Low A**, Hamid C, Reid-Schachter M, Muniz-Terrera G, Ritchie CW, Dhillon B, O’Brien JT, MacCormick IJC, MacGillivray TJ. Association between choroidal microvasculature in the eye and Alzheimer’s disease risk in cognitively healthy midlife adults. Alzheimer’s Dement. 2025;17:e70075. [[doi](http://dx.doi.org/10.1002/dad2.70075)] 
* **Low A**, McKiernan E, Prats-Sedano MA, Carter SF, Stefaniak JD, Su L, Dounavi ME, Muniz-Terrera G, Jenkins N, Bridgeman K, Ritchie K, Lawlor B, Naci L, Malhotra P, Mackay C, Koychev I, Thayanandan T, Raymont V, Ritchie CW, Stewart W, O’Brien JT. Neuroimaging and Clinical Findings in Healthy Middle-Aged Adults With Mild Traumatic Brain Injury in the PREVENT Dementia Study. JAMA Netw Open. 2024 Aug 1;7(8):e2426774. [[doi](http://dx.doi.org/10.1001/jamanetworkopen.2024.26774)] [[Scientific American](https://www.scientificamerican.com/article/concussions-are-remarkably-common-and-can-cause-long-term-problems/)]
* **Low A**, van Winden S, Cai L, Kessels RPC, Maas MC, Morris R, Nus M, Tozer DJ, Tuladhar AM, van der Kolk A, Wolters R, Mallat Z, Riksen NP, Markus HS, de Leeuw FE. Immune regulation and blood–brain barrier permeability in cerebral small vessel disease: study protocol of the INflammation and Small Vessel Disease (INSVD) study – a multicentre prospective cohort study. BMJ Open. 2024; 0:e084303. [[doi](http://dx.doi.org/10.1136/bmjopen-2024-084303)] (co-first authorship)
* Gibbon S, **Low A**, Hamid C, Reid-Schachter M, Muniz-Terrera G, Ritchie CW, Trucco E, Dhillon B, O'Brien JT, MacGillivray TJ. Association of optic disc pallor and RNFL thickness with cerebral small vessel disease in the PREVENT-Dementia study. Alzheimers Dement. 2024; 16(3):e12633. [[doi](http://dx.doi.org/10.1002/dad2.12633)]
* Mak E, Dounavi ME, Operto G, Ziukelis E, Jones PS, **Low A**, Swann P, Newton C, Terrera-Muniz G, Malhotra P, Koychev I, Falcon C, Mackay C, Lawlor B, Naci L, Wells K, Ritchie C, Ritchie K, Su L, Gispert JD, O'Brien JT. Apoe ε4 exacerbates age-dependent deficits in cortical microstructure in midlife adults. Brain Comms. 2024; accepted on 09 Feb 2024. [[doi](http://dx.doi.org/10.1093/braincomms/fcad351)]
* Buller-Peralta I, Gregory S, **Low A**, Dounavi ME, Wells K, Ntailianis G, Lawlor B, Naci L, Koychev I, Malhotra P, O’Brien JT, Ritchie CW, Muniz-Terrera G. Comprehensive allostatic load risk index is associated with increased frontal and left parietal white matter hyperintensities in mid-life cognitively healthy adults. Sci Rep. 2024; 14:573. [[doi](http://dx.doi.org/10.1038/s41598-023-49656-3)]
* Gregory S, Buller-Peralta I, De La Cruz Góngara V, Dounavi ME, **Low A**, Ntailianis G, Parra M, Ritchie CW, Ritchie K, Shannon OM, Stevenson EJ, Wells K, Muniz-Terrera G. The Mediterranean diet is not associated with neuroimaging or cognition in middle-aged adults: a cross-sectional analysis of the PREVENT Dementia Programme. Eur J Neurol. 2024; 31:e16345. [[doi](http://dx.doi.org/10.1111/ene.16345)]
* Ritchie CW, Bridgeman K, Gregory S, O’Brien JT, Danso SO, Dounavi ME, Carriere I, Driscoll D, Hillary R, Koychev I, Lawlor B, Naci L, Su L, **Low A**, Mak E, Malhotra P, Manson J, Marioni R, Murphy L, Stewart W, Muniz-Terrera G, & Ritchie K. The PREVENT Dementia programme: Baseline demographic, lifestyle, imaging and cognitive data from a midlife cohort study investigating risk factors for dementia. Brain Commun. 2024; 6(3):fcae189. [[doi](http://dx.doi.org/10.1093/braincomms/fcae189)]
* Dounavi ME, Mak E, Swann P, **Low A**, Muniz-Terrera G, McKeever A, Pope M, Williams G, Wells K, Lawlor B, Naci L, Malhotra P, MacKay C, Koychev I, Ritchie K, Su L, Ritchie C, O’Brien J. Differential association of cerebral blood flow and anisocytosis in APOE ε4 carriers at midlife. J Cereb Blood Flow Metab. 2023; 43(10):1672-1684. [[doi](http://dx.doi.org/10.1177/0271678X231173587)]
* Borchet R, Azevedo T, Badhwar A, Bernal J, Betts M, Bruuffaerts R, Bukhart M, Dewachter L, Gellersen H, **Low A**, …, Newby D, Ranson J, Llewellyn D, Veldsman M, Rittman T. Artificial intelligence for diagnosis and prognosis in neuroimaging for dementia; a systematic review. Alzheimer’s Dement. 2023; 1-20. [[doi](http://dx.doi.org/10.1002/alz.13412)] 
* **Low A**, Prats-Sedano M, McKiernan E, Carter S, Stefaniak JD, Nannoni S, Su L, Dounavi ME, Muniz-Terrera G, Ritchie K, Lawlor B, Naci L, Malhotra P, MacKay C, Koychev I, Ritchie CW, Markus HS, O’Brien JT. Modifiable and non-modifiable risk factors of dementia and midlife cerebral small vessel disease in cognitively healthy midlife adults: the PREVENT-Dementia study. Alz Res Therapy. 2022; 14:154. [[doi](http://dx.doi.org/10.1186/s13195-022-01095-4)]
* **Low A**, Prats-Sedano MA, Stefaniak JD, McKiernan EF, Carter SF, Dounavi ME, Mak E, Su L, Stupart O, Muniz-Terrera G, Ritchie K, Ritchie CW, Markus HS, O'Brien JT. CAIDE dementia risk score relates to severity and progression of cerebral small vessel disease in healthy midlife adults: the PREVENT-Dementia study. J Neurol Neurosurg Psychiatry. 2022; 93:481-490. [[doi](http://dx.doi.org/10.1136/jnnp-2021-327462)]
* Dounavi ME, **Low A**, Muniz-Terrera G, Ritchie K, Ritchie CW, Markus HS, O'Brien JT. Fluid-Attenuated Inversion Recovery MRI textural features as sensitive markers of white matter damage in midlife adults. Brain Commun. 2022; 4(3): fcac116. (co-first authorship) [[doi](http://dx.doi.org/10.1093/braincomms/fcac116)]
* Dounavi ME, Newton C, Jenkins N, Mak E, **Low A**, Muniz-Terrera G, Williams GB, Lawlor B, Naci L, Malhotra P, Mackay C, Koychev I, Ritchie K, Ritchie CW, Su L, O'Brien JT. Macrostructural brain alterations at midlife are connected to cardiovascular and not inherited risk of future dementia. J Neurol. 2022; 269(8):4299-4309. [[doi](http://dx.doi.org/10.1007/s00415-022-11061-7)]
* **Low A**, Su L, Stefaniak JD, Mak E, Dounavi ME, Muniz-Terrera G, Ritchie K, Ritchie CW, Markus HS, O'Brien JT. Inherited risk of dementia and the progression of cerebral small vessel disease and inflammatory markers in cognitively healthy midlife adults: the PREVENT-Dementia study. Neurobiol Aging. 2021; 98:124-133. [[doi](https://doi.org/10.1016/j.neurobiolaging.2020.10.029)]
* Brown R, **Low A**, Markus HS. Rate of, and risk factors for, white matter hyperintensity growth: a systematic review and meta-analysis with implications for clinical trial design. J Neurol Neurosurg Psychiatry. 2021; 92(12):1271-1277. [[doi](https://doi.org/10.1136/jnnp-2021-326569)]
* Dounavi ME, **Low A**, McKiernan E, Mak E, Muniz-Terrera G, Ritchie K, Ritchie CW, Su L, O'Brien JT. Evidence of cerebral hemodynamic dysregulation in middle-aged APOE ε4 carriers: the PREVENT-Dementia study. J Cereb Blood Flow Metab. 2021; 41(11):2844-2855. [[doi](https://doi.org/10.1177/0271678X211020863)]
* Mak E, Dounavi M, **Low A**, Carter SF, McKiernan E, Williams GB, Jones PS, Carriere I, Muniz-Terrera G, Ritchie K, Ritchie C, Su L, O’Brien JT. Proximity to dementia onset and multi-modal neuroimaging changes: The PREVENT-Dementia Study. NeuroImage. 2021;229:117749. [[doi](https://doi.org/10.1016/j.neuroimage.2021.117749)]
* Mak E, Holland N, Jones PS, Savulich G, **Low A**, Malpetti M, Kaalund SS, Passamonti L, Rittman T, Romero-Garcia R, Manavaki R, Williams GB, Hong YT, Fryer TD, Aigbirhio FI, O’Brien JT, Rowe JB. In vivo coupling of dendritic complexity with presynaptic density in primary tauopathies. Neurobiol Aging 2021; 101: 187–198. [[doi](https://doi.org/10.1016/j.neurobiolaging.2021.01.016)]
* Vipin A, Wong BYX, Kumar D, **Low A**, Ng KP, Kandiah N. Association between white matter hyperintensity load and grey matter atrophy in mild cognitive impairment is not unidirectional. Aging (Albany NY) 2021;13(8): 10973–10988. [[doi](https://doi.org/10.18632/aging.202977)]
* **Low A**, Mak E, Malpetti M, Passamonti L, Nicastro N, Stefaniak JD, Savulich G, Chouliaras L, Su L, Rowe JB, Markus HS, O’Brien JT. In vivo neuroinflammation and cerebral small vessel disease in mild cognitive impairment and Alzheimer’s disease. J Neurol Neurosurg Psychiatry. 2020; 11; 92(1): 45-52. [[doi](https://doi.org/10.1136/jnnp-2020-323894)]
* **Low A**, Mak E, Stefaniak JD, Malpetti M, Nicastro N, Markus HS, Rowe JB, O’Brien JT. Peak Width of Skeletonized Mean Diffusivity as a Marker of Diffuse Cerebrovascular Damage. Front Neurosci. 2020; 14: 238. [[doi](https://doi.org/10.3389/fnins.2020.00238)]
* Wong FCC, Yatawara C, **Low A**, Foo H, Wong BYX, Lim L, Wang B, Kumar D, Ng KP, Kandiah N. Cerebral Small Vessel Disease Influences Hippocampal Subfield Atrophy in Mild Cognitive Impairment. Transl Stroke Res. 2020, 1-9. [[doi](https://doi.org/10.1007/s12975-020-00847-4)]
* Koh W, Lim L, **Low A**, Wong B, Lim L, Silva E, Ng KP, Kandiah N. Development and validation of a brief visual based cognitive screening tool for dementia: the Visual Cognitive Assessment Test short-form (VCAT-S). J Neurol Neurosurg Psychiatry. 2020; 91(10): 1122-1123. [[doi](https://doi.org/10.1136/jnnp-2020-323106)]
* **Low A**, Mak E, Rowe JB, Markus HS, O’Brien JT. Inflammation and cerebral small vessel disease: A systematic review. Ageing Res Rev. 2019; 53:100916. [[doi](https://doi.org/10.1016/j.arr.2019.100916)]
* **Low A**, Ng KP, Chander RJ, Wong B, Kandiah N. Association of Asymmetrical Distribution of White Matter Hyperintensities and Apolipoprotein E4 on Cognitive Outcomes in Mild Cognitive Impairment and Dementia. J Alzheimers Dis. 2019; 70(3): 953-964. [[doi](https://doi.org/10.3233/JAD-190159)]
* **Low A**, Mak E, Malpetti M, Chouliaras L, Nicastro N, Su L, Holland N, Rittman T, Vázquez Rodríguez P, Passamonti L, Bevan-Jones WR, Jones PS, Rowe JB, O'Brien JT. Asymmetrical Atrophy of Thalamic Subnuclei in Alzheimer’s Disease and Amyloid-Positive Mild Cognitive Impairment is Associated with Key Clinical Features. Alzheimers Dement (Amst). 2019; 11: 690-699. [[doi](https://doi.org/10.1016/j.dadm.2019.08.001)]
* **Low A**, Foo H, Yong T, Tan LCS, Kandiah N. Hippocampal Subfield Atrophy of CA1 and Subicular Structures Predict Progression to Dementia in Idiopathic Parkinson’s disease. J Neurol Neurosurg Psychiatry. 2019; 90(6): 681-687. [[doi](https://doi.org/10.1136/jnnp-2018-319592)]
* **Low A**, Yong T, Chandler RJ, Ng KP, Kandiah N. Predictors and Patterns of Cognitive Decline Differ between Mild Cognitive Impairment in Parkinson’s disease (PD-MCI) and Alzheimer’s disease (AD-MCI). J Alzheimers Parkinsonism Dement. 2019; 3(1): 27.
* **Low A**, Lim L, Lim L, Wong B, Silva E, Ng KP, Kandiah N. Construct Validity of the Visual Cognitive Assessment Test (VCAT): A Cross-Cultural Language-Neutral Cognitive Screening Tool. Int Psychogeriatr. 2019; 21:1-9. [[doi](https://doi.org/10.1017/S1041610219000504)]

 -->

