# Submission 152 ESWC

### Contents
1. Benchmark Dataset: Dataset for benchmark evaluation.
    
    **Filepath**: [./dataset_and_results/benchmark_dataset.csv](./dataset_and_results/benchmark_dataset.csv)
2. Ontology Serialized: Ontology in the serialized format. Can be opened with [protoge](https://protege.stanford.edu/)
    
    **Filepath**: [./dataset_and_results/UOC_Ontology](./dataset_and_results/UOC_Ontology)
3. Results: The baseline outputs after postprocessing.
    
    **Filepath**: [./dataset_and_results/llm_prediction_results](./dataset_and_results/llm_prediction_results)
4. Prompts: The prompts used for the experiments.
    
    **Filepath**: [./prompts](./prompts)
5. Evaluation: The implementation of evaluation.
    
    **Filepath (Evaluation Calc)**: [./evaluation/opinion_overlap_eval.py](./evaluation/opinion_overlap_eval.py)
    **Filepath (Evaluation Applied to all results)**: [./evaluation/eval_opinion_all.ipynb](./evaluation/eval_opinion_all.ipynb)
    

## Organisation of results (Generative Model Outputs)


```bash
── MODEL_NAME
│   ├── nlprompt
│   │   ├── csv (Results in CSV)
│   │   │   ├── desc_eg_format.csv
│   │   │   ├── desc_format_eg.csv
│   │   │   ├── eg_desc_format.csv
│   │   │   ├── eg_format_desc.csv
│   │   │   ├── format_desc_eg.csv
│   │   │   └── format_eg_desc.csv
│   │   └── json (Results in JSON)
│   │       ├── desc_eg_format.json
│   │       ├── desc_format_eg.json
│   │       ├── eg_desc_format.json
│   │       ├── eg_format_desc.json
│   │       ├── format_desc_eg.json
│   │       └── format_eg_desc.json
│   └── onto_prompt
│       ├── csv
│       │   ├── jsonld.csv
│       │   ├── manchester_owl.csv
│       │   ├── obo_format.csv
│       │   ├── owl_funct.csv
│       │   ├── owl_xml.csv
│       │   ├── rdf_xml.csv
│       │   └── ttl_syntax.csv
│       └── json
│           ├── pred_jsonld.json
│           ├── pred_manchester_owl.json
│           ├── pred_obo_fromat.json
│           ├── pred_owl_funct.json
│           ├── pred_owl_xml.json
│           ├── pred_rdf_xml.json
│           └── pred_ttl_syntax.json
```