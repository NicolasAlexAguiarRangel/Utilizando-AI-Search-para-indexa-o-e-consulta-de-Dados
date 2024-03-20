# Utilizando-AI-Search-para-indexa-o-e-consulta-de-Dados

# 1 Crie um recurso do Azure AI Search
Entre no portal do Azure .

// ----Clique no botão + Criar um recurso , pesquise Azure AI Search e crie um recurso Azure AI Search com as seguintes configurações:

1.1 Assinatura : sua assinatura do Azure .
1.2 Grupo de recursos : selecione ou crie um grupo de recursos com um nome exclusivo .
1.3 Nome do serviço : um nome exclusivo .
1.4 Localização : Escolha qualquer região disponível .
1.5 Nível de preços : Básico
1.6 Selecione Review + create e depois de ver a resposta Validation Success , selecione Create .

// --- Após a conclusão da implantação, selecione Ir para o recurso . Na página de visão geral do Azure AI Search, você pode adicionar índices, importar dados e pesquisar índices criados.

2- Crie um recurso de serviços de IA do Azure

//----- Você precisará provisionar um recurso de serviços de IA do Azure que esteja no mesmo local que seu recurso do Azure AI Search. Sua solução de pesquisa usará esse recurso para enriquecer os dados no armazenamento de dados com insights gerados por IA.

2.1- Retorne à página inicial do portal do Azure. Clique no botão ＋Criar um recurso e pesquise os serviços de IA do Azure . Selecione 2.2- criar um plano de serviços de IA do Azure . Você será levado a uma página para criar um recurso de serviços de IA do Azure. 
2.3- Configure-o com as seguintes configurações:
2.4- Assinatura : sua assinatura do Azure .
2.5- Grupo de recursos : O mesmo grupo de recursos que seu recurso do Azure AI Search .
2.6- Região : o mesmo local do recurso do Azure AI Search .
2.7- Nome : Um nome exclusivo .
2.8- Nível de preços : Padrão S0
2.9- Ao marcar esta caixa, confirmo que li e compreendi todos os termos abaixo : Selecionado
2.10- Selecione Revisar + criar . Depois de ver a resposta Validation Passed , selecione Create .

Aguarde a conclusão da implantação e visualize os detalhes da implantação.

3- Crie uma conta de armazenamento
Retorne à página inicial do portal do Azure e selecione o botão + Criar um recurso .

3.1- Procure conta de armazenamento e crie um recurso de conta de armazenamento com as seguintes configurações:
3.2- Assinatura : sua assinatura do Azure .
3.3- Grupo de recursos : O mesmo grupo de recursos que os recursos do Azure AI Search e dos serviços Azure AI .
3.4- Nome da conta de armazenamento : um nome exclusivo .
3.5-Localização : Escolha qualquer localização disponível .
3.6- Padrão de desempenho
3.7- Redundância : armazenamento localmente redundante (LRS)
3.8- Clique em Revisar e em Criar . Aguarde a conclusão da implantação e vá para o recurso implantado.

Na conta de Armazenamento do Azure que você criou, no painel de menu esquerdo, selecione Configuração (em Configurações ).
Altere a configuração de Permitir acesso anônimo de Blob para Habilitado e selecione Salvar .

# Carregar documentos para o armazenamento do Azure

1- No painel do menu esquerdo, selecione Containers .

<img src="">
