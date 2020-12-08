---
title: tipo de recurso de assinatura
description: 'Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f675f8648b15f36517c1880f7bdb0c3178ef6b67
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597409"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="e77dd-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="e77dd-104">subscription resource type</span></span>

<span data-ttu-id="e77dd-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e77dd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e77dd-106">Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e77dd-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="e77dd-107">Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:</span><span class="sxs-lookup"><span data-stu-id="e77dd-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="e77dd-108">Um [alerta][] do Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="e77dd-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="e77dd-109">Uma [callRecord][] produzida após uma chamada ou uma reunião no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e77dd-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="e77dd-110">Um [chatMessage][] enviado por meio de equipes ou canais no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e77dd-110">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="e77dd-111">Uma [conversa][] em um grupo no Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e77dd-111">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="e77dd-112">Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="e77dd-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="e77dd-113">Uma [lista][] em um [site][] do SharePoint</span><span class="sxs-lookup"><span data-stu-id="e77dd-113">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="e77dd-114">Uma [mensagem][], [evento][] ou [contato][] no Outlook</span><span class="sxs-lookup"><span data-stu-id="e77dd-114">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="e77dd-115">A [presença][] de um usuário no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e77dd-115">The [presence][] of a user in Microsoft Teams</span></span>
- <span data-ttu-id="e77dd-116">Um [usuário][] ou [grupo][] no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e77dd-116">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="e77dd-117">Um [printTaskDefinition][] no serviço de impressão</span><span class="sxs-lookup"><span data-stu-id="e77dd-117">A [printTaskDefinition][] in Print Service</span></span>
- <span data-ttu-id="e77dd-118">Uma [todoTask] de um usuário da Microsoft para fazer</span><span class="sxs-lookup"><span data-stu-id="e77dd-118">A [todoTask] of a user in Microsoft To Do</span></span>

<span data-ttu-id="e77dd-119">Consulte [usar o Microsoft Graph API para obter notificações de alteração](webhooks.md) dos possíveis valores de caminho de recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="e77dd-119">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="e77dd-120">Métodos</span><span class="sxs-lookup"><span data-stu-id="e77dd-120">Methods</span></span>

| <span data-ttu-id="e77dd-121">Método</span><span class="sxs-lookup"><span data-stu-id="e77dd-121">Method</span></span> | <span data-ttu-id="e77dd-122">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e77dd-122">Return Type</span></span> | <span data-ttu-id="e77dd-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e77dd-123">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="e77dd-124">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="e77dd-124">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="e77dd-125">subscription</span><span class="sxs-lookup"><span data-stu-id="e77dd-125">subscription</span></span>](subscription.md) | <span data-ttu-id="e77dd-126">Assina um aplicativo de escuta para receber notificações sobre alterações nos dados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e77dd-126">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="e77dd-127">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="e77dd-127">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="e77dd-128">assinatura</span><span class="sxs-lookup"><span data-stu-id="e77dd-128">subscription</span></span>](subscription.md) | <span data-ttu-id="e77dd-129">Renovar uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="e77dd-129">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="e77dd-130">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="e77dd-130">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="e77dd-131">subscription</span><span class="sxs-lookup"><span data-stu-id="e77dd-131">subscription</span></span>](subscription.md) | <span data-ttu-id="e77dd-132">Lista assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="e77dd-132">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="e77dd-133">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="e77dd-133">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="e77dd-134">subscription</span><span class="sxs-lookup"><span data-stu-id="e77dd-134">subscription</span></span>](subscription.md) | <span data-ttu-id="e77dd-135">Leia as propriedades e as relações do objeto Subscription.</span><span class="sxs-lookup"><span data-stu-id="e77dd-135">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="e77dd-136">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="e77dd-136">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="e77dd-137">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e77dd-137">None</span></span> | <span data-ttu-id="e77dd-138">Excluir um objeto Subscription.</span><span class="sxs-lookup"><span data-stu-id="e77dd-138">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e77dd-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e77dd-139">Properties</span></span>

| <span data-ttu-id="e77dd-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e77dd-140">Property</span></span> | <span data-ttu-id="e77dd-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="e77dd-141">Type</span></span> | <span data-ttu-id="e77dd-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="e77dd-142">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="e77dd-143">changeType</span><span class="sxs-lookup"><span data-stu-id="e77dd-143">changeType</span></span> | <span data-ttu-id="e77dd-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e77dd-144">string</span></span> | <span data-ttu-id="e77dd-145">Indica qual é o tipo de alteração no recurso inscrito que irá emitir uma notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="e77dd-145">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="e77dd-146">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="e77dd-146">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="e77dd-147">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="e77dd-147">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="e77dd-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e77dd-148">Required.</span></span> <br><br><span data-ttu-id="e77dd-149">Observação: As notificações de alteração de lista e item raiz da unidade suportam apenas o `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="e77dd-149">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="e77dd-150">Suporte para notificações de alteração de usuário e grupo `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="e77dd-150">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="e77dd-151">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="e77dd-151">notificationUrl</span></span> | <span data-ttu-id="e77dd-152">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e77dd-152">string</span></span> | <span data-ttu-id="e77dd-153">A URL do ponto de extremidade que recebe as notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="e77dd-153">The URL of the endpoint that receives the change notifications.</span></span> <span data-ttu-id="e77dd-154">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="e77dd-154">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="e77dd-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e77dd-155">Required.</span></span> |
| <span data-ttu-id="e77dd-156">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="e77dd-156">lifecycleNotificationUrl</span></span> | <span data-ttu-id="e77dd-157">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e77dd-157">string</span></span> | <span data-ttu-id="e77dd-158">A URL do ponto de extremidade que recebe notificações de ciclo de vida, incluindo `subscriptionRemoved` e `missed` notificações.</span><span class="sxs-lookup"><span data-stu-id="e77dd-158">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="e77dd-159">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="e77dd-159">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="e77dd-160">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e77dd-160">Optional.</span></span> <br><br><span data-ttu-id="e77dd-161">[Leia mais](/graph/webhooks-lifecycle) sobre como os recursos do Outlook usam notificações de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="e77dd-161">[Read more](/graph/webhooks-lifecycle) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="e77dd-162">recurso</span><span class="sxs-lookup"><span data-stu-id="e77dd-162">resource</span></span> | <span data-ttu-id="e77dd-163">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e77dd-163">string</span></span> | <span data-ttu-id="e77dd-164">Especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="e77dd-164">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="e77dd-165">Não incluir a URL base (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="e77dd-165">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="e77dd-166">Consulte os possíveis valores do [caminho](webhooks.md) do recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="e77dd-166">See the possible resource path [values](webhooks.md) for each supported resource.</span></span> <span data-ttu-id="e77dd-167">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e77dd-167">Required.</span></span> |
| <span data-ttu-id="e77dd-168">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e77dd-168">expirationDateTime</span></span> | <span data-ttu-id="e77dd-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e77dd-169">DateTimeOffset</span></span> | <span data-ttu-id="e77dd-170">Especifica a data e a hora em que a assinatura do webhook expira.</span><span class="sxs-lookup"><span data-stu-id="e77dd-170">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="e77dd-171">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="e77dd-171">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="e77dd-172">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="e77dd-172">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="e77dd-173">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e77dd-173">Required.</span></span> |
| <span data-ttu-id="e77dd-174">clientState</span><span class="sxs-lookup"><span data-stu-id="e77dd-174">clientState</span></span> | <span data-ttu-id="e77dd-175">string</span><span class="sxs-lookup"><span data-stu-id="e77dd-175">string</span></span> | <span data-ttu-id="e77dd-176">Especifica o valor da propriedade **ClientState** enviada pelo serviço em cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="e77dd-176">Specifies the value of the **clientState** property sent by the service in each change notification.</span></span> <span data-ttu-id="e77dd-177">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="e77dd-177">The maximum length is 255 characters.</span></span> <span data-ttu-id="e77dd-178">O cliente pode verificar se a notificação de alteração veio do serviço, comparando o valor da propriedade **ClientState** enviada com a assinatura com o valor da propriedade **ClientState** recebida com cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="e77dd-178">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="e77dd-179">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e77dd-179">Optional.</span></span> |
| <span data-ttu-id="e77dd-180">id</span><span class="sxs-lookup"><span data-stu-id="e77dd-180">id</span></span> | <span data-ttu-id="e77dd-181">string</span><span class="sxs-lookup"><span data-stu-id="e77dd-181">string</span></span> | <span data-ttu-id="e77dd-p110">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e77dd-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="e77dd-184">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="e77dd-184">applicationId</span></span> | <span data-ttu-id="e77dd-185">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e77dd-185">string</span></span> | <span data-ttu-id="e77dd-186">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="e77dd-186">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="e77dd-187">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e77dd-187">Read-only.</span></span> |
| <span data-ttu-id="e77dd-188">creatorId</span><span class="sxs-lookup"><span data-stu-id="e77dd-188">creatorId</span></span> | <span data-ttu-id="e77dd-189">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e77dd-189">string</span></span> | <span data-ttu-id="e77dd-190">Identificador de usuário ou entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="e77dd-190">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="e77dd-191">Se o aplicativo usou permissões delegadas para criar a assinatura, este campo conterá a ID do usuário conectado o aplicativo chamado em nome de.</span><span class="sxs-lookup"><span data-stu-id="e77dd-191">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="e77dd-192">Se o aplicativo usava permissões de aplicativo, este campo contém a ID da entidade de serviço correspondente ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e77dd-192">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="e77dd-193">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e77dd-193">Read-only.</span></span> |
| <span data-ttu-id="e77dd-194">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="e77dd-194">includeResourceData</span></span> | <span data-ttu-id="e77dd-195">Booleano</span><span class="sxs-lookup"><span data-stu-id="e77dd-195">Boolean</span></span> | <span data-ttu-id="e77dd-196">Quando definido como `true`, alterar as notificações [inclui dados de recurso](/graph/webhooks-with-resource-data) (como o conteúdo de uma mensagem de bate-papo).</span><span class="sxs-lookup"><span data-stu-id="e77dd-196">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="e77dd-197">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e77dd-197">Optional.</span></span> | 
| <span data-ttu-id="e77dd-198">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="e77dd-198">encryptionCertificate</span></span> | <span data-ttu-id="e77dd-199">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e77dd-199">string</span></span> | <span data-ttu-id="e77dd-200">Uma representação codificada em Base64 de um certificado com uma chave pública usada para criptografar os dados de recursos nas notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="e77dd-200">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="e77dd-201">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e77dd-201">Optional.</span></span> <span data-ttu-id="e77dd-202">Obrigatório quando **includeResourceData** é verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="e77dd-202">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="e77dd-203">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="e77dd-203">encryptionCertificateId</span></span> | <span data-ttu-id="e77dd-204">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e77dd-204">string</span></span> | <span data-ttu-id="e77dd-205">Um identificador personalizado fornecido pelo aplicativo para ajudar a identificar o certificado necessário para descriptografar os dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="e77dd-205">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="e77dd-206">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e77dd-206">Optional.</span></span> <span data-ttu-id="e77dd-207">Obrigatório quando **includeResourceData** é verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="e77dd-207">Required when **includeResourceData** is true.</span></span> |
| <span data-ttu-id="e77dd-208">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="e77dd-208">latestSupportedTlsVersion</span></span> | <span data-ttu-id="e77dd-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e77dd-209">String</span></span> | <span data-ttu-id="e77dd-210">Especifica a versão mais recente do protocolo TLS que o ponto de extremidade, especificado por **notificationUrl**, é compatível.</span><span class="sxs-lookup"><span data-stu-id="e77dd-210">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="e77dd-211">Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="e77dd-211">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="e77dd-212">Para os assinantes cujo ponto de extremidade de notificação suporta uma versão menor que a versão recomendada atualmente (TLS 1.2), especificar essa propriedade por uma [linha do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) definida, permite o uso temporário da versão preterida do TLS antes de concluir a atualização para o TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="e77dd-212">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="e77dd-213">Para esses assinantes, não definir essa propriedade pela linha do tempo resultaria em uma falha nas operações da assinatura.</span><span class="sxs-lookup"><span data-stu-id="e77dd-213">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="e77dd-214">Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="e77dd-214">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="e77dd-215">Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="e77dd-215">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="e77dd-216">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="e77dd-216">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="e77dd-217">Resource</span><span class="sxs-lookup"><span data-stu-id="e77dd-217">Resource</span></span>            | <span data-ttu-id="e77dd-218">Tempo de expiração máximo</span><span class="sxs-lookup"><span data-stu-id="e77dd-218">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="e77dd-219">**Alerta** de segurança</span><span class="sxs-lookup"><span data-stu-id="e77dd-219">Security **alert**</span></span>     | <span data-ttu-id="e77dd-220">43200 minutos (em 30 dias )</span><span class="sxs-lookup"><span data-stu-id="e77dd-220">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="e77dd-221">Teams **callRecord**</span><span class="sxs-lookup"><span data-stu-id="e77dd-221">Teams **callRecord**</span></span>    | <span data-ttu-id="e77dd-222">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e77dd-222">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="e77dd-223">Teams **chatMessage**</span><span class="sxs-lookup"><span data-stu-id="e77dd-223">Teams **chatMessage**</span></span>    | <span data-ttu-id="e77dd-224">60 minutos (1 hora)</span><span class="sxs-lookup"><span data-stu-id="e77dd-224">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="e77dd-225">**Conversa** em grupo</span><span class="sxs-lookup"><span data-stu-id="e77dd-225">Group **conversation**</span></span> | <span data-ttu-id="e77dd-226">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e77dd-226">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="e77dd-227">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="e77dd-227">OneDrive **driveItem**</span></span>    | <span data-ttu-id="e77dd-228">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e77dd-228">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="e77dd-229">**Lista** do Microsoft Office SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="e77dd-229">SharePoint **list**</span></span>    | <span data-ttu-id="e77dd-230">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e77dd-230">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="e77dd-231">Outlook **mensagem**, **evento**, **contato**</span><span class="sxs-lookup"><span data-stu-id="e77dd-231">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="e77dd-232">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e77dd-232">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="e77dd-233">**usuário**, **grupo**, outros recursos de diretório</span><span class="sxs-lookup"><span data-stu-id="e77dd-233">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="e77dd-234">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e77dd-234">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="e77dd-235">**presence**</span><span class="sxs-lookup"><span data-stu-id="e77dd-235">**presence**</span></span>        | <span data-ttu-id="e77dd-236">60 minutos (1 hora)</span><span class="sxs-lookup"><span data-stu-id="e77dd-236">60 minutes (1 hour)</span></span> |
| <span data-ttu-id="e77dd-237">Imprimir **printTaskDefinition**</span><span class="sxs-lookup"><span data-stu-id="e77dd-237">Print **printTaskDefinition**</span></span> | <span data-ttu-id="e77dd-238">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e77dd-238">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="e77dd-239">**todoTask**</span><span class="sxs-lookup"><span data-stu-id="e77dd-239">**todoTask**</span></span>              | <span data-ttu-id="e77dd-240">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e77dd-240">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="e77dd-241">**Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado.</span><span class="sxs-lookup"><span data-stu-id="e77dd-241">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="e77dd-242">No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.</span><span class="sxs-lookup"><span data-stu-id="e77dd-242">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="e77dd-243">Relações</span><span class="sxs-lookup"><span data-stu-id="e77dd-243">Relationships</span></span>

<span data-ttu-id="e77dd-244">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e77dd-244">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e77dd-245">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e77dd-245">JSON representation</span></span>

<span data-ttu-id="e77dd-246">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e77dd-246">Here is a JSON representation of the resource.</span></span>

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
[printTaskDefinition]: ./printtaskdefinition.md
[todoTask]: ./todotask.md

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


