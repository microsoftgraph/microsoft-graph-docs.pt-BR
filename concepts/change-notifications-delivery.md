---
title: Receba notificações de alterações de maneiras diferentes
description: As notificações de alteração podem ser enviadas por meio de tecnologias diferentes, incluindo o webhooks e Hubs de Eventos do Azure.
author: Jumaodhiss
localization_priority: Priority
ms.custom: graphiamtop20, devx-track-azurecli
ms.openlocfilehash: 2cb6000b309b9bcaf5af840cc26976c7254d2d96
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469098"
---
# <a name="get-change-notifications-delivered-in-different-ways-preview"></a><span data-ttu-id="ade04-103">Receba notificações sobre alterações por diferentes maneiras de envio(versão prévia)</span><span class="sxs-lookup"><span data-stu-id="ade04-103">Get change notifications delivered in different ways (preview)</span></span>

<span data-ttu-id="ade04-104">A alteração de notificações podem ser enviadas em diferentes maneiras aos assinantes.</span><span class="sxs-lookup"><span data-stu-id="ade04-104">Change notifications can be delivered in different ways to subscribers.</span></span> <span data-ttu-id="ade04-105">Se o principal modo de entrega para notificações de alteração for por meio de webhooks, pode ser desafiador tirar proveito de webhooks para cenários de alto rendimento ou quando o receptor não pode expor uma URL de notificação disponível publicamente.</span><span class="sxs-lookup"><span data-stu-id="ade04-105">If the main delivery mode for change notifications is through webhooks, it can be challenging to take advantage of webhooks for high throughput scenarios or when the receiver cannot expose a publicly available notification URL.</span></span>  

<span data-ttu-id="ade04-106">Esse modo de entrega de notificações de alterações está disponível para todos os recursos que oferecem suporte a notificações de alterações do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ade04-106">This change notifications delivery mode is available for all resources that support Microsoft Graph change notifications.</span></span>

<span data-ttu-id="ade04-107">Bons exemplos de cenários de alta produtividade incluem aplicações que subscrevem um grande conjunto de recursos, aplicações que subscrevem recursos que mudam com uma alta frequência e aplicações multi-locatárias que subscrevem recursos através de um grande conjunto de organizações.</span><span class="sxs-lookup"><span data-stu-id="ade04-107">Good examples of high throughput scenarios include applications subscribing to a large set of resources, applications subscribing to resources that change with a high frequency, and multi-tenant applications that subscribe to resources accross a large set of organizations.</span></span>

## <a name="using-azure-event-hubs-to-receive-change-notifications"></a><span data-ttu-id="ade04-108">Usando os Hubs de Eventos do Azure para receber notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="ade04-108">Using Azure Event Hubs to receive change notifications</span></span>

<span data-ttu-id="ade04-109">Os [Hubs de Eventos do Azure](https://azure.microsoft.com/services/event-hubs) é um serviço popular de inclusão e distribuição de eventos em tempo real, compilado para ser dimensionável.</span><span class="sxs-lookup"><span data-stu-id="ade04-109">[Azure Event Hubs](https://azure.microsoft.com/services/event-hubs) is a popular real-time events ingestion and distribution service built for scale.</span></span> <span data-ttu-id="ade04-110">Você pode usar os Hubs de Eventos do Azure, em vez de webhooks tradicionais, para receber notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="ade04-110">You can use Azure Events Hubs instead of traditional webhooks to receive change notifications.</span></span> <span data-ttu-id="ade04-111">Este recurso está atualmente no modo de visualização.</span><span class="sxs-lookup"><span data-stu-id="ade04-111">This feature is currently in preview.</span></span>  
<span data-ttu-id="ade04-112">Usar os Hubs de Eventos do Azure para receber notificações de alteração difere do webhooks em algumas maneiras, incluindo:</span><span class="sxs-lookup"><span data-stu-id="ade04-112">Using Azure Event Hubs to receive change notifications differs from webhooks in a few ways, including:</span></span>

- <span data-ttu-id="ade04-113">Você não depende de URLs com notificações publicamente expostas.</span><span class="sxs-lookup"><span data-stu-id="ade04-113">You don't rely on publicly exposed notification URLs.</span></span> <span data-ttu-id="ade04-114">O SDK do Hubs de Eventos retransmitirá as notificações para sua aplicação.</span><span class="sxs-lookup"><span data-stu-id="ade04-114">The Event Hubs SDK will relay the notifications to your application.</span></span>
- <span data-ttu-id="ade04-115">Não é necessário responder à [validação da URL de notificação](webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="ade04-115">You don't need to reply to the [notification URL validation](webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="ade04-116">Você pode ignorar a mensagem de validação recebida.</span><span class="sxs-lookup"><span data-stu-id="ade04-116">You can ignore the validation message that you receive.</span></span>
- <span data-ttu-id="ade04-117">Você precisará de provisionar um Hub de Eventos do Azure.</span><span class="sxs-lookup"><span data-stu-id="ade04-117">You'll need to provision an Azure Event Hub.</span></span>
- <span data-ttu-id="ade04-118">Você precisará de provisionar um Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="ade04-118">You'll need to provision an Azure Key Vault.</span></span>

### <a name="set-up-the-azure-keyvault-and-azure-event-hubs"></a><span data-ttu-id="ade04-119">Configurar o Cofre de Chaves do Azure e os Hubs de Eventos do Azure</span><span class="sxs-lookup"><span data-stu-id="ade04-119">Set up the Azure KeyVault and Azure Event Hubs</span></span>

<span data-ttu-id="ade04-120">Esta seção vai orientá-lo a configurar os necessários serviços do Azure.</span><span class="sxs-lookup"><span data-stu-id="ade04-120">This section will walk you through the setup of required Azure services.</span></span>

#### <a name="option-1-using-the-azure-cli"></a><span data-ttu-id="ade04-121">Opção 1: Usando o CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="ade04-121">Option 1: Using the Azure CLI</span></span>

<span data-ttu-id="ade04-122">O [CLI do Azure](/cli/azure/what-is-azure-cli) permite que você escreva o script e automatize tarefas administrativas no Azure.</span><span class="sxs-lookup"><span data-stu-id="ade04-122">The [Azure CLI](/cli/azure/what-is-azure-cli) allows you to script and automate adminstrative tasks in Azure.</span></span> <span data-ttu-id="ade04-123">O CLI pode ser [instalado em seu computador local](/cli/azure/install-azure-cli) ou ser executado diretamente a partir do [Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="ade04-123">The CLI can be [installed on your local computer](/cli/azure/install-azure-cli) or run directly from the [Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

```azurecli
# --------------
# TODO: update the following values
#sets the name of the resource group
resourcegroup=rg-graphevents-dev
#sets the location of the resources
location='uk south'
#sets the name of the Azure Event Hubs namespace
evhamespacename=evh-graphevents-dev
#sets the name of the hub under the namespace
evhhubname=graphevents
#sets the name of the access policy to the hub
evhpolicyname=grapheventspolicy
#sets the name of the Azure KeyVault
keyvaultname=kv-graphevents
#sets the name of the secret in Azure KeyVault that will contain the connection string to the hub
keyvaultsecretname=grapheventsconnectionstring
# --------------
az group create --location $location --name $resourcegroup
az eventhubs namespace create --name $evhamespacename --resource-group $resourcegroup --sku Basic --location $location
az eventhubs eventhub create --name $evhhubname --namespace-name $evhamespacename --resource-group $resourcegroup --partition-count 2 --message-retention 1
az eventhubs eventhub authorization-rule create --name $evhpolicyname --eventhub-name $evhhubname --namespace-name $evhamespacename --resource-group $resourcegroup --rights Send
evhprimaryconnectionstring=`az eventhubs eventhub authorization-rule keys list --name $evhpolicyname --eventhub-name $evhhubname --namespace-name $evhamespacename --resource-group $resourcegroup --query "primaryConnectionString" --output tsv`
az keyvault create --name $keyvaultname --resource-group $resourcegroup --location $location --enable-soft-delete true --sku standard --retention-days 90
az keyvault secret set --name $keyvaultsecretname --value $evhprimaryconnectionstring --vault-name $keyvaultname --output none
graphspn=`az ad sp list --display-name 'Microsoft Graph Change Tracking' --query "[].appId" --output tsv`
az keyvault set-policy --name $keyvaultname --resource-group $resourcegroup --secret-permissions get --spn $graphspn --output none
keyvaulturi=`az keyvault show --name $keyvaultname --resource-group $resourcegroup --query "properties.vaultUri" --output tsv`
domainname=`az ad signed-in-user show --query 'userPrincipalName' | cut -d '@' -f 2 | sed 's/\"//'`
notificationUrl="EventHub:${keyvaulturi}secrets/${keyvaultsecretname}?tenantId=${domainname}"
echo "Notification Url:\n${notificationUrl}"
```

> <span data-ttu-id="ade04-124">**Observação:** O script fornecido aqui é compatível com shells baseados em Linux, Windows WSL e Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="ade04-124">**Note:** The script provided here is compatible with Linux based shells, Windows WSL, and Azure Cloud Shell.</span></span> <span data-ttu-id="ade04-125">Será necessário algumas atualizações para executar shells do Windows.</span><span class="sxs-lookup"><span data-stu-id="ade04-125">It will require some updates to run in Windows shells.</span></span>

#### <a name="option-2-using-the-azure-portal"></a><span data-ttu-id="ade04-126">Opção 2: Usando o Portal do Azure</span><span class="sxs-lookup"><span data-stu-id="ade04-126">Option 2: Using the Azure Portal</span></span>

##### <a name="configuring-the-azure-event-hub"></a><span data-ttu-id="ade04-127">Configurando o Hub de eventos do Azure</span><span class="sxs-lookup"><span data-stu-id="ade04-127">Configuring the Azure Event Hub</span></span>

<span data-ttu-id="ade04-128">Nesta seção, você vai:</span><span class="sxs-lookup"><span data-stu-id="ade04-128">In this section you will:</span></span>

- <span data-ttu-id="ade04-129">Criar um namespace do Hub de Eventos do Azure.</span><span class="sxs-lookup"><span data-stu-id="ade04-129">Create an Azure Event Hub namespace.</span></span>
- <span data-ttu-id="ade04-130">Adicionar um hub para este namespace que irá transmitir e entregar notificações.</span><span class="sxs-lookup"><span data-stu-id="ade04-130">Add a hub to that namespace that will relay and deliver notifications.</span></span>
- <span data-ttu-id="ade04-131">Adicionar uma política de acesso compartilhado que permita obter uma cadeia de conexão para o hub recém-criado.</span><span class="sxs-lookup"><span data-stu-id="ade04-131">Add a shared access policy that will allow you to get a connection string to the newly created hub.</span></span>

<span data-ttu-id="ade04-132">Etapas:</span><span class="sxs-lookup"><span data-stu-id="ade04-132">Steps:</span></span>

1. <span data-ttu-id="ade04-133">Abra um navegador para o [Portal do Azure](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="ade04-133">Open a browser to the [Azure Portal](https://portal.azure.com).</span></span>
1. <span data-ttu-id="ade04-134">Selecione **Criar um recurso**.</span><span class="sxs-lookup"><span data-stu-id="ade04-134">Select **Create a resource**.</span></span>
1. <span data-ttu-id="ade04-135">Digite **Hubs de Evento** na barra de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="ade04-135">Type **Event Hubs** in the search bar.</span></span>
1. <span data-ttu-id="ade04-136">Selecione a sugestão **Hubs de Eventos**.</span><span class="sxs-lookup"><span data-stu-id="ade04-136">Select the **Event Hubs** suggestion.</span></span> <span data-ttu-id="ade04-137">A página de criação dos Hubs de Evento será carregada.</span><span class="sxs-lookup"><span data-stu-id="ade04-137">The Event Hubs creation page will load.</span></span>  
1. <span data-ttu-id="ade04-138">Na página de criação dos Hubs de Evento clique **criar**.</span><span class="sxs-lookup"><span data-stu-id="ade04-138">On the Event Hubs creation page, click **Create**.</span></span>
1. <span data-ttu-id="ade04-139">Preencha os detalhes da criação no namespace dos Hubs de Eventos e clique em **Criar**.</span><span class="sxs-lookup"><span data-stu-id="ade04-139">Fill in the Event Hubs namespace creation details, and then click **Create**.</span></span>  
1. <span data-ttu-id="ade04-140">Quando o namespace do Hub de Eventos for provisionado, vá para a página do namespace.</span><span class="sxs-lookup"><span data-stu-id="ade04-140">When the Event Hub namespace is provisioned, go to the page for the namespace.</span></span>  
1. <span data-ttu-id="ade04-141">Clique em **Hubs de Eventos** e **+ Hub de Eventos**.</span><span class="sxs-lookup"><span data-stu-id="ade04-141">Click **Event Hubs** and **+ Event Hub**.</span></span>  
1. <span data-ttu-id="ade04-142">Dê um nome para o novo Hub de Eventos e clique em **Criar**.</span><span class="sxs-lookup"><span data-stu-id="ade04-142">Give a name to the new Event Hub, and click **Create**.</span></span>  
1. <span data-ttu-id="ade04-143">Depois que o Hub de Eventos foi criado, clique no nome do Hub de Eventos e, em seguida, clique em **Políticas de acesso compartilhado** e **+ Adicionar** para adicionar uma nova política.</span><span class="sxs-lookup"><span data-stu-id="ade04-143">After the Event Hub has been created, click the name of the Event Hub, and then click **Shared access policies** and **+ Add** to add a new policy.</span></span>  
1. <span data-ttu-id="ade04-144">Dê um nome à política, marque **Enviar**, e clique em **Criar**.</span><span class="sxs-lookup"><span data-stu-id="ade04-144">Give a name to the policy, check **Send**, and click **Create**.</span></span>  
1. <span data-ttu-id="ade04-145">Depois de criar a política, clique no nome da política para abrir o painel de detalhes e, em seguida, copie o valor da **Chave principal da cadeia de conexão**.</span><span class="sxs-lookup"><span data-stu-id="ade04-145">After the policy has been created, click the name of the policy to open the details panel, and then copy the **Connection string-primary key** value.</span></span> <span data-ttu-id="ade04-146">Anote-o; você precisará dele para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="ade04-146">Write it down; you'll need it for the next step.</span></span>  

##### <a name="configuring-the-azure-key-vault"></a><span data-ttu-id="ade04-147">Configurando o Azure Key Vault</span><span class="sxs-lookup"><span data-stu-id="ade04-147">Configuring the Azure Key Vault</span></span>

<span data-ttu-id="ade04-148">Para acessar o Hub de Eventos de forma segura e permitir rotações de chaves, o Microsoft Graph obtém a cadeia de conexão para o Hub de Eventos através do Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="ade04-148">In order to access the Event Hub securely and to allow for key rotations, Microsoft Graph gets the connection string to the Event Hub through Azure Key Vault.</span></span>  
<span data-ttu-id="ade04-149">Nesta seção, você vai:</span><span class="sxs-lookup"><span data-stu-id="ade04-149">In this section, you will:</span></span>

- <span data-ttu-id="ade04-150">Criar um Azure Key Vault para armazenar segredo.</span><span class="sxs-lookup"><span data-stu-id="ade04-150">Create an Azure Key Vault to store secret.</span></span>
- <span data-ttu-id="ade04-151">Adicionar a cadeia de conexão ao Hub de Evento como um segredo.</span><span class="sxs-lookup"><span data-stu-id="ade04-151">Add the connection string to the Event Hub as a secret.</span></span>
- <span data-ttu-id="ade04-152">Adicionar uma política de acesso para o Microsoft Graph acessar o segredo.</span><span class="sxs-lookup"><span data-stu-id="ade04-152">Add an access policy for Microsoft Graph to access the secret.</span></span>

<span data-ttu-id="ade04-153">Etapas:</span><span class="sxs-lookup"><span data-stu-id="ade04-153">Steps:</span></span>

1. <span data-ttu-id="ade04-154">Abra um navegador para o [Portal do Azure](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="ade04-154">Open a browser to the [Azure Portal](https://portal.azure.com).</span></span>
1. <span data-ttu-id="ade04-155">Selecione **Criar um recurso**.</span><span class="sxs-lookup"><span data-stu-id="ade04-155">Select **Create a resource**.</span></span>
1. <span data-ttu-id="ade04-156">Digite **Cofre de Chaves** na barra de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="ade04-156">Type **Key Vault** in the search bar.</span></span>
1. <span data-ttu-id="ade04-157">Selecione a sugestão do **Cofre de Chaves**.</span><span class="sxs-lookup"><span data-stu-id="ade04-157">Select the **Key Vault** suggestion.</span></span> <span data-ttu-id="ade04-158">A página de criação do Cofre de Chaves será carregada.</span><span class="sxs-lookup"><span data-stu-id="ade04-158">The Key Vault creation page will load.</span></span>
1. <span data-ttu-id="ade04-159">Na página de criação do Cofre de Chaves clique **criar**.</span><span class="sxs-lookup"><span data-stu-id="ade04-159">On the Key Vault creation page, click **Create**.</span></span>  
1. <span data-ttu-id="ade04-160">Preencha os detalhes da criação do cofre de chaves e, em seguida, clique em **Revisar + Criar** e **Criar**.</span><span class="sxs-lookup"><span data-stu-id="ade04-160">Fill in the Key Vault creation details, and then click **Review + Create** and **Create**.</span></span>  
1. <span data-ttu-id="ade04-161">Vá para o cofre de chaves recém-criado usando **Ir para o recurso** da notificação.</span><span class="sxs-lookup"><span data-stu-id="ade04-161">Go to the newly crated key vault using the **Go to resource** from the notification.</span></span>  
1. <span data-ttu-id="ade04-162">Copie o **nome do DNS**; você precisará dele para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="ade04-162">Copy the **DNS name**; you will need it for the next step.</span></span>  
1. <span data-ttu-id="ade04-163">Vá para **Segredos** e clique em **+ Gerar/Importar**.</span><span class="sxs-lookup"><span data-stu-id="ade04-163">Go to **Secrets** and click **+ Generate/Import**.</span></span>  
1. <span data-ttu-id="ade04-164">Dê um nome ao segredo e guarde-o para mais tarde; você precisará dele para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="ade04-164">Give a name to the secret, and keep the name for later; you will need it for the next step.</span></span> <span data-ttu-id="ade04-165">Para o valor, cole a cadeia de conexão que você gerou na etapa Hubs de Eventos.</span><span class="sxs-lookup"><span data-stu-id="ade04-165">For the value, paste in the connection string you generated at the Event Hubs step.</span></span> <span data-ttu-id="ade04-166">Clique em **Criar**.</span><span class="sxs-lookup"><span data-stu-id="ade04-166">Click **Create**.</span></span>  
1. <span data-ttu-id="ade04-167">Clique em **Políticas de Acesso** e **+ Adicionar Política de Acesso**.</span><span class="sxs-lookup"><span data-stu-id="ade04-167">Click **Access Policies** and **+ Add Access Policy**.</span></span>  
1. <span data-ttu-id="ade04-168">Para **Permissões de segredo**, selecione **Obter**, e para **Selecionar Principal**, selecione **Controle de Alterações do Microsoft Graph**.</span><span class="sxs-lookup"><span data-stu-id="ade04-168">For **Secret permissions**, select **Get**, and for **Select Principal**, select **Microsoft Graph Change Tracking**.</span></span> <span data-ttu-id="ade04-169">Clique em **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="ade04-169">Click **Add**.</span></span>  

### <a name="creating-the-subscription-and-receiving-notifications"></a><span data-ttu-id="ade04-170">Criando a assinatura e recebendo notificações</span><span class="sxs-lookup"><span data-stu-id="ade04-170">Creating the subscription and receiving notifications</span></span>

<span data-ttu-id="ade04-171">Depois de você criar os serviços necessários Azure Key Vault e do Hubs de Eventos do Azure, você poderá criar sua assinatura e começar a receber as notificações de alteração por meio dos Hubs de Eventos do Azure.</span><span class="sxs-lookup"><span data-stu-id="ade04-171">After you create the required Azure KeyVault and Azure Event Hubs services, you will be able to create your subscription and start receiving change notifications via Azure Event Hubs.</span></span>

#### <a name="creating-the-subcription"></a><span data-ttu-id="ade04-172">Criando a assinatura</span><span class="sxs-lookup"><span data-stu-id="ade04-172">Creating the subcription</span></span>

<span data-ttu-id="ade04-173">As assinaturas para alterar as notificações com os Hubs de Eventos são quase idênticas como alterar as notificações com webhooks.</span><span class="sxs-lookup"><span data-stu-id="ade04-173">Subscriptions to change notifications with Event Hubs are almost identical to change notifications with webhooks.</span></span> <span data-ttu-id="ade04-174">A principal diferença é que elas dependem dos Hubs de Eventos para entregar notificações.</span><span class="sxs-lookup"><span data-stu-id="ade04-174">The key difference is that they rely on Event Hubs to deliver notifications.</span></span> <span data-ttu-id="ade04-175">Todas as outras operações são similares, inclusive a [criação de assinatura](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="ade04-175">All other operations are similar, including [subscription creation](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span></span>  

<span data-ttu-id="ade04-176">A principal diferença durante a criação da assinatura será o **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="ade04-176">The main difference during subscription creation will be the **notificationUrl**.</span></span> <span data-ttu-id="ade04-177">Você deve defini-lo para `EventHub:https://<azurekeyvaultname>.vault.azure.net/secrets/<secretname>?tenantId=<domainname>` os seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="ade04-177">You must set it to `EventHub:https://<azurekeyvaultname>.vault.azure.net/secrets/<secretname>?tenantId=<domainname>`, with the following values:</span></span>

- <span data-ttu-id="ade04-178">`azurekeyvaultname` - O nome que você atribuiu ao cofre de chaves quando o criou.</span><span class="sxs-lookup"><span data-stu-id="ade04-178">`azurekeyvaultname` - The name you gave to the key vault when you created it.</span></span> <span data-ttu-id="ade04-179">Pode ser encontrado no nome DNS.</span><span class="sxs-lookup"><span data-stu-id="ade04-179">Can be found in the DNS name.</span></span>
- <span data-ttu-id="ade04-180">`secretname` - O nome que você atribuiu ao segredo quando o criou.</span><span class="sxs-lookup"><span data-stu-id="ade04-180">`secretname` - The name you gave to the secret when you created it.</span></span> <span data-ttu-id="ade04-181">Pode ser encontrado na página **Segredos**. do Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="ade04-181">Can be found on the Azure Key Vault **Secrets** page.</span></span>
- <span data-ttu-id="ade04-182">`domainname` – O nome do seu locatário do. por exemplo, consto.onmicrosoft.com ou contoso.com.</span><span class="sxs-lookup"><span data-stu-id="ade04-182">`domainname` - The name of your tenant; for example, consto.onmicrosoft.com or contoso.com.</span></span> <span data-ttu-id="ade04-183">Como esse domínio será usado para acessar o Azure Key Vault é importante que ele corresponda ao domínio usado pela assinatura do Azure que possui o Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="ade04-183">Because this domain will be used to access the Azure Key Vault, it is important that it matches the domain used by the Azure subscription that holds the Azure Key Vault.</span></span> <span data-ttu-id="ade04-184">Para obter essa informação, você pode ir para a página de visão geral do Azure Key Vault que você criou e clique na assinatura.</span><span class="sxs-lookup"><span data-stu-id="ade04-184">To get this information, you can go to the overview page of the Azure Key Vault you created and click the subscription.</span></span> <span data-ttu-id="ade04-185">O nome de domínio é exibido sob o campo **Diretório**.</span><span class="sxs-lookup"><span data-stu-id="ade04-185">The domain name is displayed under the **Directory** field.</span></span>

#### <a name="receiving-notifications"></a><span data-ttu-id="ade04-186">Recebendo notificações</span><span class="sxs-lookup"><span data-stu-id="ade04-186">Receiving notifications</span></span>

<span data-ttu-id="ade04-187">Os eventos agora serão enviados para o aplicativo através dos Hubs de Eventos.</span><span class="sxs-lookup"><span data-stu-id="ade04-187">Events will be now delivered to your application by Event Hubs.</span></span> <span data-ttu-id="ade04-188">Para detalhes, confira [Recebendo eventos](/azure/event-hubs/get-started-dotnet-standard-send-v2#receive-events) na documentação Hubs de Eventos.</span><span class="sxs-lookup"><span data-stu-id="ade04-188">For details, see [receiving events](/azure/event-hubs/get-started-dotnet-standard-send-v2#receive-events) in the Event Hubs documentation.</span></span>

<span data-ttu-id="ade04-189">Antes de receber as notificações no aplicativo, você precisará criar outra política de acesso compartilhado com uma permissão de "Escuta" e obter a cadeia de conexão, semelhante às etapas listadas em [Configurando o Azure Event Hub](#configuring-the-azure-event-hub).</span><span class="sxs-lookup"><span data-stu-id="ade04-189">Before you can receive the notifications in your application, you'll need to create another shared access policy with a "Listen" permission and obtain the connection string, similar to the steps listed in [Configuring the Azure Event Hub](#configuring-the-azure-event-hub).</span></span>

> <span data-ttu-id="ade04-190">**Observação:** Criar uma política separada para o aplicativo que escuta mensagens de Hubs de Eventos, em vez de reutilizar a mesma cadeia de conexão que você definiu no Azure keyVault.</span><span class="sxs-lookup"><span data-stu-id="ade04-190">**Note:** Create a separate policy for the application that listens to Event Hubs messages instead of reusing the same connection string you set in Azure KeyVault.</span></span> <span data-ttu-id="ade04-191">Isto garante que cada componente da solução tenha apenas as permissões que precisa e siga o princípio de segurança com o mínimo de permissões.</span><span class="sxs-lookup"><span data-stu-id="ade04-191">This ensures that each component of the solution has only the permissions it needs and follows the least permissions security principle.</span></span>

> <span data-ttu-id="ade04-192">**Observação:** Seu aplicativo recebe mensagens de validação sempre que criar uma nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="ade04-192">**Note:** Your application receives validation messages whenever it creates a new subscription.</span></span> <span data-ttu-id="ade04-193">Você deve ignorar essas notificações.</span><span class="sxs-lookup"><span data-stu-id="ade04-193">You should ignore these notifications.</span></span> <span data-ttu-id="ade04-194">O exemplo a seguir representa o corpo de uma mensagem de validação.</span><span class="sxs-lookup"><span data-stu-id="ade04-194">The following example represents the body of a validation message.</span></span>

```json
 {
    "value":[
        {
            "subscriptionId":"NA",
            "subscriptionExpirationDateTime":"NA",
            "clientState":"NA",
            "changeType":"Validation: Testing client application reachability for subscription Request-Id: 522a8e7e-096a-494c-aaf1-ac0dcfca45b7",
            "resource":"NA",
            "resourceData":{
                "@odata.type":"NA",
                "@odata.id":"NA",
                "id":"NA"
            }
        }
    ]
}
```

### <a name="what-happens-if-the-microsoft-graph-change-tracking-application-is-missing"></a><span data-ttu-id="ade04-195">O que acontece se o aplicativo de controle de alterações do Microsoft Graph estiver ausente?</span><span class="sxs-lookup"><span data-stu-id="ade04-195">What happens if the Microsoft Graph change tracking application is missing?</span></span>

<span data-ttu-id="ade04-196">É possível que o serviço principal do **Controle de Alterações do Microsoft Graph** esteja ausente no seu locatário, dependendo de quando o locatário foi criado e de operações administrativas.</span><span class="sxs-lookup"><span data-stu-id="ade04-196">It's possible that the **Microsoft Graph Change Tracking** service principal is missing from your tenant, depending on when the tenant was created and administrative operations.</span></span> <span data-ttu-id="ade04-197">Para resolver este problema, execute [a seguinte consulta](https://developer.microsoft.com/pt-BR/graph/graph-explorer?request=servicePrincipals&method=POST&version=v1.0&GraphUrl=https://graph.microsoft.com&requestBody=eyJhcHBJZCI6IjBiZjMwZjNiLTRhNTItNDhkZi05YTgyLTIzNDkxMGM0YTA4NiJ9) no [Microsoft Graph Explorer](https://developer.microsoft.com/pt-BR/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="ade04-197">To resolve this issue, run [the following query](https://developer.microsoft.com/pt-BR/graph/graph-explorer?request=servicePrincipals&method=POST&version=v1.0&GraphUrl=https://graph.microsoft.com&requestBody=eyJhcHBJZCI6IjBiZjMwZjNiLTRhNTItNDhkZi05YTgyLTIzNDkxMGM0YTA4NiJ9) in [Microsoft Graph Explorer](https://developer.microsoft.com/pt-BR/graph/graph-explorer).</span></span>

<span data-ttu-id="ade04-198">Detalhes da consulta:</span><span class="sxs-lookup"><span data-stu-id="ade04-198">Query details:</span></span>

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals
{
    "appId": "0bf30f3b-4a52-48df-9a82-234910c4a086"
}
```

> <span data-ttu-id="ade04-199">**Observação:** Você pode obter um acesso negado ao executar esta consulta.</span><span class="sxs-lookup"><span data-stu-id="ade04-199">**Note:** You can get an access denied running this query.</span></span> <span data-ttu-id="ade04-200">Neste caso, selecione o ícone de engrenagem ao lado do nome da sua conta no canto superior esquerdo.</span><span class="sxs-lookup"><span data-stu-id="ade04-200">In this case, select the gear icon next to your account name in the top left corner.</span></span> <span data-ttu-id="ade04-201">Em seguida, selecione **Selecionar Permissões** e pesquise **Application.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="ade04-201">Then select **Select Permissions** and search for **Application.ReadWrite.All**.</span></span> <span data-ttu-id="ade04-202">Marque a permissão e selecione **Consentir**.</span><span class="sxs-lookup"><span data-stu-id="ade04-202">Check the permission and select **Consent**.</span></span> <span data-ttu-id="ade04-203">Após o consentimento dessa nova permissão, execute a solicitação novamente.</span><span class="sxs-lookup"><span data-stu-id="ade04-203">After consenting to this new permission, run the request again.</span></span>

> <span data-ttu-id="ade04-204">**Observação:** Esta API só funciona com uma conta corporativa ou de estudante e não com uma conta pessoal.</span><span class="sxs-lookup"><span data-stu-id="ade04-204">**Note:** This API only works with a school or work account, not with a personal account.</span></span> <span data-ttu-id="ade04-205">Certifique-se que você está conectado com uma conta no seu domínio.</span><span class="sxs-lookup"><span data-stu-id="ade04-205">Make sure that you are signed in with an account on your domain.</span></span>

<span data-ttu-id="ade04-206">Como alternativa, você pode usar este script do [Azure Active Directory PowerShell](/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) para adicionar o serviço principal ausente.</span><span class="sxs-lookup"><span data-stu-id="ade04-206">Alternatively, you can use this [Azure Active Directory PowerShell](/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) script to add the missing service principal.</span></span>

```PowerShell
Connect-AzureAD -TenantId <tenant-id>
# replace tenant-id by the id of your tenant.
New-AzureADServicePrincipal -AppId 0bf30f3b-4a52-48df-9a82-234910c4a086
```

## <a name="next-steps"></a><span data-ttu-id="ade04-207">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ade04-207">Next steps</span></span>

<span data-ttu-id="ade04-208">Confira os seguintes, inícios rápidos dos Hubs de Eventos do Azure:</span><span class="sxs-lookup"><span data-stu-id="ade04-208">See the following Azure Event Hubs quick starts:</span></span>

- [<span data-ttu-id="ade04-209">.NET Core</span><span class="sxs-lookup"><span data-stu-id="ade04-209">.NET Core</span></span>](/azure/event-hubs/get-started-dotnet-standard-send-v2)
- [<span data-ttu-id="ade04-210">Java</span><span class="sxs-lookup"><span data-stu-id="ade04-210">Java</span></span>](/azure/event-hubs/event-hubs-java-get-started-send)
- [<span data-ttu-id="ade04-211">Python</span><span class="sxs-lookup"><span data-stu-id="ade04-211">Python</span></span>](/azure/event-hubs/get-started-python-send-v2)
- [<span data-ttu-id="ade04-212">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ade04-212">JavaScript</span></span>](/azure/event-hubs/get-started-node-send-v2)
