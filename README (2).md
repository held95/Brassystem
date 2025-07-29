# 🩺 Sistema de Relatório Médico - CG e VASC

Este é um sistema desenvolvido em **Streamlit** que permite o carregamento de arquivos `.txt` contendo dados de escala médica dos hospitais **CG** e **VASC**, e gera um relatório detalhado com valores de produção, horas trabalhadas, coordenação, INSS e TED.

---

## ✅ Funcionalidades

- Upload de dois arquivos `.txt` (`cg.txt` e `vasc.txt`)
- Identificação de médicos e horários com base em padrões textuais
- Cálculo de:
  - Horas trabalhadas
  - Valores por hora (úteis e finais de semana)
  - Produção total
  - Coordenação
  - INSS
  - TED
- Visualização dos dados em formato de tabela diretamente no navegador
- Exportação do relatório como **Excel (.xlsx)**
- [Futuramente] Exportação como **PDF**

---

## 🚀 Como usar

### 1. Executar localmente

#### Pré-requisitos

- Python 3.8+
- Instalar as dependências:

```bash
pip install -r requirements.txt
```

#### Executar o app

```bash
streamlit run app.py
```

---

### 2. Executar online (Streamlit Cloud)

- Faça deploy do repositório no [Streamlit Cloud](https://streamlit.io/cloud).
- O app será executado diretamente no navegador, sem necessidade de instalação.

---

## 📂 Estrutura esperada dos arquivos

Os arquivos `.txt` devem conter a escala de médicos, com nomes e horários. Exemplo de linha:

```
7	JOÃO MARCEL 07-19H	MARIA CLARA 13-19H
```

O sistema identifica os nomes e calcula automaticamente as horas com base em padrões fixos.

---

## 📦 Tecnologias usadas

- [Streamlit](https://streamlit.io/)
- [Pandas](https://pandas.pydata.org/)
- [Python](https://www.python.org/)
- [OpenPyXL](https://openpyxl.readthedocs.io/en/stable/)

---

## 📈 Resultados

O relatório final contém as seguintes colunas:

- Arquivo
- Nome
- Total de Vezes
- Fins de Semana
- Dias Úteis
- Horas Trabalhadas
- Valor Hora FDS
- Valor Hora
- Produção
- Coordenação
- INSS
- **TED** (Produção + Coordenação - INSS)

---

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

---

## 🙋‍♂️ Autor

Desenvolvido por **Hélder Corrêa**  
Contato: [LinkedIn](https://www.linkedin.com/in/seu-perfil) | [GitHub](https://github.com/held95)