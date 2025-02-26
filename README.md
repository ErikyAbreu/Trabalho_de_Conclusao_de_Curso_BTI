# **AVALIAÇÃO DAS AÇÕES DE APOIO AO ENSINO DE MATEMÁTICA DISCRETA NA UFERSA - CAMPUS PAU DOS FERROS:** IMPACTOS NO DESEMPENHO ACADÊMICO 

## 🎯 Objetivos

Este repositório tem como objetivo servir como um pacote de replicação para o Trabalho de Conclusão de Curso (TCC) do curso de Bacharelado em Tecnologia da Informação do discente Eriky Veloso.
A estrutura do repositório está organizada da seguinte forma:
- Pasta "Artefatos": Contém os formulários e modelos de planilhas utilizados na pesquisa.
- Pasta "Desenvolvimento": Reúne a análise e o tratamento dos dados, realizados por meio da biblioteca Pandas, da linguagem de programação Python, com o auxílio da plataforma Google Colab.
Essa organização facilita a replicação e compreensão dos procedimentos adotados ao longo do estudo.

## 📌 Passo a Passo para Replicar

### 1️⃣ Preenchimento do Arquivo na Pasta "Artefatos"
1. Acesse a pasta **"Artefatos"** no seu diretório.
2. Localize o arquivo “modelo_de_planilha”.
3. Insira os dados necessários conforme as diretrizes do projeto.
4. Salve o arquivo.
 5.Converta na extensão .csv antes de prosseguir para o próximo passo.

---

### 2️⃣ Upload da Planilha no Google Drive
1. Acesse sua conta do **Google Drive** ([drive.google.com](https://drive.google.com/)).
2. Clique no botão **"Novo"** > **"Upload de Arquivo"**.
3. Selecione a planilha preenchida e aguarde o upload ser concluído.
4. Após o upload, clique com o botão direito sobre a planilha e selecione **"Obter link"**.
5. Copie o caminho do arquivo para usá-lo mais tarde no Google Colab.

---

### 3️⃣ Cópia do Código para o Google Colab
1. Acesse o **Google Colab** através do link: [Google Colab](https://colab.google/).
2. Localize o código que deseja copiar (analise_dos_dados_pacote_de_replicacao.ipynb).
3. Faça uma cópia do notebook.

---

### 4️⃣ Ajuste das Importações no Código

No Google Colab, localize o trecho do código responsável por importar a base de dados:

```python
# IMPORTANDO A BASE DE DADOS UTILIZADA
tabela_alunos = pd.read_csv("/content/drive/MyDrive/CAMINHO/NOME_DO_ARQUIVO.csv")
display(tabela_alunos)
quant_dados = 00  # INFORME A QUANTIDADE DE DADOS OBTIDOS
```

#### 🔹 Modificações necessárias:
- **Substitua** `"/content/drive/MyDrive/CAMINHO/NOME_DO_ARQUIVO.csv"` pelo **caminho exato** da planilha no Google Drive.
  - Exemplo:
    ```python
    tabela_alunos = pd.read_csv("/content/drive/MyDrive/MeuProjeto/Dados/alunos.csv")
    ```
- **Troque** `00` pelo número de registros contidos na planilha.
  - Exemplo:
    ```python
    quant_dados = 250  # Se houver 250 registros na planilha
    ```

---

### 5️⃣ Executando o Código no Google Colab
1. Após realizar as modificações, clique no botão **"Executar"** na célula de código.
2. O Google Colab pedirá **permissão para acessar seu Google Drive**.
3. Faça login na sua conta do Google e conceda as permissões necessárias.
4. Aguarde a execução e verifique se os dados foram importados corretamente.

Agora o seu código está pronto para ser utilizado no Google Colab com os dados atualizados! 

## 📖 Resumo

Este trabalho diz respeito à realização de um estudo sobre os efeitos de ações de apoio ao ensino da componente curricular Matemática Discreta (MD), nos discentes da Universidade Federal Rural do Semi-Árido (Ufersa) campus Pau dos Ferros para verificar, por meio de análises estatísticas, o impacto das ações de apoio na melhora do rendimento acadêmico. A pesquisa utiliza uma abordagem quantitativa, aplicando métodos estatísticos, como regressão linear e análise do coeficiente de determinação, para correlacionar o número de participação nas atividades do projeto com as notas obtidas nas avaliações formais. Os dados foram coletados por meio de questionários aplicados durante o Projeto de Ações de Apoio à Melhoria do Ensino de Graduação (AAMEG), seguido de uma análise estatística, auxiliada pela linguagem de programação Python, para identificar padrões de desempenho. Os resultados indicam que há uma correlação positiva entre a quantidade de atividades realizadas e o rendimento dos discentes, evidenciando que os alunos que participaram ativamente das ações de apoio apresentaram melhores resultados nas avaliações. Conclui-se que as estratégias de apoio pedagógico podem ser uma ferramenta eficaz para reduzir a taxa de desistência e reprovação, além de melhorar a compreensão do conteúdo da disciplina. Com base nos resultados, recomenda-se a continuidade e o aprimoramento dessas ações, a fim de promover um ambiente de aprendizagem mais inclusivo e eficaz.

