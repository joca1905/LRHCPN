# LRHCPN
Implementation of the logistic regression algorithm in colored Petri nets
![RLHCPN_classification](images/RL.png)
<p align="justify">
Implementation of the logistic regression algorithm for colored Petri nets using the CPN-tools software. The algorithm works for classification. It includes various functions implemented in CPN-ML and examples of applications in different databases. An excellent tool for those working with CPN-tools and discrete event systems.
</p>

**:rocket: Technologies used in the project:**

:computer: CPN Tools:  https://cpntools.org/
:memo: Version: 4.0.1

:computer: CPN IDE: https://cpnide.org/
:memo: Version: 1.24.1031

# ⚙️ **Implementation Features** 

- **Applicable to binary Classification:** <p align="justify">The LR algorithm implemented in coloured Petri nets (LRHCPN) is suitable for addressing both binary classification problems.</p>

- **Graphical Visualization:** <p align="justify"> The model in Petri nets provides a graphical visualization of the LR algorithm, making the modeling process straightforward and user-friendly.</p>

- **Fully Adaptable Implementation:** <p align="justify"> The proposed method offers a fully adaptable implementation and can be used with any set of numerical data for binary classification.</p>

- **Versatile Application:** <p align="justify"> This implementation is ideal for modeling discrete systems, supporting the development of a variety of new applications.</p>

# :exclamation: **Instructions for using RL for binary classification:** 
- **`STEP 1:`**<p align="justify"> Open the CPN tools and in the toolbox open the **NET** palette, then click on the **Load net** option and load the `RL_IOT.cpn` model.</p>
- **`STEP 2:`**<p align="justify"> In the CPN Tools toolbox, with the model loaded, click on the `Declarations` option. Upon clicking this item, directly below `Standard declarations`, you will find the `Config model` option to adjust the model parameters. The configurable parameters are: `i` (number of iterations), `bt` (batch size setting, used only with the "mini-batch" solver; use `NONE` for other configurations), `lr` (learning rate), and `solver` (optimizer). For `solver`, there are currently three available functions: `"sgd"`, `"batch"`, and `"mini-batch"`.</p>
- **`STEP 3:`**<p align="justify"> In the transitions `Load elements from test`, `Load elements training`, `Load test labels`, and `Load training labels`, adjust the links to the location on your computer where the .txt files of the training and testing databases are stored. The databases are divided into four parts: training samples, testing samples, training labels, and testing labels. Place the files in the correct locations.</p>
- **`STEP 4:`**<p align="justify"> For a faster simulation, in the toolbox, open the `Simulation` palette and press the `Fast forward` tool. You can also adjust the value of this tool to simulate a larger number of model steps.
</p>

# :bulb: **Simulation of discrete event systems** 

![RHCPN_planta1](images/IOT.png)
<p align="justify">
The LRHCPN opens up new possibilities for the modeling of discrete event systems, and it can be integrated into other models to perform binary classification tasks.
</p>

![RHCPN_planta2](images/Check-for-Fault.png)

<p align="justify">
In the detection of attacks on IoT services, the RLHCPN can be configured to monitor network traffic and identify anomalous patterns associated with attacks. For instance, IoT sensors can send real-time traffic data to the Petri net model, which classifies it as normal or suspicious traffic using RL algorithms. The model processes the information and makes automatic decisions based on predefined attack patterns, helping to quickly identify threats and activate appropriate responses in the security system.
</p>

# 📁 Applied Datasets

| **Dataset**                                    | **Description**                                                                                                                                                               |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **IoT dataset for Intrusion Detection Systems (IDS) - BoTNeTIoT-L01** | Available at [IDS Dataset][https://www.kaggle.com/datasets/azalhowaide/iot-dataset-for-intrusion-detection-systems-ids/data]  |


# Authors

<table>
  <tr>
    <td>
      <img src="https://github.com/joca1905/KNNHCPN/blob/9622ecf604c4f60df4f5246f2ef2380682118c24/Images/Joaquim.jpg" alt="foto_joaquim" width="150"/>
    </td>
    <td>
      <strong>Joaquim Osterwald Frota Moura Filho</strong><br>
      <sub>PhD student at PPGETI, Federal University of Ceará</sub>
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://github.com/joca1905/KNNHCPN/blob/1c15b254dbb96ee0a7937a4e7fa6f9f46666c97a/Images/van.jpg" alt="foto_vanessa" width="150"/>
    </td>
    <td>
      <strong>Vanessa Vieira de Sousa </strong><br>
      <sub>PhD student at PPGETI, Federal University of Ceará</sub>
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://github.com/joca1905/KNNHCPN/blob/9622ecf604c4f60df4f5246f2ef2380682118c24/Images/Giovanni.jpeg" alt="foto_gio3" width="150"/>
    </td>
    <td>
      <strong>Giovanni Cordeiro Barroso</strong><br>
      <sub>Full professor at the Federal University of Ceará</sub>
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://github.com/joca1905/KNNHCPN/blob/9622ecf604c4f60df4f5246f2ef2380682118c24/Images/George.jpeg" alt="foto_george" width="150"/>
    </td>
    <td>
      <strong>George André Pereira Thé</strong><br>
      <sub>Professor at the Federal University of Ceará</sub>
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://github.com/joca1905/KNNHCPN/blob/9622ecf604c4f60df4f5246f2ef2380682118c24/Images/Amora.jpeg" alt="foto_amora" width="150"/>
    </td>
    <td>
      <strong>Márcio André Baima Amora</strong><br>
      <sub>Associate professor I at the Federal University of Ceará, Sobral Campus</sub>
    </td>
  </tr>
</table>

# References

[1] A. Alhowaide, I. Alsmadi, and J. Tang, ``Towards the design of real-time autonomous IoT NIDS,'' Cluster Comput, vol. 26, pp. 2489--2502, 2023. https://doi.org/10.1007/s10586-021-03231-5.

[2] J. P. da Silva Fonseca, A. R. de Sousa, and J. J. P. Z. de Souza Tavares, ``Modeling and controlling IoT-based devices’ behavior with high-level Petri nets,'' Procedia Computer Science, vol. 217, pp. 1462--1469, 2023. 4th International Conference on Industry 4.0 and Smart Manufacturing. https://doi.org/10.1016/j.procs.2022.12.345.

[3] D. Jurafsky and J. H. Martin, ``Speech and Language Processing: An Introduction to Natural Language Processing, Computational Linguistics, and Speech Recognition with Language Models,'' 3rd ed., draft, Stanford Univ. and Univ. of Colorado at Boulder, Aug. 2024. 

[4] R. Albuquerque, C. Júnior, G. Barroso, and G. Barreto, ``A novel fully adaptive neural network modeling and implementation using colored Petri nets,'' Discrete Event Dynamic Systems, vol. 33, pp. 1--32, Jun. 2023, doi: 10.1007/s10626-023-00377-9.

[5] M. Nauman, N. Akhtar, O. H. Alhazmi, M. Hameed, H. Ullah, and N. Khan, ``Improving the correctness of medical diagnostics based on machine learning with coloured Petri nets,'' IEEE Access, vol. 9, pp. 143434--143447, 2021, doi: 10.1109/ACCESS.2021.3121092.

[6] Y. R. M. de Oliveira, Á. Sobrinho, L. D. da Silva, D. Santos, K. C. Gorgônio, and A. Perkusich, ``Coloured Petri Nets Modeling Multilayer Perceptron Neural Networks,'' in 2024 IEEE International Conference on Consumer Electronics (ICCE), 2024, pp. 1--4. https://doi.org/10.1109/ICCE59016.2024.10444319.

[7] X. Wang, W. Yu, Z. Ding, X. Zhai, and S. Saha, ``Modeling and Analyzing of Breast Tumor Deterioration Process with Petri Nets and Logistic Regression,'' Complex System Modeling and Simulation, vol. 2, no. 3, pp. 264--272, 2022. https://doi.org/10.23919/CSMS.2022.0016.

[8] Y. Xing, H. Shu, H. Zhao, D. Li, and L. Guo, ``Survey on botnet detection techniques: Classification, methods, and evaluation,'' Math. Probl. Eng., vol. 2021, Article ID 6640499, Apr. 2021, https://doi.org/10.1155/2021/6640499.

[9] Y. Meidan et al., ``N-BaIoT—Network-Based Detection of IoT Botnet Attacks Using Deep Autoencoders,'' IEEE Pervasive Comput., vol. 17, no. 3, pp. 12--22, Jul.--Sep. 2018, doi: 10.1109/MPRV.2018.03367731.

[10] A. Alhowaide, I. Alsmadi, J. Tang, ``Features Quality Impact on Cyber Physical Security Systems,'' 2019 IEEE 10th Annual Information Technology, Electronics and Mobile Communication Conference (IEMCON), outubro de 2019.

[11] C. A. Petri, ``Kommunikation mit Automaten'' (Communication with Automata), Ph.D. Thesis, University of Bonn, 1962.

# Citation

If this repository helps you in any way, consider citing our paper as follows:

```bibtex
@unpublished{moura2024rl,
  author    = {Joaquim Moura and Vanessa Vieira and Giovanni Barroso and George A. P. Thé and Márcio Amora},
  title     = {Modeling the Logistic Regression Algorithm Using Colored Petri Nets to detect anomalous traffic in IoT services},
  note      = {In preparation},
  year      = {2024},
  organization = {Federal University of Ceará},
}
