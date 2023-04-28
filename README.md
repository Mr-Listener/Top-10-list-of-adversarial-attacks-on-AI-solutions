# list of Top 10 adversarial attacks on AI solutions

## 1. Evasion attacks
Evasion attacks involve inputs for MLsec that result in an incorrect output and cause models to make false predictions or behave in an unexpected manner [1]. As an example from the real world, we can take an AI-driver malware detection engine, which can be bypassed using an adversarial attack by changing binary in such a way that it will not be recognized as a malware.

## 2. Poisoning attacks
Poisoning attacks involve injecting data into the training dataset to make MLsec models produce an incorrect output [2]. Such an attack can be performed, for example, against a spam filter by poisoning the ML classifier with non-spam data, which looks like spam to retrain the classifier.

## 3. Model inversion
Model inversion relates to retrieving information about the samples used in the dataset [3]. This type of attack can be used against NLP algorithms, such as GPT-3 [4], to retrieve critical information on how the system was trained.
These data can contain credit card information, passwords, or any other private information.

## 4. Backdoor attacks
Backdoor attacks affect training models in such a way that they behave anomalously when fed a particular input but work as intended with other inputs [5]. For example, AI applications, especially devices, may be developed by multiple vendors. The outsourced AI algorithm developer can insert a backdoor into their AI model and sell it to an IoT vendor as a smart speaker model. These types of backdoors can, for example, have some undocumented voice commands for accessing the device.

## 5. Model extraction
Model extraction implies gaining knowledge about the ML model and its parameters with the help of model extraction attacks [7]. For example, if someone wants to steal an API-provider’s model, the attackers could use legitimate API requests in a specially-crafted manner so that it leads to model extraction after a finite number of API calls.

## 6. Membership inference
Membership inference is a privacy attack that is intended to determine whether certain data points were in the training dataset or not [8]. The healthcare industry could be affected by these types of attacks as their datasets contain private medical data.

## 7. Trojan attacks
Trojan attacks are direct modifications to a trained model. The intention is to enable the model to perform additional tasks [9]. In comparison to the backdoor attack above, the attacker does not have access to the dataset; however, the attacker has access to the MLsec model stored or transmitted insecurely. Many AI applications were trained with the help of transfer learning, therefore, most of the time the model base is publicly available. Attackers may hack the model hosting and inject trojans into the base model and affect models derived from that as well.

## 8. Presentation attacks
Presentation attacks are methods where the attacker generates and constructs new objects to fool the MLsec model [10]. Face recognition applications are the most common target for such an attack.

## 9. Attribute inference
Attribute inference is an attack that is performed to get information about dataset attributes [11]. With this attack, the hackers may find information about the dataset attributes and guess what parameters are favored by the model. Recommendation systems may be a good example of a target for attribute inference attack.

## 10. Slowdown attack
Slowdown attack implies performing various types of DoS attacks [12], as some ML-related operations are resource intensive (e.g., re-training a model, transfer learning, inference on complex models). Any publicly available AIdriven API can be vulnerable to this type of attack.


### References

[1]: Szegedy, C., Zaremba, W., Sutskever, I., Bruna, J., Erhan, D., Goodfellow, I., Fergus, R.: Intriguing properties of neural networks (2013). https://arxiv.org/abs/1312.6199

[2]: Schwarzschild, A., Goldblum, M., Gupta, A., Dickerson, J.P., Goldstein, T.: Just how toxic is data poisoning? A unified benchmark for backdoor and data poisoning attacks. In: International Conference on Machine Learning. PMLR (2021)

[3]: Fredrikson, M., Jha, S., Ristenpart, T.: Model inversion attacks that exploit confidence information and basic countermeasures. In: Proceedings of the 22nd ACM SIGSAC Conference on Computer and Communications Security (2015)

[4]: Floridi, L., Chiriatti, M.: GPT-3: Its nature, scope, limits, and consequences. Minds Mach. 30(4), 681–694 (2020)

[5]: Gu, T., Dolan-Gavitt, B., Garg, S.: BadNets: Identifying vulnerabilities in the machine learning model supply chain (2017). https://arxiv.org/abs/1708.06733

[7]: Oh, S.J., Schiele, B., Fritz, M.: Towards reverse-engineering black-box neural networks. In: Explainable AI: Interpreting, Explaining and Visualizing Deep Learning. Springer, Berlin (2019)

[8]: Shokri, R., Stronati, M., Song, C., Shmatikov, V.: Membership inference attacks against machine learning models. In: 2017 IEEE Symposium on Security and Privacy (SP). IEEE, Piscataway (2017)

[9]: Liu, Y., Ma, S., Aafer, Y., Lee, W.C., Zhai, J., Wang, W., Zhang, X.: Trojaning attack on neural networks (2017)

[10]: Brewster, T.: Fraudsters Cloned Company Director’s Voice In $35 Million Bank Heist, Police Find (2021). https://www.forbes.com/sites/thomasbrewster/2021/10/14/huge-bankfraud-uses-deep-fake-voice-tech-to-steal-millions/?sh=1456cb187559

[11]: Gong, N.Z., Liu, B.: You are who you know and how you behave: attribute inference attacks via users’ social friends and behaviors. In: 25th {USENIX} Security Symposium (2016)

[12]: Hong, S., Kaya, Y., Modoranu, I.V., Dumitra¸s, T.: A Panda? No, It’s a Sloth: Slowdown Attacks on Adaptive Multi-Exit Neural Network Inference (2020). https://arxiv.org/abs/2010.02432


