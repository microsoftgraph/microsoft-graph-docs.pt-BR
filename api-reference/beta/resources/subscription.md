---
title: tipo de recurso de assinatura
description: 'Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b3efc8736b5dffe745f43ad096837cb05827e734
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932490"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="f6211-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="f6211-104">subscription resource type</span></span>

<span data-ttu-id="f6211-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6211-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6211-106">Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f6211-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="f6211-107">Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:</span><span class="sxs-lookup"><span data-stu-id="f6211-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="f6211-108">Um [alerta][] do Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="f6211-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="f6211-109">Uma [callRecord][] produzida após uma chamada ou uma reunião no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="f6211-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="f6211-110">Um [chatMessage][] enviado por meio de equipes ou canais no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="f6211-110">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="f6211-111">Uma [conversa][] em um grupo no Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f6211-111">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="f6211-112">Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="f6211-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="f6211-113">Uma [lista][] em um [site][] do SharePoint</span><span class="sxs-lookup"><span data-stu-id="f6211-113">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="f6211-114">Uma [mensagem][], [evento][] ou [contato][] no Outlook</span><span class="sxs-lookup"><span data-stu-id="f6211-114">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="f6211-115">A [presença][] de um usuário no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="f6211-115">The [presence][] of a user in Microsoft Teams</span></span>
- <span data-ttu-id="f6211-116">Um [usuário][] ou [grupo][] no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f6211-116">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="f6211-117">Um [printTaskDefinition][] no serviço de impressão</span><span class="sxs-lookup"><span data-stu-id="f6211-117">A [printTaskDefinition][] in Print Service</span></span>

<span data-ttu-id="f6211-118">Consulte [usar o Microsoft Graph API para obter notificações de alteração](webhooks.md) dos possíveis valores de caminho de recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="f6211-118">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="f6211-119">Métodos</span><span class="sxs-lookup"><span data-stu-id="f6211-119">Methods</span></span>

| <span data-ttu-id="f6211-120">Método</span><span class="sxs-lookup"><span data-stu-id="f6211-120">Method</span></span> | <span data-ttu-id="f6211-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f6211-121">Return Type</span></span> | <span data-ttu-id="f6211-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6211-122">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="f6211-123">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="f6211-123">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="f6211-124">assinatura</span><span class="sxs-lookup"><span data-stu-id="f6211-124">subscription</span></span>](subscription.md) | <span data-ttu-id="f6211-125">Assina um aplicativo de escuta para receber notificações sobre alterações nos dados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f6211-125">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="f6211-126">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="f6211-126">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="f6211-127">subscription</span><span class="sxs-lookup"><span data-stu-id="f6211-127">subscription</span></span>](subscription.md) | <span data-ttu-id="f6211-128">Renovar uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="f6211-128">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="f6211-129">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="f6211-129">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="f6211-130">assinatura</span><span class="sxs-lookup"><span data-stu-id="f6211-130">subscription</span></span>](subscription.md) | <span data-ttu-id="f6211-131">Lista assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="f6211-131">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="f6211-132">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="f6211-132">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="f6211-133">subscription</span><span class="sxs-lookup"><span data-stu-id="f6211-133">subscription</span></span>](subscription.md) | <span data-ttu-id="f6211-134">Leia as propriedades e as relações do objeto Subscription.</span><span class="sxs-lookup"><span data-stu-id="f6211-134">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="f6211-135">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="f6211-135">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="f6211-136">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f6211-136">None</span></span> | <span data-ttu-id="f6211-137">Excluir um objeto Subscription.</span><span class="sxs-lookup"><span data-stu-id="f6211-137">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f6211-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6211-138">Properties</span></span>

| <span data-ttu-id="f6211-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6211-139">Property</span></span> | <span data-ttu-id="f6211-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6211-140">Type</span></span> | <span data-ttu-id="f6211-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6211-141">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f6211-142">changeType</span><span class="sxs-lookup"><span data-stu-id="f6211-142">changeType</span></span> | <span data-ttu-id="f6211-143">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6211-143">string</span></span> | <span data-ttu-id="f6211-144">Indica qual é o tipo de alteração no recurso inscrito que irá emitir uma notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="f6211-144">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="f6211-145">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="f6211-145">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="f6211-146">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="f6211-146">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="f6211-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6211-147">Required.</span></span> <br><br><span data-ttu-id="f6211-148">Observação: As notificações de alteração de lista e item raiz da unidade suportam apenas o `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="f6211-148">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="f6211-149">Suporte para notificações de alteração de usuário e grupo `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="f6211-149">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="f6211-150">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="f6211-150">notificationUrl</span></span> | <span data-ttu-id="f6211-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6211-151">string</span></span> | <span data-ttu-id="f6211-152">A URL do ponto de extremidade que recebe as notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="f6211-152">The URL of the endpoint that receives the change notifications.</span></span> <span data-ttu-id="f6211-153">Esta URL deve fazer uso do protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="f6211-153">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="f6211-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6211-154">Required.</span></span> |
| <span data-ttu-id="f6211-155">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="f6211-155">lifecycleNotificationUrl</span></span> | <span data-ttu-id="f6211-156">string</span><span class="sxs-lookup"><span data-stu-id="f6211-156">string</span></span> | <span data-ttu-id="f6211-157">A URL do ponto de extremidade que recebe notificações do ciclo de vida, incluindo notificações de `subscriptionRemoved` e `missed`.</span><span class="sxs-lookup"><span data-stu-id="f6211-157">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="f6211-158">Esta URL deve fazer uso do protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="f6211-158">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="f6211-159">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f6211-159">Optional.</span></span> <br><br><span data-ttu-id="f6211-160">[Leia mais](/graph/webhooks-lifecycle) sobre como os recursos do Outlook usam notificações do ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="f6211-160">[Read more](/graph/webhooks-lifecycle) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="f6211-161">recurso</span><span class="sxs-lookup"><span data-stu-id="f6211-161">resource</span></span> | <span data-ttu-id="f6211-162">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6211-162">string</span></span> | <span data-ttu-id="f6211-163">Especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="f6211-163">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="f6211-164">Não incluir a URL base (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="f6211-164">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="f6211-165">Consulte os possíveis valores do [caminho](webhooks.md) do recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="f6211-165">See the possible resource path [values](webhooks.md) for each supported resource.</span></span> <span data-ttu-id="f6211-166">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6211-166">Required.</span></span> |
| <span data-ttu-id="f6211-167">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f6211-167">expirationDateTime</span></span> | <span data-ttu-id="f6211-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6211-168">DateTimeOffset</span></span> | <span data-ttu-id="f6211-169">Especifica a data e a hora em que a assinatura do webhook expira.</span><span class="sxs-lookup"><span data-stu-id="f6211-169">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="f6211-170">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="f6211-170">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="f6211-171">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="f6211-171">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="f6211-172">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6211-172">Required.</span></span> |
| <span data-ttu-id="f6211-173">clientState</span><span class="sxs-lookup"><span data-stu-id="f6211-173">clientState</span></span> | <span data-ttu-id="f6211-174">string</span><span class="sxs-lookup"><span data-stu-id="f6211-174">string</span></span> | <span data-ttu-id="f6211-175">Especifica o valor da propriedade **ClientState** enviada pelo serviço em cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="f6211-175">Specifies the value of the **clientState** property sent by the service in each change notification.</span></span> <span data-ttu-id="f6211-176">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="f6211-176">The maximum length is 255 characters.</span></span> <span data-ttu-id="f6211-177">O cliente pode verificar se a notificação de alteração veio do serviço, comparando o valor da propriedade **ClientState** enviada com a assinatura com o valor da propriedade **ClientState** recebida com cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="f6211-177">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="f6211-178">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f6211-178">Optional.</span></span> |
| <span data-ttu-id="f6211-179">id</span><span class="sxs-lookup"><span data-stu-id="f6211-179">id</span></span> | <span data-ttu-id="f6211-180">string</span><span class="sxs-lookup"><span data-stu-id="f6211-180">string</span></span> | <span data-ttu-id="f6211-p110">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f6211-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="f6211-183">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="f6211-183">applicationId</span></span> | <span data-ttu-id="f6211-184">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6211-184">string</span></span> | <span data-ttu-id="f6211-185">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="f6211-185">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="f6211-186">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f6211-186">Read-only.</span></span> |
| <span data-ttu-id="f6211-187">creatorId</span><span class="sxs-lookup"><span data-stu-id="f6211-187">creatorId</span></span> | <span data-ttu-id="f6211-188">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6211-188">string</span></span> | <span data-ttu-id="f6211-189">Identificador de usuário ou entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="f6211-189">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="f6211-190">Se o aplicativo usou permissões delegadas para criar a assinatura, este campo conterá a ID do usuário conectado o aplicativo chamado em nome de.</span><span class="sxs-lookup"><span data-stu-id="f6211-190">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="f6211-191">Se o aplicativo usava permissões de aplicativo, este campo contém a ID da entidade de serviço correspondente ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f6211-191">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="f6211-192">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f6211-192">Read-only.</span></span> |
| <span data-ttu-id="f6211-193">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="f6211-193">includeResourceData</span></span> | <span data-ttu-id="f6211-194">Booleano</span><span class="sxs-lookup"><span data-stu-id="f6211-194">Boolean</span></span> | <span data-ttu-id="f6211-195">Quando definido como `true`, alterar as notificações [inclui dados de recurso](/graph/webhooks-with-resource-data) (como o conteúdo de uma mensagem de bate-papo).</span><span class="sxs-lookup"><span data-stu-id="f6211-195">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="f6211-196">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f6211-196">Optional.</span></span> | 
| <span data-ttu-id="f6211-197">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="f6211-197">encryptionCertificate</span></span> | <span data-ttu-id="f6211-198">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6211-198">string</span></span> | <span data-ttu-id="f6211-199">Uma representação codificada em Base64 de um certificado com uma chave pública usada para criptografar os dados de recursos nas notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="f6211-199">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="f6211-200">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f6211-200">Optional.</span></span> <span data-ttu-id="f6211-201">Obrigatório quando **includeResourceData** é verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="f6211-201">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="f6211-202">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="f6211-202">encryptionCertificateId</span></span> | <span data-ttu-id="f6211-203">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6211-203">string</span></span> | <span data-ttu-id="f6211-204">Um identificador personalizado fornecido pelo aplicativo para ajudar a identificar o certificado necessário para descriptografar os dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6211-204">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="f6211-205">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f6211-205">Optional.</span></span> <span data-ttu-id="f6211-206">Obrigatório quando **includeResourceData** é verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="f6211-206">Required when **includeResourceData** is true.</span></span> |
| <span data-ttu-id="f6211-207">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="f6211-207">latestSupportedTlsVersion</span></span> | <span data-ttu-id="f6211-208">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6211-208">String</span></span> | <span data-ttu-id="f6211-209">Especifica a versão mais recente do protocolo TLS que o ponto de extremidade, especificado por **notificationUrl** , é compatível.</span><span class="sxs-lookup"><span data-stu-id="f6211-209">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl** , supports.</span></span> <span data-ttu-id="f6211-210">Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="f6211-210">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="f6211-211">Para os assinantes cujo ponto de extremidade de notificação suporta uma versão menor que a versão recomendada atualmente (TLS 1.2), especificar essa propriedade por uma [linha do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) definida, permite o uso temporário da versão preterida do TLS antes de concluir a atualização para o TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="f6211-211">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="f6211-212">Para esses assinantes, não definir essa propriedade pela linha do tempo resultaria em uma falha nas operações da assinatura.</span><span class="sxs-lookup"><span data-stu-id="f6211-212">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="f6211-213">Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="f6211-213">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="f6211-214">Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="f6211-214">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="f6211-215">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="f6211-215">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="f6211-216">Resource</span><span class="sxs-lookup"><span data-stu-id="f6211-216">Resource</span></span>            | <span data-ttu-id="f6211-217">Tempo de expiração máximo</span><span class="sxs-lookup"><span data-stu-id="f6211-217">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="f6211-218">**Alerta** de segurança</span><span class="sxs-lookup"><span data-stu-id="f6211-218">Security **alert**</span></span>     | <span data-ttu-id="f6211-219">43200 minutos (em 30 dias )</span><span class="sxs-lookup"><span data-stu-id="f6211-219">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="f6211-220">Teams **callRecord**</span><span class="sxs-lookup"><span data-stu-id="f6211-220">Teams **callRecord**</span></span>    | <span data-ttu-id="f6211-221">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="f6211-221">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="f6211-222">Teams **chatMessage**</span><span class="sxs-lookup"><span data-stu-id="f6211-222">Teams **chatMessage**</span></span>    | <span data-ttu-id="f6211-223">60 minutos (1 hora)</span><span class="sxs-lookup"><span data-stu-id="f6211-223">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="f6211-224">**Conversa** em grupo</span><span class="sxs-lookup"><span data-stu-id="f6211-224">Group **conversation**</span></span> | <span data-ttu-id="f6211-225">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="f6211-225">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f6211-226">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="f6211-226">OneDrive **driveItem**</span></span>    | <span data-ttu-id="f6211-227">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="f6211-227">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f6211-228">**Lista** do Microsoft Office SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f6211-228">SharePoint **list**</span></span>    | <span data-ttu-id="f6211-229">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="f6211-229">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f6211-230">Outlook **mensagem** , **evento** , **contato**</span><span class="sxs-lookup"><span data-stu-id="f6211-230">Outlook **message** , **event** , **contact**</span></span>              | <span data-ttu-id="f6211-231">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="f6211-231">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f6211-232">**usuário** , **grupo** , outros recursos de diretório</span><span class="sxs-lookup"><span data-stu-id="f6211-232">**user** , **group** , other directory resources</span></span>   | <span data-ttu-id="f6211-233">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="f6211-233">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f6211-234">**presence**</span><span class="sxs-lookup"><span data-stu-id="f6211-234">**presence**</span></span>        | <span data-ttu-id="f6211-235">60 minutos (1 hora)</span><span class="sxs-lookup"><span data-stu-id="f6211-235">60 minutes (1 hour)</span></span> |
| <span data-ttu-id="f6211-236">Imprimir **printTaskDefinition**</span><span class="sxs-lookup"><span data-stu-id="f6211-236">Print **printTaskDefinition**</span></span> | <span data-ttu-id="f6211-237">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="f6211-237">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="f6211-238">**Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado.</span><span class="sxs-lookup"><span data-stu-id="f6211-238">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="f6211-239">No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.</span><span class="sxs-lookup"><span data-stu-id="f6211-239">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="f6211-240">Relações</span><span class="sxs-lookup"><span data-stu-id="f6211-240">Relationships</span></span>

<span data-ttu-id="f6211-241">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6211-241">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6211-242">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6211-242">JSON representation</span></span>

<span data-ttu-id="f6211-243">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6211-243">Here is a JSON representation of the resource.</span></span>

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


