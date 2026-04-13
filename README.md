# 📘 Projeto GEA - Guia de Ensino Aprendizagem

Autores:
3 ano - Curso Técnico de Informática - EE Geraldo Jardim Linhares

> **Status do Projeto:** 🚀 Em Desenvolvimento (Versão v1_30032026)  
> **Instituição:** Escola Geraldo Jardim Linhares  
> **Modelo Pedagógico:** Inspirado na *Escola da Escolha* (ICE)

---

## 📝 Descrição do Projeto
Este projeto visa a **automatização** do preenchimento e gestão do Guia de Ensino e de Aprendizagem. [cite_start]O objetivo é substituir o processo manual (arquivos Word e e-mails) por uma interface web integrada a um banco de dados (planilha), garantindo a integridade dos dados e facilitando a análise pedagógica. [cite: 1]

---

## 🔄 Fluxo de Processos

### ❌ Como é hoje (Problema)
O fluxo atual gera múltiplas versões e dificulta a centralização:
`Professor (Word) ➔ Cópia Manual ➔ E-mail ➔ Coordenador (Download/Cópia) ➔ Drive Local` 📉

### ✅ Como será (Solução)
Interface centralizada para maior agilidade:
`Professor ➔ Interface Web (Formulário GEA) ➔ Banco de Dados (Planilha) ➔ Dashboard da Coordenação` 📈


---

## 🛠️ Estrutura do Guia (Seções)

O formulário está dividido em quatro pilares fundamentais para o Ensino Médio Integral:

1.  [cite_start]**🆔 Identificação**: Dados do docente, turma, componente e bimestre. [cite: 1]
2.  [cite_start]**🧠 Fundamentação**: Justificativa, conteúdos e habilidades (Cognitivas e Socioemocionais). [cite: 1]
3.  **🤝 Situações Didáticas**: 
    * [cite_start]*Prévias*: Mobilização de conhecimento. [cite: 1]
    * [cite_start]*Autodidáticas*: Foco na autonomia. [cite: 1]
    * [cite_start]*Didático-Cooperativas*: Trabalho em equipe. [cite: 1]
    * [cite_start]*Complementares*: Expansão do conteúdo. [cite: 1]
4.  [cite_start]**⚙️ Operacionalização**: Práticas, espaços, recursos e avaliação. [cite: 1]

---

## 💻 Implementação Técnica (Google Apps Script)

[cite_start]O sistema utiliza a função `gerarFormularioGuia()` para criar dinamicamente o formulário com as validações necessárias. [cite: 1]

```javascript
// Exemplo de trecho do código de automação
function gerarFormularioGuia() {
  var form = FormApp.create('Guia de Ensino e de Aprendizagem');
  form.addTextItem().setTitle('Professor').setRequired(true);
  // ... (restante do código no arquivo)
}
```

---

## 📋 Requisitos do Sistema

| Tipo | Descrição |
| :--- | :--- |
| **RF01** | [cite_start]Coleta de identificação completa (Professor/Turma/Matéria) [cite: 1] |
| **RF05** | [cite_start]Segmentação de atividades em 4 categorias didáticas [cite: 1] |
| **RNF01** | [cite_start]Interface intuitiva com quebras de página por seção [cite: 1] |
| **RNF02** | [cite_start]Fidelidade total ao modelo de Antônio Carlos Gomes da Costa [cite: 1] |

---

## ⚖️ Regras de Validação (Qualidade)

Para garantir que o planejamento seja eficaz, o sistema valida:
* [cite_start]**Justificativa**: Mínimo de 50 caracteres. [cite: 1]
* [cite_start]**Habilidades**: Recomendado uso de códigos da **BNCC**. [cite: 1]
* [cite_start]**Atividades**: Verificação obrigatória de menção a trabalhos em grupo nas didático-cooperativas. [cite: 1]
* [cite_start]**Datas**: Referência estrita ao bimestre letivo vigente. [cite: 1]

---

## 📚 Referências Bibliográficas
* [cite_start]*COSTA, Antônio Carlos Gomes da.* (Concepção original do Guia). [cite: 1]
* [cite_start]*Caderno de Formação: Espaços Educativos e Gestão do Ensino e da Aprendizagem* (pág. 25). [cite: 1]

---
⭐ **Desenvolvido para transformar a educação através da tecnologia.**
