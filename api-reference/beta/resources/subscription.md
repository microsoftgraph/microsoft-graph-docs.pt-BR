---
title: tipo de recurso de assinatura
description: 'Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 82690551bc11aad59506613bfc833270db414b4b
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742108"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="9f76f-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="9f76f-104">subscription resource type</span></span>

<span data-ttu-id="9f76f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f76f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f76f-106">Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9f76f-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="9f76f-107">Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:</span><span class="sxs-lookup"><span data-stu-id="9f76f-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="9f76f-108">Um [alerta][] do Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="9f76f-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="9f76f-109">Uma [callRecord][] produzida após uma chamada ou uma reunião no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9f76f-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="9f76f-110">Um [chatMessage][] enviado por meio de equipes ou canais no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9f76f-110">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="9f76f-111">Uma [conversa][] em um grupo no Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9f76f-111">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="9f76f-112">Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="9f76f-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="9f76f-113">Uma [lista][] em um [site][] do SharePoint</span><span class="sxs-lookup"><span data-stu-id="9f76f-113">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="9f76f-114">Uma [mensagem][], [evento][] ou [contato][] no Outlook</span><span class="sxs-lookup"><span data-stu-id="9f76f-114">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="9f76f-115">A [presença][] de um usuário no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9f76f-115">The [presence][] of a user in Microsoft Teams</span></span>
- <span data-ttu-id="9f76f-116">Um [usuário][] ou [grupo][] no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="9f76f-116">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="9f76f-117">Consulte [usar o Microsoft Graph API para obter notificações de alteração](webhooks.md) dos possíveis valores de caminho de recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="9f76f-117">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="9f76f-118">Métodos</span><span class="sxs-lookup"><span data-stu-id="9f76f-118">Methods</span></span>

| <span data-ttu-id="9f76f-119">Método</span><span class="sxs-lookup"><span data-stu-id="9f76f-119">Method</span></span> | <span data-ttu-id="9f76f-120">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9f76f-120">Return Type</span></span> | <span data-ttu-id="9f76f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f76f-121">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="9f76f-122">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="9f76f-122">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="9f76f-123">assinatura</span><span class="sxs-lookup"><span data-stu-id="9f76f-123">subscription</span></span>](subscription.md) | <span data-ttu-id="9f76f-124">Assina um aplicativo de escuta para receber notificações sobre alterações nos dados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9f76f-124">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="9f76f-125">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="9f76f-125">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="9f76f-126">subscription</span><span class="sxs-lookup"><span data-stu-id="9f76f-126">subscription</span></span>](subscription.md) | <span data-ttu-id="9f76f-127">Renovar uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="9f76f-127">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="9f76f-128">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="9f76f-128">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="9f76f-129">assinatura</span><span class="sxs-lookup"><span data-stu-id="9f76f-129">subscription</span></span>](subscription.md) | <span data-ttu-id="9f76f-130">Lista assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="9f76f-130">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="9f76f-131">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="9f76f-131">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="9f76f-132">subscription</span><span class="sxs-lookup"><span data-stu-id="9f76f-132">subscription</span></span>](subscription.md) | <span data-ttu-id="9f76f-133">Leia as propriedades e as relações do objeto Subscription.</span><span class="sxs-lookup"><span data-stu-id="9f76f-133">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="9f76f-134">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="9f76f-134">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="9f76f-135">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9f76f-135">None</span></span> | <span data-ttu-id="9f76f-136">Excluir um objeto Subscription.</span><span class="sxs-lookup"><span data-stu-id="9f76f-136">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9f76f-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f76f-137">Properties</span></span>

| <span data-ttu-id="9f76f-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f76f-138">Property</span></span> | <span data-ttu-id="9f76f-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f76f-139">Type</span></span> | <span data-ttu-id="9f76f-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f76f-140">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="9f76f-141">changeType</span><span class="sxs-lookup"><span data-stu-id="9f76f-141">changeType</span></span> | <span data-ttu-id="9f76f-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f76f-142">string</span></span> | <span data-ttu-id="9f76f-143">Indica qual é o tipo de alteração no recurso inscrito que irá emitir uma notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="9f76f-143">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="9f76f-144">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="9f76f-144">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="9f76f-145">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="9f76f-145">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="9f76f-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f76f-146">Required.</span></span> <br><br><span data-ttu-id="9f76f-147">Observação: As notificações de alteração de lista e item raiz da unidade suportam apenas o `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="9f76f-147">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="9f76f-148">Suporte para notificações de alteração de usuário e grupo `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="9f76f-148">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="9f76f-149">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="9f76f-149">notificationUrl</span></span> | <span data-ttu-id="9f76f-150">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f76f-150">string</span></span> | <span data-ttu-id="9f76f-151">A URL do ponto de extremidade que recebe as notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="9f76f-151">The URL of the endpoint that receives the change notifications.</span></span> <span data-ttu-id="9f76f-152">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="9f76f-152">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="9f76f-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f76f-153">Required.</span></span> |
| <span data-ttu-id="9f76f-154">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="9f76f-154">lifecycleNotificationUrl</span></span> | <span data-ttu-id="9f76f-155">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f76f-155">string</span></span> | <span data-ttu-id="9f76f-156">A URL do ponto de extremidade que recebe notificações de ciclo de vida, incluindo `subscriptionRemoved` e `missed` notificações.</span><span class="sxs-lookup"><span data-stu-id="9f76f-156">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="9f76f-157">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="9f76f-157">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="9f76f-158">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9f76f-158">Optional.</span></span> <br><br><span data-ttu-id="9f76f-159">[Leia mais](/graph/webhooks-lifecycle) sobre como os recursos do Outlook usam notificações de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="9f76f-159">[Read more](/graph/webhooks-lifecycle) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="9f76f-160">recurso</span><span class="sxs-lookup"><span data-stu-id="9f76f-160">resource</span></span> | <span data-ttu-id="9f76f-161">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f76f-161">string</span></span> | <span data-ttu-id="9f76f-162">Especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="9f76f-162">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="9f76f-163">Não incluir a URL base (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="9f76f-163">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="9f76f-164">Consulte os possíveis valores do [caminho](webhooks.md) do recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="9f76f-164">See the possible resource path [values](webhooks.md) for each supported resource.</span></span> <span data-ttu-id="9f76f-165">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f76f-165">Required.</span></span> |
| <span data-ttu-id="9f76f-166">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9f76f-166">expirationDateTime</span></span> | <span data-ttu-id="9f76f-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f76f-167">DateTimeOffset</span></span> | <span data-ttu-id="9f76f-168">Especifica a data e a hora em que a assinatura do webhook expira.</span><span class="sxs-lookup"><span data-stu-id="9f76f-168">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="9f76f-169">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="9f76f-169">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="9f76f-170">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="9f76f-170">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="9f76f-171">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f76f-171">Required.</span></span> |
| <span data-ttu-id="9f76f-172">clientState</span><span class="sxs-lookup"><span data-stu-id="9f76f-172">clientState</span></span> | <span data-ttu-id="9f76f-173">string</span><span class="sxs-lookup"><span data-stu-id="9f76f-173">string</span></span> | <span data-ttu-id="9f76f-174">Especifica o valor da propriedade **ClientState** enviada pelo serviço em cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="9f76f-174">Specifies the value of the **clientState** property sent by the service in each change notification.</span></span> <span data-ttu-id="9f76f-175">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="9f76f-175">The maximum length is 255 characters.</span></span> <span data-ttu-id="9f76f-176">O cliente pode verificar se a notificação de alteração veio do serviço, comparando o valor da propriedade **ClientState** enviada com a assinatura com o valor da propriedade **ClientState** recebida com cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="9f76f-176">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="9f76f-177">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9f76f-177">Optional.</span></span> |
| <span data-ttu-id="9f76f-178">id</span><span class="sxs-lookup"><span data-stu-id="9f76f-178">id</span></span> | <span data-ttu-id="9f76f-179">string</span><span class="sxs-lookup"><span data-stu-id="9f76f-179">string</span></span> | <span data-ttu-id="9f76f-p110">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f76f-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="9f76f-182">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="9f76f-182">applicationId</span></span> | <span data-ttu-id="9f76f-183">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f76f-183">string</span></span> | <span data-ttu-id="9f76f-184">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="9f76f-184">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="9f76f-185">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f76f-185">Read-only.</span></span> |
| <span data-ttu-id="9f76f-186">creatorId</span><span class="sxs-lookup"><span data-stu-id="9f76f-186">creatorId</span></span> | <span data-ttu-id="9f76f-187">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f76f-187">string</span></span> | <span data-ttu-id="9f76f-188">Identificador de usuário ou entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="9f76f-188">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="9f76f-189">Se o aplicativo usou permissões delegadas para criar a assinatura, este campo conterá a ID do usuário conectado o aplicativo chamado em nome de.</span><span class="sxs-lookup"><span data-stu-id="9f76f-189">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="9f76f-190">Se o aplicativo usava permissões de aplicativo, este campo contém a ID da entidade de serviço correspondente ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f76f-190">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="9f76f-191">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f76f-191">Read-only.</span></span> |
| <span data-ttu-id="9f76f-192">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="9f76f-192">includeResourceData</span></span> | <span data-ttu-id="9f76f-193">Booleano</span><span class="sxs-lookup"><span data-stu-id="9f76f-193">Boolean</span></span> | <span data-ttu-id="9f76f-194">Quando definido como `true`, alterar as notificações [inclui dados de recurso](/graph/webhooks-with-resource-data) (como o conteúdo de uma mensagem de bate-papo).</span><span class="sxs-lookup"><span data-stu-id="9f76f-194">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="9f76f-195">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9f76f-195">Optional.</span></span> | 
| <span data-ttu-id="9f76f-196">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="9f76f-196">encryptionCertificate</span></span> | <span data-ttu-id="9f76f-197">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f76f-197">string</span></span> | <span data-ttu-id="9f76f-198">Uma representação codificada em Base64 de um certificado com uma chave pública usada para criptografar os dados de recursos nas notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="9f76f-198">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="9f76f-199">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9f76f-199">Optional.</span></span> <span data-ttu-id="9f76f-200">Obrigatório quando **includeResourceData** é verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="9f76f-200">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="9f76f-201">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="9f76f-201">encryptionCertificateId</span></span> | <span data-ttu-id="9f76f-202">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f76f-202">string</span></span> | <span data-ttu-id="9f76f-203">Um identificador personalizado fornecido pelo aplicativo para ajudar a identificar o certificado necessário para descriptografar os dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f76f-203">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="9f76f-204">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9f76f-204">Optional.</span></span> <span data-ttu-id="9f76f-205">Obrigatório quando **includeResourceData** é verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="9f76f-205">Required when **includeResourceData** is true.</span></span> |
| <span data-ttu-id="9f76f-206">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="9f76f-206">latestSupportedTlsVersion</span></span> | <span data-ttu-id="9f76f-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f76f-207">String</span></span> | <span data-ttu-id="9f76f-208">Especifica a versão mais recente do protocolo TLS que o ponto de extremidade, especificado por **notificationUrl**, é compatível.</span><span class="sxs-lookup"><span data-stu-id="9f76f-208">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="9f76f-209">Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="9f76f-209">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="9f76f-210">Para os assinantes cujo ponto de extremidade de notificação suporta uma versão menor que a versão recomendada atualmente (TLS 1.2), especificar essa propriedade por uma [linha do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) definida, permite o uso temporário da versão preterida do TLS antes de concluir a atualização para o TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="9f76f-210">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="9f76f-211">Para esses assinantes, não definir essa propriedade pela linha do tempo resultaria em uma falha nas operações da assinatura.</span><span class="sxs-lookup"><span data-stu-id="9f76f-211">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="9f76f-212">Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="9f76f-212">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="9f76f-213">Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="9f76f-213">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="9f76f-214">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="9f76f-214">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="9f76f-215">Resource</span><span class="sxs-lookup"><span data-stu-id="9f76f-215">Resource</span></span>            | <span data-ttu-id="9f76f-216">Tempo de expiração máximo</span><span class="sxs-lookup"><span data-stu-id="9f76f-216">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="9f76f-217">**Alerta** de segurança</span><span class="sxs-lookup"><span data-stu-id="9f76f-217">Security **alert**</span></span>     | <span data-ttu-id="9f76f-218">43200 minutos (em 30 dias )</span><span class="sxs-lookup"><span data-stu-id="9f76f-218">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="9f76f-219">Teams **callRecord**</span><span class="sxs-lookup"><span data-stu-id="9f76f-219">Teams **callRecord**</span></span>    | <span data-ttu-id="9f76f-220">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="9f76f-220">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="9f76f-221">Teams **chatMessage**</span><span class="sxs-lookup"><span data-stu-id="9f76f-221">Teams **chatMessage**</span></span>    | <span data-ttu-id="9f76f-222">60 minutos (1 hora)</span><span class="sxs-lookup"><span data-stu-id="9f76f-222">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="9f76f-223">**Conversa** em grupo</span><span class="sxs-lookup"><span data-stu-id="9f76f-223">Group **conversation**</span></span> | <span data-ttu-id="9f76f-224">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="9f76f-224">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="9f76f-225">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="9f76f-225">OneDrive **driveItem**</span></span>    | <span data-ttu-id="9f76f-226">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="9f76f-226">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="9f76f-227">**Lista** do Microsoft Office SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9f76f-227">SharePoint **list**</span></span>    | <span data-ttu-id="9f76f-228">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="9f76f-228">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="9f76f-229">Outlook **mensagem**, **evento**, **contato**</span><span class="sxs-lookup"><span data-stu-id="9f76f-229">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="9f76f-230">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="9f76f-230">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="9f76f-231">**usuário**, **grupo**, outros recursos de diretório</span><span class="sxs-lookup"><span data-stu-id="9f76f-231">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="9f76f-232">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="9f76f-232">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="9f76f-233">**presence**</span><span class="sxs-lookup"><span data-stu-id="9f76f-233">**presence**</span></span>        | <span data-ttu-id="9f76f-234">60 minutos (1 hora)</span><span class="sxs-lookup"><span data-stu-id="9f76f-234">60 minutes (1 hour)</span></span> |


> <span data-ttu-id="9f76f-235">**Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado.</span><span class="sxs-lookup"><span data-stu-id="9f76f-235">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="9f76f-236">No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.</span><span class="sxs-lookup"><span data-stu-id="9f76f-236">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="9f76f-237">Relações</span><span class="sxs-lookup"><span data-stu-id="9f76f-237">Relationships</span></span>

<span data-ttu-id="9f76f-238">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f76f-238">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f76f-239">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f76f-239">JSON representation</span></span>

<span data-ttu-id="9f76f-240">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f76f-240">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscription",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false,
        "sortable": false
      }
    }
  ]
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "lifecycleNotificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string",
  "includeResourceData": "boolean",
  "encryptionCertificate": "string",
  "encryptionCertificateId": "string",
  "latestSupportedTlsVersion": "string"
}
```

[contato]: ./contact.md
[contact]: ./contact.md
[conversa]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[list]: ./list.md
[site]: ./site.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
[chatMessage]: ./chatmessage.md
[callRecord]: ./callrecords-callrecord.md
[presence]: ./presence.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


