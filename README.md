# Learning-Assisted Optimization for Transmission Switching

## Goals ⚽

The aim of this repository is to provide some details of the data sets used in paper [[1]](https://arxiv.org/abs/2304.07269). This article has been developed by some members of the [OASYS group](https://sites.google.com/view/groupoasys/home) thanks to the funding of the project [Flexanalytics](https://groupoasysflexanalytics.readthedocs.io/en/latest/). We suggest you to visit the related link to know more our research 😉

## How can I download the data? ⬇
The data files are included in this repository.

## Summary 🧮📊📖

The success of the proposal analyzed in [[1]](https://arxiv.org/abs/2304.07269) has been tested in a realistic 118-bus power system. The data comprises four files:

The first one is `case118Blumsak.m`. It contains information about the network (nodes, lines, generators location, maximum flow capacity, etc).

Then, three files containing the information of the data have been included. In these files, the results of the 500 instances generated for each of the three databases used in the paper can be found. The first columns contain the load values for the 118 buses. The next columns represent the optimal decision variables for the 186 lines. If the decision variable associated with a certain line is always 1, then, it means that this line belongs to the given spanning tree. Finally, the last columns are associated with the optimal voltage angles for the 118 buses.

The three databases differ on the nodal demand $d_n$ values generated with three different probability distributions centered in the baseline demand $\widehat{d_n}$. The three cases detailed in the manuscript are:
* `unif10`: The demand levels are sampled using independent uniform distributions in the range
[0.9 $\widehat{d_n}$, 1.1 $\widehat{d_n}$]
* `unif20`: The demand levels are sampled using independent uniform distributions in the range
[0.8 $\widehat{d_n}$, 1.2 $\widehat{d_n}$]
* `normal`: The demand levels are sampled using a multinormal distribution with the correlation matrix obtained from the demand time series available at [3].

## References 📚

[1] Pineda, S. Morales, J.M., and Jiménez-Cordero, A. (2023). Learning-Assisted Optimization for Transmission Switching. Submitted. Available [here](https://arxiv.org/abs/2304.07269).

[2] OASYS, Learning_Assisted_Optimization_for_Transmission_Switching, Github repository (https://github.com/groupoasys/Learning_Assisted_Optimization_for_Transmission_Switching), 2023.

[3] Joswig-Jones, Trager, Ahmed Zamzam, and Kyri Baker. 2021. "OPFLearnData: Dataset for Learning AC Optimal Power Flow." NREL Data Catalog. Golden, CO: National Renewable Energy Laboratory. Last updated: December 12, 2023. DOI: 10.7799/1827404. 

## How to cite the repo and the paper? 📝

If you want to cite paper [[1]](https://www.researchgate.net/publication/370058669_Learning-Assisted_Optimization_for_Transmission_Switching) or this repo [[2]](https://github.com/groupoasys/Learning_Assisted_Optimization_for_Transmission_Switching), please use the following bib entry:

* Article:
```
@techreport{pineda2023learning,
  author = {Pineda, Salvador; Morales, Juan Miguel and Jiménez-Cordero, Asunción},
  title = {Learning Assisted Optimization for Transmission Switching},
  institution = {Universidad de M\'alaga},
  year = {2023},
  note = {Available at \url{https://www.researchgate.net/publication/370058669_Learning-Assisted_Optimization_for_Transmission_Switching}}
}
```
* Repository:
```
@misc{OASYS2023learning,
author={OASYS},
  year={2023},
  title = {{Learning\_Assisted\_Optimization\_for\_Transmission\_Switching}},
  howpublished = {\url{https://github.com/groupoasys/Learning_Assisted_Optimization_for_Transmission_Switching}}
}
```

## Do you want to contribute? 🙋‍♀️🙋‍♂️
 
 Please, do it 😋 Any feedback is welcome 🤗 so feel free to ask or comment anything you want via a Pull Request in this repo.
 If you need extra help, you can ask Salvador Pineda (spineda@uma.es), Juan Miguel Morales (juan.morales@uma.es) or  Asunción Jiménez-Cordero (asuncionjc@uma.es).
 
 ## Contributors 🌬☀
 
 * [OASYS group](http://oasys.uma.es) -  groupoasys@gmail.com
 
 ## Developed by 👩‍💻👨‍💻👨‍💻
 
 * [Salvador Pineda](https://www.researchgate.net/profile/Salvador_Pineda) - spineda@uma.es
 * [Juan Miguel Morales](https://www.researchgate.net/profile/Juan_Morales25) - juan.morales@uma.es
 * [Asunción Jiménez Cordero](https://www.researchgate.net/profile/Asuncion_Jimenez-Cordero/research) - asuncionjc@uma.es
 
 
 ## License 📝
 
    Copyright 2023 Optimization and Analytics for Sustainable energY Systems (OASYS)

    Licensed under the GNU General Public License, Version 3 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.gnu.org/licenses/gpl-3.0.en.html

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.


