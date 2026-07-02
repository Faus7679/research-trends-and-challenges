# Research Trends and Challenges in Computational Science and Software Engineering

**Author:** [Student Name]  
**Course:** [Course Name and Number]  
**Institution:** [University Name]  
**Instructor:** [Instructor Name]  
**Date:** July 2026

---

## Abstract

This paper examines the current landscape of computational science research by exploring active theoretical and applied trends, identifying unresolved challenges within the Software Engineering discipline, analyzing emerging obstacles in computational science, and evaluating how these developments influence individual, organizational, and societal behaviors. Drawing on peer-reviewed literature and recent industry reports, the analysis demonstrates that advances in machine learning, quantum computing, and high-performance computing are reshaping research priorities, while simultaneously introducing challenges around reproducibility, security, and ethical governance. These dynamics exert measurable pressure on cultural norms, professional responsibility, and the ways in which technology communities collaborate and socialize.

*Keywords:* computational science, software engineering, machine learning, quantum computing, research trends, emerging challenges

---

## Introduction

Computational science sits at the intersection of mathematics, computer science, and domain-specific sciences, providing the algorithmic and software infrastructure that drives modern research across medicine, physics, climate modeling, finance, and beyond. In parallel, Software Engineering—the discipline most directly responsible for designing, building, and maintaining the software systems that underpin computational science—continues to evolve in response to rapidly changing requirements, scale demands, and societal expectations.

Understanding both the trajectories and the gaps in these fields is essential for practitioners, researchers, and policymakers. This paper addresses four interconnected questions: (1) what trends characterize contemporary computational science research; (2) which topics urgently require additional research within Software Engineering; (3) what emerging challenges threaten the progress of computational science; and (4) how do these trends, topics, and challenges reshape human behavior at the individual, organizational, and societal levels.

---

## Section 1: Current Trends in Computational Science Research

### 1.1 Machine Learning and Artificial Intelligence Integration

Perhaps the most transformative trend in computational science over the past decade is the deep integration of machine learning (ML) and artificial intelligence (AI) into both theoretical frameworks and applied workflows. Neural network architectures—particularly deep learning models—have demonstrated breakthrough performance in tasks ranging from protein structure prediction (Jumper et al., 2021) to climate emulation (Rasp et al., 2021). AlphaFold2's prediction of protein folding with near-experimental accuracy exemplifies how ML-driven computational methods are supplanting or augmenting traditional first-principles simulations that previously required orders of magnitude more computing time (Jumper et al., 2021).

From a theoretical perspective, researchers are investigating the mathematical foundations of deep learning: generalization bounds, the geometry of loss landscapes, and the expressive power of various architectures (Bartlett et al., 2021). Applied research increasingly focuses on physics-informed neural networks (PINNs), which embed known physical laws as constraints within the training objective, enabling models to solve partial differential equations with limited labeled data (Raissi et al., 2019). These dual developments—theoretical formalization and applied deployment—illustrate that the ML trend operates simultaneously on both dimensions of computational science.

### 1.2 High-Performance and Exascale Computing

The deployment of exascale supercomputers—systems capable of performing 10¹⁸ floating-point operations per second—represents a structural shift in what is computationally tractable. The United States Department of Energy's Frontier system at Oak Ridge National Laboratory achieved exascale status in 2022 (Top500, 2022), and similar milestones have followed in Europe and Asia. This expansion in raw compute power is enabling simulations of unprecedented fidelity in areas such as nuclear fusion modeling, drug discovery, and cosmological structure formation (Messina, 2017).

Theoretically, exascale computing has motivated renewed interest in numerical stability and algorithm design optimized for massively parallel architectures. Practically, it has accelerated the co-design of hardware and software: application teams now work directly with processor architects to adapt solvers and data structures to heterogeneous node configurations that combine CPUs with GPUs and specialized accelerators (Dongarra et al., 2014). This co-design paradigm has become a recognized subdiscipline of computational science in its own right.

### 1.3 Quantum Computing

Quantum computing occupies a unique position as a trend that is both theoretically mature and practically nascent. Quantum algorithms such as Shor's factoring algorithm and Grover's search algorithm were established theoretically in the 1990s; however, viable fault-tolerant quantum hardware is only beginning to approach the scales needed to outperform classical computers on problems of practical interest (Preskill, 2018). The concept of "quantum advantage"—demonstrating that a quantum device solves a problem faster than any classical computer—has been claimed by Google (Arute et al., 2019) and challenged by subsequent classical algorithm improvements, illustrating the healthy tension between theoretical predictions and experimental realities.

Applied research increasingly explores near-term "noisy intermediate-scale quantum" (NISQ) devices for optimization problems, quantum chemistry, and machine learning kernels, even without full error correction (Preskill, 2018). Hybrid classical-quantum algorithms—such as the variational quantum eigensolver (VQE)—combine classical optimization loops with quantum circuit evaluations to simulate molecular Hamiltonians at scales intractable for pure classical methods (Peruzzo et al., 2014).

### 1.4 Reproducibility and Open Science

A quieter but structurally important trend is the growing emphasis on reproducibility in computational research. Investigations have shown that a significant fraction of published computational results cannot be reproduced due to undisclosed code, proprietary data, or environment dependencies (Peng, 2011; Stodden et al., 2018). Responses include the adoption of containerization technologies (Docker, Singularity), version-controlled workflow management systems (Snakemake, Nextflow), and open-data mandates from funding agencies such as the U.S. National Science Foundation and the European Research Council. Journals across computational biology, climate science, and computational physics now require authors to deposit code and data, reflecting a cultural shift toward transparency as a scientific norm.

### 1.5 Data-Intensive Science and Scientific Data Management

The fourth paradigm of science—data-intensive discovery (Hey et al., 2009)—continues to mature as instruments, simulations, and sensor networks generate petabyte-scale datasets. High-Energy Physics at CERN's Large Hadron Collider, the Square Kilometre Array radio telescope, and global genomic databases all exemplify domains where the challenge is less about compute and more about data management, query performance, and analysis pipelines. Trends include federated learning (training models across distributed datasets without centralizing raw data), efficient data serialization formats, and provenance tracking to maintain the lineage of derived datasets (Jordan & Mitchell, 2015).

---

## Section 2: Current Topics Requiring Research in Software Engineering

### 2.1 Software Reliability and Formal Verification

Despite decades of research, software failures remain common and costly. The 2021 global software-related losses exceeded $2.08 trillion according to the Consortium for Information and Software Quality (CISQ, 2022). Formal verification—mathematically proving that a program satisfies its specification—remains computationally expensive and requires significant expertise, limiting its adoption in industrial practice. Research is needed to develop more scalable automated verification tools, better abstractions for concurrent and distributed systems, and methods to formally verify machine learning models whose behavior is notoriously difficult to specify (Seshia et al., 2018). Hybrid approaches that combine lightweight runtime monitoring with static analysis are a promising direction (Leucker & Schallhart, 2009).

### 2.2 Security Engineering and DevSecOps

The Software Engineering community has long advocated for security-by-design, yet the frequency and severity of software vulnerabilities continue to escalate. High-profile supply-chain attacks—such as the SolarWinds incident in 2020 and the Log4Shell vulnerability in 2021—demonstrated that attackers are exploiting trusted software pipelines rather than individual systems (Solarwinds, 2021). Research is needed in several areas: automated vulnerability detection using program analysis and ML; software bill of materials (SBOM) standards and tooling; security requirements elicitation; and the integration of security practices into agile and DevOps workflows under the "DevSecOps" paradigm (Williams & Dabirsiaghi, 2012). Understanding why developers introduce vulnerabilities—cognitive load, inadequate training, unclear APIs—is equally important (Green & Smith, 2016).

### 2.3 AI-Assisted and Automated Software Development

The emergence of large language model (LLM)-based coding assistants—such as GitHub Copilot, OpenAI Codex, and similar tools—has introduced fundamentally new questions for Software Engineering research. Empirical studies show that these tools increase developer throughput but also introduce security vulnerabilities and code quality issues when developers uncritically accept suggestions (Pearce et al., 2022). Research questions include: How should automated code generation tools be evaluated for correctness and safety? How do developers form mental models of AI-generated code? What sociotechnical governance structures should surround AI-assisted development in safety-critical systems? The intersection of human factors research, empirical software engineering, and AI ethics is particularly under-explored.

### 2.4 Software Sustainability and Technical Debt

Technical debt—the accumulated cost of deferred or suboptimal design decisions—is a well-recognized phenomenon, yet reliable measurement and management strategies remain elusive. Research shows that a significant portion of a software team's time is spent addressing technical debt rather than delivering new functionality (Besker et al., 2018). Longitudinal studies that track how debt evolves across project lifetimes, tooling that quantifies debt in heterogeneous codebases, and organizational interventions that incentivize debt repayment are all under-researched. Additionally, the sustainability of open-source software—on which much critical infrastructure depends—raises questions about maintenance economics, contributor burnout, and governance models (Eghbal, 2020).

### 2.5 Human-Centered Software Engineering

Traditional software engineering metrics focus on code artifacts, but evidence increasingly shows that team dynamics, communication patterns, and developer well-being have strong impacts on software quality and delivery. Research topics include: the effect of remote and distributed work on coordination costs; the role of psychological safety in defect detection and knowledge sharing; inclusive design practices that ensure software is accessible and unbiased; and evidence-based approaches to developer onboarding and mentoring. The COVID-19 pandemic catalyzed a dramatic shift to remote work, creating a natural experiment whose full implications for Software Engineering practice are still being analyzed (Ralph et al., 2020).

---

## Section 3: Emerging Challenges in Computational Science Research

### 3.1 Reproducibility and Replication Crisis

As noted in Section 1.4, computational science faces a reproducibility crisis that threatens the integrity of the scientific record. A key challenge is that reproducibility requires not only code and data but also precise software environments, hardware configurations, and random seeds. Containers and workflow managers partially address this, but long-term preservation of computational environments remains unsolved: software dependencies become obsolete, cloud APIs change, and proprietary components may be withdrawn (Stodden et al., 2018). Addressing this challenge requires investment in persistent digital infrastructure (repositories, archives), community standards for environment specification, and funding agency policies that reward reproducible research.

### 3.2 Energy Consumption and Environmental Sustainability

Training large ML models and running exascale simulations consume enormous amounts of electricity. Estimates suggest that training a single large language model can emit as much CO₂ as five cars over their entire lifetimes (Strubell et al., 2019). As computational workloads grow, data centers' share of global electricity consumption is projected to increase significantly. The challenge is twofold: technical (developing more energy-efficient algorithms, hardware, and cooling systems) and governance-related (establishing standards for reporting computational carbon footprints, incentivizing green computing practices). The research community must grapple with the tension between scientific ambition and environmental responsibility.

### 3.3 Ethical AI and Algorithmic Bias

As ML-driven computational systems are deployed in high-stakes domains—criminal justice, healthcare, hiring, and credit—algorithmic bias and fairness have emerged as critical challenges. Biases encoded in training data propagate into model predictions, potentially amplifying existing social inequities (Obermeyer et al., 2019). Addressing this requires interdisciplinary collaboration: computer scientists must work with social scientists, ethicists, and affected communities to define context-appropriate fairness criteria, audit deployed systems, and design redress mechanisms. Technical interventions such as fairness-aware training, differential privacy, and interpretability methods are necessary but insufficient without accompanying policy and legal frameworks (Barocas et al., 2019).

### 3.4 Cybersecurity in Computational Infrastructure

Computational science infrastructure—HPC clusters, cloud-based simulation platforms, research data repositories—is increasingly targeted by cybercriminals and state actors. The 2020 compromise of numerous European supercomputers by cryptocurrency miners demonstrated that even air-gapped research networks are vulnerable (NCSC, 2020). Challenges include securing complex, heterogeneous software stacks; managing privileged access in multi-user research environments; and protecting sensitive research data (pre-publication results, personally identifiable biomedical data). Addressing these challenges requires a shift from reactive to proactive security: threat modeling specific to computational research workflows, mandatory security training for researchers, and collaboration between computer security researchers and domain scientists.

### 3.5 Talent Pipeline and Interdisciplinary Training

Computational science requires researchers fluent in both domain science and advanced computational methods—a combination that traditional academic structures are poorly designed to produce. Funding and recognition systems in academia reward disciplinary depth over breadth, creating a "two-culture" problem where domain scientists lack computational literacy and computer scientists lack domain context (Wilson et al., 2014). Addressing this challenge requires curriculum reform at undergraduate and graduate levels, new interdisciplinary degree programs, professional development resources (such as the Software Carpentry and Data Carpentry programs), and promotion criteria that value software and data contributions alongside traditional publications.

### 3.6 Managing Scale and Complexity

Modern computational systems—from cloud-native microservices to multi-physics simulation frameworks—operate at scales of complexity that challenge both human understanding and automated analysis tools. Emergent behaviors, cascading failures, and subtle interactions between components are difficult to anticipate, test, or debug. Chaos engineering (deliberately injecting failures to discover weaknesses), advanced observability tooling, and formal methods for distributed systems are partial responses, but no comprehensive solution exists. Research into complexity science, resilience engineering, and human-computer interaction for system operators is needed to develop principled approaches to managing this complexity (Sommerville, 2011).

---

## Section 4: Impact on Individual, Organizational, and Societal Behaviors

### 4.1 Impact on Individuals

The trends and challenges described above reshape the professional identity, daily practices, and ethical responsibilities of individual computational scientists and software engineers in several ways.

**Cultural shifts:** The reproducibility movement has instilled a new professional norm: publishing code and data is no longer optional but expected. Researchers who previously regarded their code as a secondary artifact now invest in documentation, testing, and packaging as integral parts of the research process. This norm is being socialized through graduate training programs, mentorship, and peer review practices (Peng, 2011).

**Responsibility:** The widespread use of AI coding assistants places new responsibility on individual developers to critically evaluate machine-generated code rather than accepting it uncritically. This demands elevated metacognitive skills—awareness of where automated tools may fail—and a stronger sense of professional accountability for software quality and security (Pearce et al., 2022). Similarly, researchers who deploy ML models in consequential domains must grapple with their personal ethical obligations when those models produce harmful outcomes.

**Socialization and well-being:** The shift to distributed and remote work, accelerated by the COVID-19 pandemic, has changed how software engineers and researchers socialize with colleagues: asynchronous communication tools replace hallway conversations, onboarding becomes harder, and informal mentorship relationships are more difficult to form (Ralph et al., 2020). Burnout and isolation are documented concerns, particularly for open-source maintainers who support critical infrastructure without commensurate recognition or compensation (Eghbal, 2020).

### 4.2 Impact on Organizations

**Culture:** Computational science organizations—research labs, universities, and technology companies—are being reshaped by the open-science movement and by the demands of cross-disciplinary collaboration. "Research software engineer" (RSE) has emerged as a recognized professional role distinct from both the traditional academic researcher and the industrial software developer, reflecting an organizational acknowledgment that high-quality software development is a distinct and valued competency (Hettrick et al., 2014). Organizations are establishing RSE groups, data science platforms, and reproducibility offices to institutionalize these values.

**Responsibility:** The cybersecurity challenge imposes new organizational responsibilities: compliance with data protection regulations (GDPR, HIPAA), incident response planning, and vendor risk management. Supply-chain attacks have prompted organizations to demand software bills of materials from vendors and to implement stricter controls over dependencies (Solarwinds, 2021). These obligations require investment in security personnel and infrastructure that many research organizations—accustomed to lean operational models—have historically lacked.

**Governance and socialization:** Algorithmic fairness and ethical AI concerns are driving organizations to establish internal AI ethics boards, impact assessment processes, and external stakeholder engagement programs. Companies such as Google, Microsoft, and IBM have published AI principles and governance frameworks; research institutions are developing institutional review processes analogous to Institutional Review Boards for human subjects research (Jobin et al., 2019). These governance mechanisms represent new forms of organizational socialization that embed ethical deliberation into standard operating procedures.

### 4.3 Impact on Society

**Cultural norms:** The broad societal penetration of AI-driven computational systems—in search engines, healthcare diagnostics, financial services, and criminal justice—has begun to reshape cultural norms around privacy, agency, and trust. Surveys consistently show that public trust in AI systems is conditional on perceived transparency and accountability (Eurobarometer, 2020). The growing discourse around algorithmic rights and the "right to explanation" (as articulated in the EU's General Data Protection Regulation) reflects a societal demand that computational systems be legible and contestable.

**Responsibility and regulation:** Governments and international bodies are responding to computational science's societal footprint with new regulatory frameworks. The EU AI Act (2024), the U.S. Executive Order on Safe, Secure, and Trustworthy AI (2023), and similar instruments in China, the United Kingdom, and Canada attempt to impose safety, transparency, and accountability obligations on AI developers and deployers. These frameworks reflect a societal judgment that the benefits of computational innovation must be balanced against harm prevention and equitable distribution of benefits.

**Socialization and equity:** The energy demands of large-scale computation raise questions of environmental justice: data centers are disproportionately sited in regions with low electricity costs but high environmental impact. The talent pipeline challenge intersects with equity: underrepresented groups in science and engineering face structural barriers that compound the difficulty of entering computationally intensive fields. Initiatives such as broadening participation programs, open-access publication mandates, and free online educational resources (MOOCs, Software Carpentry) are attempts to mitigate these inequities. At a macro level, the concentration of advanced computational capabilities—supercomputers, large AI training clusters—in a small number of wealthy nations and corporations raises geopolitical and equity concerns about who controls the infrastructure of knowledge production.

---

## Conclusion

Computational science and Software Engineering stand at a pivotal moment. The trends surveyed here—AI/ML integration, exascale computing, quantum computing, open science, and data-intensive discovery—offer extraordinary scientific and societal opportunities. Yet these opportunities are accompanied by equally significant challenges: reproducibility failures, unsustainable energy demands, algorithmic bias, cybersecurity threats, and an insufficient talent pipeline. These challenges are not merely technical; they are cultural, organizational, and political.

The individuals who practice computational science and software engineering must internalize new professional norms centered on transparency, responsibility, and ethical awareness. Organizations must evolve governance structures, recognize new roles, and accept accountability for the systems they create. Society must engage in deliberate, inclusive, and evidence-based policy discussions to ensure that the benefits of computational progress are broadly shared and its harms are mitigated.

Meeting these intertwined opportunities and challenges is one of the defining tasks of the coming decades.

---

## References

Arute, F., Arya, K., Babbush, R., Bacon, D., Bardin, J. C., Barends, R., ... & Martinis, J. M. (2019). Quantum supremacy using a programmable superconducting processor. *Nature*, *574*(7779), 505–510. https://doi.org/10.1038/s41586-019-1666-5

Barocas, S., Hardt, M., & Narayanan, A. (2019). *Fairness and machine learning: Limitations and opportunities*. fairmlbook.org. https://fairmlbook.org/

Bartlett, P. L., Montanari, A., & Rakhlin, A. (2021). Deep learning: A statistical viewpoint. *Acta Numerica*, *30*, 87–201. https://doi.org/10.1017/S0962492921000027

Besker, T., Martini, A., & Bosch, J. (2018). Technical debt cripples software developer productivity: A longitudinal study on developers' daily software development work. *Proceedings of the 2018 IEEE/ACM International Conference on Technical Debt*, 105–114. https://doi.org/10.1145/3194164.3194178

CISQ (Consortium for Information and Software Quality). (2022). *The cost of poor software quality in the US: A 2022 report*. https://www.it-cisq.org/

Dongarra, J., Hittinger, J., Bell, J., Chacon, L., Falgout, R., Heroux, M., ... & Wild, S. (2014). *Applied mathematics research for exascale computing* (Report No. DOE/ASCR-14). U.S. Department of Energy. https://doi.org/10.2172/1149042

Eghbal, N. (2020). *Working in public: The making and maintenance of open source software*. Stripe Press.

Eurobarometer. (2020). *Attitudes towards the impact of digitisation and automation on daily life* (Special Eurobarometer 501). European Commission. https://europa.eu/eurobarometer/

Green, M., & Smith, M. (2016). Developers are not the enemy! The need for usable security APIs. *IEEE Security & Privacy*, *14*(5), 40–46. https://doi.org/10.1109/MSP.2016.100

Hettrick, S., Antonioletti, M., Carr, L., Chue Hong, N., Crouch, S., De Roure, D., ... & Sufi, S. (2014). UK research software survey 2014. *Zenodo*. https://doi.org/10.5281/zenodo.14809

Hey, T., Tansley, S., & Tolle, K. (Eds.). (2009). *The fourth paradigm: Data-intensive scientific discovery*. Microsoft Research.

Jobin, A., Ienca, M., & Vayena, E. (2019). The global landscape of AI ethics guidelines. *Nature Machine Intelligence*, *1*(9), 389–399. https://doi.org/10.1038/s42256-019-0088-2

Jordan, M. I., & Mitchell, T. M. (2015). Machine learning: Trends, perspectives, and prospects. *Science*, *349*(6245), 255–260. https://doi.org/10.1126/science.aaa8415

Jumper, J., Evans, R., Pritzel, A., Green, T., Figurnov, M., Ronneberger, O., ... & Hassabis, D. (2021). Highly accurate protein structure prediction with AlphaFold. *Nature*, *596*(7873), 583–589. https://doi.org/10.1038/s41586-021-03819-2

Leucker, M., & Schallhart, C. (2009). A brief account of runtime verification. *Journal of Logic and Algebraic Programming*, *78*(5), 293–303. https://doi.org/10.1016/j.jlap.2008.08.004

Messina, P. (2017). The Exascale Computing Project. *Computing in Science & Engineering*, *19*(3), 63–67. https://doi.org/10.1109/MCSE.2017.57

NCSC (National Cyber Security Centre). (2020). *Advisory: Malicious actors compromise European supercomputers to mine cryptocurrency*. https://www.ncsc.gov.uk/

Obermeyer, Z., Powers, B., Vogeli, C., & Mullainathan, S. (2019). Dissecting racial bias in an algorithm used to manage the health of populations. *Science*, *366*(6464), 447–453. https://doi.org/10.1126/science.aax2342

Pearce, H., Ahmad, B., Tan, B., Dolan-Gavitt, B., & Karri, R. (2022). Asleep at the keyboard? Assessing the security of GitHub Copilot's code contributions. *2022 IEEE Symposium on Security and Privacy*, 754–768. https://doi.org/10.1109/SP46214.2022.9833571

Peng, R. D. (2011). Reproducible research in computational science. *Science*, *334*(6060), 1226–1227. https://doi.org/10.1126/science.1213847

Peruzzo, A., McClean, J., Shadbolt, P., Yung, M. H., Zhou, X. Q., Love, P. J., ... & O'Brien, J. L. (2014). A variational eigenvalue solver on a photonic quantum processor. *Nature Communications*, *5*(1), 4213. https://doi.org/10.1038/ncomms5213

Preskill, J. (2018). Quantum computing in the NISQ era and beyond. *Quantum*, *2*, 79. https://doi.org/10.22331/q-2018-08-06-79

Raissi, M., Perdikaris, P., & Karniadakis, G. E. (2019). Physics-informed neural networks: A deep learning framework for solving forward and inverse problems involving nonlinear partial differential equations. *Journal of Computational Physics*, *378*, 686–707. https://doi.org/10.1016/j.jcp.2018.10.045

Ralph, P., Baltes, S., Adisaputri, G., Torkar, R., Kovalenko, V., Kalinowski, M., ... & Alkadhi, R. (2020). Pandemic programming: How COVID-19 affects software developers and how their organizations can help. *Empirical Software Engineering*, *25*(6), 4927–4961. https://doi.org/10.1007/s10664-020-09875-y

Rasp, S., Dueben, P. D., Scher, S., Weyn, J. A., Mouatadid, S., & Thuerey, N. (2021). WeatherBench: A benchmark data set for data-driven weather forecasting. *Journal of Advances in Modeling Earth Systems*, *13*(7), e2020MS002203. https://doi.org/10.1029/2020MS002203

Seshia, S. A., Sadigh, D., & Sastry, S. S. (2018). Formal specification for deep neural networks. *International Symposium on Automated Technology for Verification and Analysis*, 20–34. https://doi.org/10.1007/978-3-030-01090-4_2

Solarwinds. (2021). *SUNBURST cyberattack overview*. https://www.solarwinds.com/sa-overview/securityadvisory

Sommerville, I. (2011). *Software engineering* (9th ed.). Addison-Wesley.

Stodden, V., Seiler, J., & Ma, Z. (2018). An empirical analysis of journal policy effectiveness for computational reproducibility. *Proceedings of the National Academy of Sciences*, *115*(11), 2584–2589. https://doi.org/10.1073/pnas.1708290115

Strubell, E., Ganesh, A., & McCallum, A. (2019). Energy and policy considerations for deep learning in NLP. *Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics*, 3645–3650. https://doi.org/10.18653/v1/P19-1355

Top500. (2022). *Top500 list – November 2022*. https://www.top500.org/lists/top500/2022/11/

Williams, J., & Dabirsiaghi, A. (2012). The unfortunate reality of insecure libraries. *Contrast Security White Paper*. https://www.contrastsecurity.com/

Wilson, G., Aruliah, D. A., Brown, C. T., Chue Hong, N. P., Davis, M., Guy, R. T., ... & Wilson, P. (2014). Best practices for scientific computing. *PLOS Biology*, *12*(1), e1001745. https://doi.org/10.1371/journal.pbio.1001745
