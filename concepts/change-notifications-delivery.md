---
title: Receba notificações de alterações de maneiras diferentes
description: As notificações de alteração podem ser enviadas por meio de tecnologias diferentes, incluindo o webhooks e Hubs de Eventos do Azure.
author: Jumaodhiss
ms.localizationpriority: high
ms.custom: graphiamtop20, devx-track-azurecli
ms.openlocfilehash: 5a93ed69c7e0ed83dcb9ac9d877a59b9033d30b2
ms.sourcegitcommit: 0fa7148e0b776663eaca3e79e72b85046d4b8b1a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/15/2022
ms.locfileid: "63500900"
---
# <a name="get-change-notifications-delivered-in-different-ways"></a>Receber notificações de alterações de maneiras diferentes

As notificações de alteração podem ser entregues de diferentes maneiras aos assinantes. Se o principal modo de entrega para notificações de alteração for por meio de webhooks, pode ser desafiador tirar proveito de webhooks para cenários de alto rendimento ou quando o receptor não pode expor um URL de notificação disponível publicamente.  

Esse modo de entrega de notificações de alterações está disponível para todos os recursos que oferecem suporte a notificações de alterações do Microsoft Graph.

Bons exemplos de cenários de alta produtividade incluem aplicações que subscrevem um grande conjunto de recursos, aplicações que subscrevem recursos que mudam com uma alta frequência e aplicações multi-locatárias que subscrevem recursos através de um grande conjunto de organizações.

## <a name="using-azure-event-hubs-to-receive-change-notifications"></a>Usando os Hubs de Eventos do Azure para receber notificações de alteração

Os [Hubs de Eventos do Azure](https://azure.microsoft.com/services/event-hubs) é um serviço popular de inclusão e distribuição de eventos em tempo real, compilado para ser dimensionável. Você pode usar os Hubs de Eventos do Azure, em vez de webhooks tradicionais, para receber notificações de alteração.  
Usar os Hubs de Eventos do Azure para receber notificações de alteração difere do webhooks em algumas maneiras, incluindo:

- Você não depende de URLs com notificações publicamente expostas. O SDK do Hubs de Eventos retransmitirá as notificações para sua aplicação.
- Não é necessário responder à [validação da URL de notificação](webhooks.md#notification-endpoint-validation). Você pode ignorar a mensagem de validação recebida.
- Você precisará de provisionar um Hub de Eventos do Azure.
- Você precisará de provisionar um Azure Key Vault.

### <a name="set-up-the-azure-keyvault-and-azure-event-hubs"></a>Configurar o Cofre de Chaves do Azure e os Hubs de Eventos do Azure

Esta seção vai orientá-lo a configurar os necessários serviços do Azure.

#### <a name="option-1-using-the-azure-cli"></a>Opção 1: Usando o CLI do Azure

O [CLI do Azure](/cli/azure/what-is-azure-cli) permite que você escreva o script e automatize tarefas administrativas no Azure. O CLI pode ser [instalado em seu computador local](/cli/azure/install-azure-cli) ou ser executado diretamente a partir do [Azure Cloud Shell](/azure/cloud-shell/quickstart).

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

> **Observação:** O script fornecido aqui é compatível com shells baseados em Linux, Windows WSL e Azure Cloud Shell. Será necessário algumas atualizações para executar shells do Windows.

#### <a name="option-2-using-the-azure-portal"></a>Opção 2: Usando o Portal do Azure

##### <a name="configuring-the-azure-event-hub"></a>Configurando o Hub de eventos do Azure

Nesta seção, você vai:

- Criar um namespace do Hub de Eventos do Azure.
- Adicionar um hub para este namespace que irá transmitir e entregar notificações.
- Adicionar uma política de acesso compartilhado que permita obter uma cadeia de conexão para o hub recém-criado.

Etapas:

1. Abra um navegador para o [Portal do Azure](https://portal.azure.com).
1. Selecione **Criar um recurso**.
1. Digite **Hubs de Evento** na barra de pesquisa.
1. Selecione a sugestão **Hubs de Eventos**. A página de criação dos Hubs de Evento será carregada.  
1. Na página de criação dos Hubs de Evento clique **criar**.
1. Preencha os detalhes da criação no namespace dos Hubs de Eventos e clique em **Criar**.  
1. Quando o namespace do Hub de Eventos for provisionado, vá para a página do namespace.  
1. Clique em **Hubs de Eventos** e **+ Hub de Eventos**.  
1. Dê um nome para o novo Hub de Eventos e clique em **Criar**.  
1. Depois que o Hub de Eventos foi criado, clique no nome do Hub de Eventos e, em seguida, clique em **Políticas de acesso compartilhado** e **+ Adicionar** para adicionar uma nova política.  
1. Dê um nome à política, marque **Enviar**, e clique em **Criar**.  
1. Depois que a política for criada, clique no nome da política para abrir o painel de detalhes e, em seguida, copie o valor da **Chave primária da cadeia de conexão**. Anote-a; você precisará dela na próxima etapa.  

##### <a name="configuring-the-azure-key-vault"></a>Configurando o Azure Key Vault

Para acessar o Hub de Eventos de forma segura e permitir rotações de chaves, o Microsoft Graph obtém a cadeia de conexão para o Hub de Eventos através do Azure Key Vault.  
Nesta seção, você vai:

- Criar um Azure Key Vault para armazenar segredo.
- Adicionar a cadeia de conexão ao Hub de Evento como um segredo.
- Adicionar uma política de acesso para o Microsoft Graph acessar o segredo.

Etapas:

1. Abra um navegador para o [Portal do Azure](https://portal.azure.com).
1. Selecione **Criar um recurso**.
1. Digite **Cofre de Chaves** na barra de pesquisa.
1. Selecione a sugestão do **Cofre de Chaves**. A página de criação do Cofre de Chaves será carregada.
1. Na página de criação do Cofre de Chaves clique **criar**.  
1. Preencha os detalhes da criação do cofre de chaves e, em seguida, clique em **Revisar + Criar** e **Criar**.  
1. Acesse o cofre de chaves recém-criado usando o **recurso Vá para** da notificação.  
1. Copie o **nome do DNS**; você precisará dele para a próxima etapa.  
1. Vá para **Segredos** e clique em **+ Gerar/Importar**.  
1. Dê um nome ao segredo e guarde-o para mais tarde; você precisará dele para a próxima etapa. Para o valor, cole a cadeia de conexão que você gerou na etapa Hubs de Eventos. Clique em **Criar**.  
1. Clique em **Políticas de Acesso** e **+ Adicionar Política de Acesso**.  
1. Para **Permissões secretas**, selecione **Obter** e para **Selecionar Principal**, selecione **Controle de Alterações do Microsoft Graph**. Clique em **Adicionar**.  

### <a name="creating-the-subscription-and-receiving-notifications"></a>Criando a assinatura e recebendo notificações

Depois de você criar os serviços necessários Azure Key Vault e do Hubs de Eventos do Azure, você poderá criar sua assinatura e começar a receber as notificações de alteração por meio dos Hubs de Eventos do Azure.

#### <a name="creating-the-subcription"></a>Criando a assinatura

As assinaturas para alterar as notificações com os Hubs de Eventos são quase idênticas como alterar as notificações com webhooks. A principal diferença é que elas dependem dos Hubs de Eventos para entregar notificações. Todas as outras operações são similares, inclusive a [criação de assinatura](/graph/api/subscription-post-subscriptions).  

A principal diferença durante a criação da assinatura será o **notificationUrl**. Você deve defini-lo para `EventHub:https://<azurekeyvaultname>.vault.azure.net/secrets/<secretname>?tenantId=<domainname>` os seguintes valores:

- `azurekeyvaultname` - O nome que você atribuiu ao cofre de chaves quando o criou. Pode ser encontrado no nome DNS.
- `secretname` - O nome que você atribuiu ao segredo quando o criou. Pode ser encontrado na página **Segredos**. do Azure Key Vault.
- `domainname` – O nome do seu locatário do. por exemplo, consto.onmicrosoft.com ou contoso.com. Como esse domínio será usado para acessar o Azure Key Vault é importante que ele corresponda ao domínio usado pela assinatura do Azure que possui o Azure Key Vault. Para obter essa informação, você pode ir para a página de visão geral do Azure Key Vault que você criou e clique na assinatura. O nome de domínio é exibido sob o campo **Diretório**.

#### <a name="receiving-notifications"></a>Recebendo notificações

Os eventos agora serão enviados para o aplicativo através dos Hubs de Eventos. Para detalhes, confira [Recebendo eventos](/azure/event-hubs/get-started-dotnet-standard-send-v2#receive-events) na documentação Hubs de Eventos.

Antes de receber as notificações no aplicativo, você precisará criar outra política de acesso compartilhado com uma permissão de "Escuta" e obter a cadeia de conexão, semelhante às etapas listadas em [Configurando o Azure Event Hub](#configuring-the-azure-event-hub).

> **Observação:** Criar uma política separada para o aplicativo que escuta mensagens de Hubs de Eventos, em vez de reutilizar a mesma cadeia de conexão que você definiu no Azure keyVault. Isto garante que cada componente da solução tenha apenas as permissões que precisa e siga o princípio de segurança com o mínimo de permissões.

> **Observação:** Seu aplicativo recebe mensagens de validação sempre que criar uma nova assinatura. Você deve ignorar essas notificações. O exemplo a seguir representa o corpo de uma mensagem de validação.

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

### <a name="what-happens-if-the-microsoft-graph-change-tracking-application-is-missing"></a>O que acontece se o aplicativo Microsoft Graph Change Tracking estiver faltando?

É possível que o serviço principal do **Controle de Alterações do Microsoft Graph** esteja ausente no seu locatário, dependendo de quando o locatário foi criado e de operações administrativas. Para resolver este problema, execute [a seguinte consulta](https://developer.microsoft.com/en-us/graph/graph-explorer?request=servicePrincipals&method=POST&version=v1.0&GraphUrl=https://graph.microsoft.com&requestBody=eyJhcHBJZCI6IjBiZjMwZjNiLTRhNTItNDhkZi05YTgyLTIzNDkxMGM0YTA4NiJ9) no [Microsoft Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer).

Detalhes da consulta: `0bf30f3b-4a52-48df-9a82-234910c4a086` é o appId global para o aplicativo Microsoft Graph Change Tracking.

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals

{
    "appId": "0bf30f3b-4a52-48df-9a82-234910c4a086"
}
```

> **Observação:** Você pode obter um acesso negado ao executar esta consulta. Neste caso, selecione o ícone de engrenagem ao lado do nome da sua conta no canto superior esquerdo. Em seguida, selecione **Selecionar Permissões** e pesquise **Application.ReadWrite.All**. Marque a permissão e selecione **Consentir**. Após o consentimento dessa nova permissão, execute a solicitação novamente.

> **Observação:** Esta API só funciona com uma conta corporativa ou de estudante e não com uma conta pessoal. Certifique-se que você está conectado com uma conta no seu domínio.

Como alternativa, você pode utilizar o cmdlet [New-MgServicePrincipal](/powershell/module/microsoft.graph.applications/new-mgserviceprincipal?view=graph-powershell-1.0&preserve-view=true) no PowerShell do Microsoft Graph para adicionar a entidade de serviço ausente. Veja a seguir um exemplo de script.

```PowerShell
Connect-Graph -Scopes "Application.ReadWrite.All"
New-MgServicePrincipal -AppId "0bf30f3b-4a52-48df-9a82-234910c4a086"
```

## <a name="next-steps"></a>Próximas etapas

Confira os seguintes, inícios rápidos dos Hubs de Eventos do Azure:

- [.NET Core](/azure/event-hubs/get-started-dotnet-standard-send-v2)
- [Java](/azure/event-hubs/event-hubs-java-get-started-send)
- [Python](/azure/event-hubs/get-started-python-send-v2)
- [JavaScript](/azure/event-hubs/get-started-node-send-v2)
