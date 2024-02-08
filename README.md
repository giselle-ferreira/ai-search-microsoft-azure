# ai-search-microsoft-azure

- Passo a passo de experimento utilizando **Azure Ai Search** indexação e extração de dados. 
- Realizado como desafio de projeto no Bootcamp **Microsoft Azure AI Fundamentals** da [Dio.me](https://dio.me)
- Documentação: [https://aka.ms/ai900-ai-search](https://aka.ms/ai900-ai-search)

<br/>

## Passo 1
- Abrir a página do Portal [https://portal.azure.com/#home](https://portal.azure.com/#home), buscar e selecionar o "Ai Search"

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/8ea85c0c-c98f-43c2-9d44-2f43f407be3f)

## Passo 2
- Clique em "Create" para criar um novo search service e preencha as informações de acordo com a ordem da imagem abaixo:

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/86b08c93-3147-4a37-91ca-53128a62833c)

- Depois que as informações são validadas, é aberta uma tela com as configurações. Clique em "Create".

 ![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/f110f490-edd4-41c5-91b6-81021c99f264)

- Depois da confirmação de criação, clique em "Go to resource"

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/76dc98c8-dd67-49b6-9b08-c10fd5d6285f)

## Passo 3
- Precisamos criar agora um recurso de IA
- De volta à Home do [Portal Azure](https://portal.azure.com/#home), no menu lateral, clique em "Create a resource", escolha "AI + Machine Learning", depois "Azure Ai Services"

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/7aa6d46e-edcc-472b-80ae-66d36258b301)

## Passo 4
- Preenche com as informações segundo a imagem abaixo. Clica em "Review + Create"

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/f56f92eb-7720-4328-8584-119a4df6278d)

- Após validação das informações, clica em "Create"

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/89aceb49-e017-46be-8bdf-eab5af53da45)

- Aguarde até a finalização da criação do recurso.

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/7bf7b2a0-4810-4b9c-89f3-e2c6729c9fee)

## Passo 5
- Agora criaremos uma conta de armazenamento
- Volte à home do [Portal Azure](https://portal.azure.com/#home), busque e selecione "storage accounts"

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/375a3f7e-f4e0-4a6a-86f1-3b1289cba152)

## Passo 6
- Clique então em "Create"

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/e5ec4e33-e8f3-47c3-b69b-94d1ef082498)

- Preencha os dados conforme imagem abaixo. Os demais que não estão numerados, possivelmente já virão preenchidos.

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/8e5cc876-beb7-48c4-a93e-fb740c98dbb6)

- Após a validação dos dados, clique em "Create"

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/130dedb0-475e-4e89-9cdc-8ba82d138cee)

- Depois de criado, clique em "go to resource"

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/1f081965-3967-4bc8-a11b-4f9c7736b3b5)

## Passo 7
- Na tela do storage, no menu lateral esquerdo, procure e selecione a opção "configuration". Ela vai abrir a tela da direita que está sendo mostrada abaixo. Clique para habilitar a opção conforme imagem e clique em "save".

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/100f602c-9db9-48e7-b464-d9ed02291f48)

## Passo 8
- No menu lateral esquerdo, clique em "Containers", depois em "+ containers", que abrirá uma aba lateral, que deve ser preenchida conforme imagem abaixo. Depois clique em "create".

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/50a65a0e-8846-431a-b4c5-4e6952bd7782)

## Passo 9
- Depois de criado, as informações são atualizadas na tela. Selecione para abrir o container.

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/e896d151-f78f-4bc2-b073-a92ea9b8da4f)

## Passo 10
- Em um novo navegador, faça o download do zip contido no link fornecido na documentação: [https://aka.ms/mslearn-coffee-reviews](https://aka.ms/mslearn-coffee-reviews), e extraia os arquivos em uma pasta "reviews"
- Clique então em upload, que abrirá uma aba lateral. Selecione então todos os arquivos descompactados, e clique em "upload"

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/508deac0-ff04-4409-8657-f9a04e6603b1)

-E assim ficam os arquivos carregados
  
![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/98e99fac-abae-44bb-a2d1-93f22ae4ad4d)

## Passo 11
- Agora voltamos ao Ai Search, através do campo de busca.

 ![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/a6f1fdad-4f91-4aaa-85b8-9b46fb31fa2e)

- Selecione o serviço criado anteriormente

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/fc322c64-2ee2-48f1-9f3c-3f9124cf6b3e)

- Clique em "import data"

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/0e17e2bd-c85e-42c6-918b-2e104850e4ea)

## Passo 12
- Selecione o Azure Blob Storage

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/d3b17083-d67e-41f4-a75f-18bcd624aa96)

- Preencha os dados conforme os passos na imagem.
- A informações não presentes nos passos já vêm preenchidas, ou devem ser deixadas em branco.

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/efce68bc-a7c1-43ef-b85e-fb31725508ae)

## Passo 13
- Na aba "Add Cognitive skills (optional)" selecione seu recurso.

![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/ae1ece30-854a-455a-b4ed-3ee6be67bea5)


## Passo 14


## Passo 15






##

## Comentários
Pude perceber que as análise são bem similares e satisfatórias, não importa o idioma que estamos trabalhando, seja inglês, português, espanhol ou francês, confome nos exemplos adicionais que eu trouxe aqui. Não encontrei discrepâncias, e percebi que realmente é uma ferramenta poderosa para empresas no quesito de análise de satisfação dos clientes. 

##

<div align="center">
<p>Made with ❤️ by Giselle Ferreira.</p>
  <p>
    <a href="https://linkedin.com/in/giselleferreiras" target="_blank" >
      <img align="center" height="35" src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="Giselle Ferreira Linkedin" />
    </a>
    <a href="https://instagram.com/giselletech" target="_blank" >
      <img align="center" height="35" src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/Instagram_icon.png/1200px-Instagram_icon.png" alt="Giselle Ferreira Instagram" />
    </a>
  </p>
</div>
