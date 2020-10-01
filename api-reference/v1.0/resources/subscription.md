---
title: tipo de recurso de assinatura
description: 'Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3a82995a88b3dd5829b0f1f7c9b2cb5bcb5dfa18
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314654"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="cef84-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="cef84-104">subscription resource type</span></span>

<span data-ttu-id="cef84-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cef84-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cef84-106">Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cef84-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="cef84-107">Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:</span><span class="sxs-lookup"><span data-stu-id="cef84-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="cef84-108">Um [alerta][] do Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="cef84-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="cef84-109">Uma [callRecord][] produzida após uma chamada ou uma reunião no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="cef84-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="cef84-110">Um [chatMessage][] enviado por meio de equipes ou canais no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="cef84-110">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="cef84-111">Uma [conversa][] em um grupo no Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="cef84-111">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="cef84-112">Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="cef84-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="cef84-113">Uma [lista][] em um [site][] do SharePoint</span><span class="sxs-lookup"><span data-stu-id="cef84-113">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="cef84-114">Uma [mensagem][], [evento][] ou [contato][] no Outlook</span><span class="sxs-lookup"><span data-stu-id="cef84-114">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="cef84-115">Um [usuário][] ou [grupo][] no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="cef84-115">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="cef84-116">Consulte [usar o Microsoft Graph API para obter notificações de alteração](webhooks.md) dos possíveis valores de caminho de recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="cef84-116">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="cef84-117">Métodos</span><span class="sxs-lookup"><span data-stu-id="cef84-117">Methods</span></span>

| <span data-ttu-id="cef84-118">Método</span><span class="sxs-lookup"><span data-stu-id="cef84-118">Method</span></span> | <span data-ttu-id="cef84-119">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cef84-119">Return Type</span></span> | <span data-ttu-id="cef84-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cef84-120">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="cef84-121">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="cef84-121">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="cef84-122">assinatura</span><span class="sxs-lookup"><span data-stu-id="cef84-122">subscription</span></span>](subscription.md) | <span data-ttu-id="cef84-123">Assina um aplicativo de escuta para receber notificações sobre alterações nos dados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cef84-123">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="cef84-124">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="cef84-124">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="cef84-125">subscription</span><span class="sxs-lookup"><span data-stu-id="cef84-125">subscription</span></span>](subscription.md) | <span data-ttu-id="cef84-126">Renova uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="cef84-126">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="cef84-127">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="cef84-127">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="cef84-128">assinatura</span><span class="sxs-lookup"><span data-stu-id="cef84-128">subscription</span></span>](subscription.md) | <span data-ttu-id="cef84-129">Lista assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="cef84-129">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="cef84-130">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="cef84-130">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="cef84-131">subscription</span><span class="sxs-lookup"><span data-stu-id="cef84-131">subscription</span></span>](subscription.md) | <span data-ttu-id="cef84-132">Lê as propriedades e as relações do objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="cef84-132">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="cef84-133">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="cef84-133">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="cef84-134">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="cef84-134">None</span></span> | <span data-ttu-id="cef84-135">Exclui um objeto assinatura.</span><span class="sxs-lookup"><span data-stu-id="cef84-135">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cef84-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cef84-136">Properties</span></span>

| <span data-ttu-id="cef84-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cef84-137">Property</span></span> | <span data-ttu-id="cef84-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="cef84-138">Type</span></span> | <span data-ttu-id="cef84-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="cef84-139">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="cef84-140">changeType</span><span class="sxs-lookup"><span data-stu-id="cef84-140">changeType</span></span> | <span data-ttu-id="cef84-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cef84-141">string</span></span> | <span data-ttu-id="cef84-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cef84-142">Required.</span></span> <span data-ttu-id="cef84-143">Indica qual é o tipo de alteração no recurso inscrito que irá emitir uma notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="cef84-143">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="cef84-144">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="cef84-144">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="cef84-145">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="cef84-145">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="cef84-146">Observação: As notificações de alteração de lista e item raiz da unidade suportam apenas o `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="cef84-146">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="cef84-147">Suporte para notificações de alteração de usuário e grupo `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="cef84-147">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="cef84-148">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="cef84-148">notificationUrl</span></span> | <span data-ttu-id="cef84-149">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cef84-149">string</span></span> | <span data-ttu-id="cef84-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cef84-150">Required.</span></span> <span data-ttu-id="cef84-151">O URL do ponto de extremidade que receberá as notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="cef84-151">The URL of the endpoint that will receive the change notifications.</span></span> <span data-ttu-id="cef84-152">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="cef84-152">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="cef84-153">recurso</span><span class="sxs-lookup"><span data-stu-id="cef84-153">resource</span></span> | <span data-ttu-id="cef84-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cef84-154">string</span></span> | <span data-ttu-id="cef84-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cef84-155">Required.</span></span> <span data-ttu-id="cef84-156">Especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="cef84-156">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="cef84-157">Não incluir a URL base (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="cef84-157">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> <span data-ttu-id="cef84-158">Consulte os possíveis valores do [caminho](webhooks.md) do recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="cef84-158">See the possible resource path [values](webhooks.md) for each supported resource.</span></span>|
| <span data-ttu-id="cef84-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cef84-159">expirationDateTime</span></span> | [<span data-ttu-id="cef84-160">dateTime</span><span class="sxs-lookup"><span data-stu-id="cef84-160">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="cef84-161">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cef84-161">Required.</span></span> <span data-ttu-id="cef84-162">Especifica a data e a hora em que a assinatura do webhook expira.</span><span class="sxs-lookup"><span data-stu-id="cef84-162">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="cef84-163">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="cef84-163">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="cef84-164">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="cef84-164">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="cef84-165">clientState</span><span class="sxs-lookup"><span data-stu-id="cef84-165">clientState</span></span> | <span data-ttu-id="cef84-166">string</span><span class="sxs-lookup"><span data-stu-id="cef84-166">string</span></span> | <span data-ttu-id="cef84-167">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cef84-167">Optional.</span></span> <span data-ttu-id="cef84-168">Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="cef84-168">Specifies the value of the `clientState` property sent by the service in each change notification.</span></span> <span data-ttu-id="cef84-169">O comprimento máximo é de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="cef84-169">The maximum length is 128 characters.</span></span> <span data-ttu-id="cef84-170">O cliente pode verificar se a notificação de alteração veio do serviço pela comparação do valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida contendo cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="cef84-170">The client can check that the change notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each change notification.</span></span> |
| <span data-ttu-id="cef84-171">id</span><span class="sxs-lookup"><span data-stu-id="cef84-171">id</span></span> | <span data-ttu-id="cef84-172">string</span><span class="sxs-lookup"><span data-stu-id="cef84-172">string</span></span> | <span data-ttu-id="cef84-p109">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cef84-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="cef84-175">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="cef84-175">applicationId</span></span> | <span data-ttu-id="cef84-176">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cef84-176">string</span></span> | <span data-ttu-id="cef84-177">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="cef84-177">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="cef84-178">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cef84-178">Read-only.</span></span> |
| <span data-ttu-id="cef84-179">creatorId</span><span class="sxs-lookup"><span data-stu-id="cef84-179">creatorId</span></span> | <span data-ttu-id="cef84-180">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cef84-180">string</span></span> | <span data-ttu-id="cef84-181">Identificador de usuário ou entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="cef84-181">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="cef84-182">Se o aplicativo usado delegada permissões para criar a assinatura, esse campo contém a id do usuário que entrou no aplicativo chamado em nome dele.</span><span class="sxs-lookup"><span data-stu-id="cef84-182">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="cef84-183">Se o aplicativo usou permissões do aplicativo, esse campo contém a id da entidade de serviço correspondente ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cef84-183">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="cef84-184">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cef84-184">Read-only.</span></span> |
| <span data-ttu-id="cef84-185">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="cef84-185">includeResourceData</span></span> | <span data-ttu-id="cef84-186">Booleano</span><span class="sxs-lookup"><span data-stu-id="cef84-186">Boolean</span></span> | <span data-ttu-id="cef84-187">Quando definido como `true`, alterar as notificações [inclui dados de recurso](/graph/webhooks-with-resource-data) (como o conteúdo de uma mensagem de bate-papo).</span><span class="sxs-lookup"><span data-stu-id="cef84-187">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="cef84-188">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cef84-188">Optional.</span></span> | 
| <span data-ttu-id="cef84-189">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="cef84-189">encryptionCertificate</span></span> | <span data-ttu-id="cef84-190">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cef84-190">string</span></span> | <span data-ttu-id="cef84-191">Uma representação codificada em Base64 de um certificado com uma chave pública usada para criptografar os dados de recursos nas notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="cef84-191">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="cef84-192">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cef84-192">Optional.</span></span> <span data-ttu-id="cef84-193">Obrigatório quando **includeResourceData** é verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="cef84-193">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="cef84-194">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="cef84-194">encryptionCertificateId</span></span> | <span data-ttu-id="cef84-195">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cef84-195">string</span></span> | <span data-ttu-id="cef84-196">Um identificador personalizado fornecido pelo aplicativo para ajudar a identificar o certificado necessário para descriptografar os dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="cef84-196">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="cef84-197">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cef84-197">Optional.</span></span> 
| <span data-ttu-id="cef84-198">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="cef84-198">latestSupportedTlsVersion</span></span> | <span data-ttu-id="cef84-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cef84-199">String</span></span> | <span data-ttu-id="cef84-200">Especifica a versão mais recente do protocolo TLS que o ponto de extremidade, especificado por **notificationUrl**, é compatível.</span><span class="sxs-lookup"><span data-stu-id="cef84-200">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="cef84-201">Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="cef84-201">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="cef84-202">Para os assinantes cujo ponto de extremidade de notificação suporta uma versão menor que a versão recomendada atualmente (TLS 1.2), especificar essa propriedade por uma [linha do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) definida, permite o uso temporário da versão preterida do TLS antes de concluir a atualização para o TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="cef84-202">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="cef84-203">Para esses assinantes, não definir essa propriedade pela linha do tempo resultaria em uma falha nas operações da assinatura.</span><span class="sxs-lookup"><span data-stu-id="cef84-203">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="cef84-204">Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="cef84-204">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="cef84-205">Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="cef84-205">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="cef84-206">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="cef84-206">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="cef84-207">Resource</span><span class="sxs-lookup"><span data-stu-id="cef84-207">Resource</span></span>            | <span data-ttu-id="cef84-208">Tempo de expiração máximo</span><span class="sxs-lookup"><span data-stu-id="cef84-208">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="cef84-209">**Alerta** de segurança</span><span class="sxs-lookup"><span data-stu-id="cef84-209">Security **alert**</span></span>     | <span data-ttu-id="cef84-210">43200 minutos (em 30 dias )</span><span class="sxs-lookup"><span data-stu-id="cef84-210">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="cef84-211">Teams **callRecord**</span><span class="sxs-lookup"><span data-stu-id="cef84-211">Teams **callRecord**</span></span>    | <span data-ttu-id="cef84-212">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="cef84-212">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="cef84-213">Teams **chatMessage**</span><span class="sxs-lookup"><span data-stu-id="cef84-213">Teams **chatMessage**</span></span>    | <span data-ttu-id="cef84-214">60 minutos (1 hora)</span><span class="sxs-lookup"><span data-stu-id="cef84-214">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="cef84-215">**Conversa** em grupo</span><span class="sxs-lookup"><span data-stu-id="cef84-215">Group **conversation**</span></span> | <span data-ttu-id="cef84-216">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="cef84-216">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="cef84-217">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="cef84-217">OneDrive **driveItem**</span></span>    | <span data-ttu-id="cef84-218">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="cef84-218">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="cef84-219">**Lista** do Microsoft Office SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="cef84-219">SharePoint **list**</span></span>    | <span data-ttu-id="cef84-220">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="cef84-220">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="cef84-221">Outlook **mensagem**, **evento**, **contato**</span><span class="sxs-lookup"><span data-stu-id="cef84-221">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="cef84-222">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="cef84-222">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="cef84-223">**usuário**, **grupo**, outros recursos de diretório</span><span class="sxs-lookup"><span data-stu-id="cef84-223">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="cef84-224">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="cef84-224">4230 minutes (under 3 days)</span></span>    |

> <span data-ttu-id="cef84-225">**Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado.</span><span class="sxs-lookup"><span data-stu-id="cef84-225">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="cef84-226">No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.</span><span class="sxs-lookup"><span data-stu-id="cef84-226">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="cef84-227">Relações</span><span class="sxs-lookup"><span data-stu-id="cef84-227">Relationships</span></span>

<span data-ttu-id="cef84-228">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cef84-228">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cef84-229">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cef84-229">JSON representation</span></span>

<span data-ttu-id="cef84-230">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cef84-230">Here is a JSON representation of the resource.</span></span>

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
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

