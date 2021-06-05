# AntiKnowledgeBase

This repository contains data related to the paper "Mining an" anti-knowledge base" from Wikipedia updates with applications to fact checking and beyond" (VLDB'20). 

An Anti-Knowledge Base (AKB) is a collection of mistakes, expressed as subject-predicate-object triples (with the semantics that the corresponding fact is false). The current version contains around 100,000 such triples, mined by analyzing the update log on Wikipedia using a large cluster. The specific steps of the mining pipeline are described in detail in the aforementioned paper. 

The repository contains two files, containing different types of mistakes:
- akb_entities.tsv contains mistakes where people confuse entities
- akb_numbers.tsv contains mistakes where people confuse numbers

The AKB entries have been mined automatically and have no perfect precision (i.e., some of the entries may accidentally represent accurate facts). The entries are ranked (i.e., the first entries are more likely to represent mistakes) and are associated with confidence values. 

When using the data in this repository, please cite the associated paper, e.g. via BibTex:

@article{karagiannis2019mining,
  title={Mining an" anti-knowledge base" from Wikipedia updates with applications to fact checking and beyond},
  author={Karagiannis, Georgios and Trummer, Immanuel and Jo, Saehan and Khandelwal, Shubham and Wang, Xuezhi and Yu, Cong},
  journal={Proceedings of the VLDB Endowment},
  volume={13},
  number={4},
  pages={561--573},
  year={2019},
  publisher={VLDB Endowment}
}
