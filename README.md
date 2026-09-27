# Echo Genius · Laudo de Ecocardiograma Transtorácico

Software de laudos de ecocardiograma que roda **inteiramente no navegador** (um único `index.html`, sem instalação e sem servidor). Versão genérica, para qualquer médico ou instituição configurar o próprio logo, os próprios dados e a própria assinatura.

**Acesse:** https://geniuscosta.github.io/echo-genius/

## O que faz

- **Modos:** Adulto, Pediátrico (Z-scores de Pettersen) e Transesofágico (Ecote).
- **Medidas e cálculos automáticos:** superfície corpórea (DuBois/Haycock), massa e índices do VE, ERP, volumes, FE (Teichholz e Simpson), índices do AE/AD, aorta indexada, E/e′, PSAP.
- **Descrição e conclusão automáticas**, editáveis, com referências ASE/EACVI.
- **Importação PACS** (botão **PACS**, `Ctrl+I`): lê o REPORT em PDF ou o DICOM SR do aparelho (testado com Philips Affiniti 70) e preenche as medidas.
- **PDF e impressão** em folha A4, com banco de pacientes local.

## Configuração: logo, médico e assinatura

Clique em **⚙ Médico / Logo** na barra superior:

| Campo | Onde aparece no laudo |
|---|---|
| **Logo** (JPEG ou PNG) | Centralizado no topo de todas as páginas, sobre fundo branco (até 9,5 × 3 cm) |
| **Nome** e **CRM** | Abaixo da linha de assinatura, em negrito; o nome também vai para o campo "Médico" |
| **Especialidades / RQE** | Uma por linha, em itálico, abaixo do nome |
| **Cidade** | Rodapé com a data (ex.: "Salvador-Bahia, 27 de setembro de 2026.") |
| **Assinatura digitalizada** (opcional) | Rubrica sobre a linha de assinatura |

- **Assinatura:** o ideal é um PNG com fundo transparente. Um JPEG com fundo branco também funciona, porque o branco é removido automaticamente.
- **Onde fica salvo:** as configurações ficam **no próprio navegador**. Em outro computador ou navegador, é preciso configurar de novo.

## Guia rápido

> Este guia também está dentro do programa: botão **❓ Ajuda** na barra superior (ou tecla **F1**).

**Acesso:** https://geniuscosta.github.io/echo-genius/, no **Google Chrome** ou no **Microsoft Edge**.

**Primeira vez: configure seus dados.** Clique em **⚙ Médico / Logo** e preencha logo da clínica (JPEG ou PNG), nome, CRM, especialidades/RQE (uma por linha), cidade e, se quiser, a assinatura digitalizada. Clique em **Salvar**: fica gravado neste computador.

**Fazendo o laudo**
1. **Novo** limpa o laudo anterior.
2. **Identificação:** nome, idade, **sexo** (obrigatório, porque muda as referências), peso e altura.
3. **Medidas:** digite ou clique em **PACS** para importar do aparelho. Para criança, clique em **Pediátrico** *antes* de importar.
4. **Descrição:** marque os achados nos botões. O texto se monta sozinho e pode ser editado.
5. **Conclusão:** gerada automaticamente; edite se precisar.
6. **PDF** ou **Imprimir**. **Salvar** guarda o paciente no **Banco**.

**Atalhos:** `Ctrl+N` novo · `Ctrl+I` PACS · `Ctrl+S` salvar · `Ctrl+Shift+S` PDF · `Ctrl+P` imprimir · `Ctrl+L` banco · `F1` ajuda

**Importante**
- **Revise sempre** os valores importados e os textos automáticos antes de liberar o laudo.
- Seus dados e os pacientes ficam **só no seu navegador**: nada vai para a internet.
- **Computador compartilhado:** cada médico deve usar o **próprio perfil** do Chrome ou do Edge. Senão, um sobrescreve a configuração do outro.
- **Limpar os dados do navegador** apaga a configuração e o Banco.

Também funciona abrindo o `index.html` direto do computador. O botão "Pasta…", que salva os PDFs numa pasta, funciona melhor no Edge.

## Privacidade

Os dados dos pacientes **não saem do computador**: tudo é processado e guardado no navegador (localStorage). Nada é enviado a servidores. O leitor de PDF e as bibliotecas de geração de PDF são carregados de CDN público (cdnjs).

## Aviso

Ferramenta de apoio à elaboração de laudos. Os valores importados e os textos automáticos **devem ser revisados pelo médico responsável** antes da liberação do laudo.

---
Software de laudos Echo Genius® · Desenvolvido pelo Dr. Genius Costa
