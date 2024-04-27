# Transformers

Use self, and cross attention to learn query, key, values(embedding) triplets for context generation

![transformer](https://machinelearningmastery.com/wp-content/uploads/2021/08/attention_research_1.png)


I use scaled dot product attention, although it can be easily changed to Additive attention


![scale](scaled.png)


Transformers have the advantage of having no recurrent units, and thus requires less training time than previous recurrent neural architectures, "Wikipedia"

Config::


{
    'seq_len': 350,
    'd_model': 512,
    'lang_src': 'en',
    'lang_tgt': 'it',
    'batch_size': 8,
    'num_epochs': 20,
    'lr': 1e-4
}
Uses multi head attention for internal context


![mha](mha.png)
