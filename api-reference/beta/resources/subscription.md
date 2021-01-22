---
title: tipo de recurso de assinatura
description: 'Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: e34f6f04545c9f878e5429e54923ef223a883547
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934799"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="c3afc-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="c3afc-104">subscription resource type</span></span>

<span data-ttu-id="c3afc-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3afc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3afc-106">Uma assinatura que permite a um aplicativo cliente receber notificações sobre alterações de dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c3afc-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="c3afc-107">Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:</span><span class="sxs-lookup"><span data-stu-id="c3afc-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="c3afc-108">Um [alerta][] do Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="c3afc-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="c3afc-109">Uma [callRecord][] produzida após uma chamada ou uma reunião no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c3afc-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="c3afc-110">Um [chatMessage][] enviado por meio de equipes ou canais no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c3afc-110">A [chatMessage][] sent via teams or channels in Microsoft Teams</span></span>
- <span data-ttu-id="c3afc-111">Uma [conversa][] em um grupo no Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c3afc-111">A [conversation][] in a Microsoft 365 group</span></span>
- <span data-ttu-id="c3afc-112">Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="c3afc-112">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="c3afc-113">Uma [lista][] em um [site][] do SharePoint</span><span class="sxs-lookup"><span data-stu-id="c3afc-113">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="c3afc-114">Uma [mensagem][], [evento][] ou [contato][] no Outlook</span><span class="sxs-lookup"><span data-stu-id="c3afc-114">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="c3afc-115">A [presença][] de um usuário no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c3afc-115">The [presence][] of a user in Microsoft Teams</span></span>
- <span data-ttu-id="c3afc-116">Um [usuário][] ou [grupo][] no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c3afc-116">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="c3afc-117">Uma [impressora][] no Serviço de Impressão (quando um trabalho de impressão para a impressora chega ao estado JobFetchable – pronto para ser buscado para impressão).</span><span class="sxs-lookup"><span data-stu-id="c3afc-117">A [printer][] in Print Service (when a print job for the printer gets to JobFetchable state - ready to be fetched for printing).</span></span>
- <span data-ttu-id="c3afc-118">Uma [printTaskDefinition][] no Serviço de Impressão</span><span class="sxs-lookup"><span data-stu-id="c3afc-118">A [printTaskDefinition][] in Print Service</span></span>
- <span data-ttu-id="c3afc-119">Um [todoTask] de um usuário no Microsoft To Do</span><span class="sxs-lookup"><span data-stu-id="c3afc-119">A [todoTask] of a user in Microsoft To Do</span></span>

<span data-ttu-id="c3afc-120">Consulte [usar o Microsoft Graph API para obter notificações de alteração](webhooks.md) dos possíveis valores de caminho de recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="c3afc-120">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="c3afc-121">Métodos</span><span class="sxs-lookup"><span data-stu-id="c3afc-121">Methods</span></span>

| <span data-ttu-id="c3afc-122">Método</span><span class="sxs-lookup"><span data-stu-id="c3afc-122">Method</span></span> | <span data-ttu-id="c3afc-123">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c3afc-123">Return Type</span></span> | <span data-ttu-id="c3afc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3afc-124">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="c3afc-125">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="c3afc-125">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="c3afc-126">assinatura</span><span class="sxs-lookup"><span data-stu-id="c3afc-126">subscription</span></span>](subscription.md) | <span data-ttu-id="c3afc-127">Assina um aplicativo de escuta para receber notificações sobre alterações nos dados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c3afc-127">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="c3afc-128">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="c3afc-128">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="c3afc-129">subscription</span><span class="sxs-lookup"><span data-stu-id="c3afc-129">subscription</span></span>](subscription.md) | <span data-ttu-id="c3afc-130">Renove uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="c3afc-130">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="c3afc-131">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="c3afc-131">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="c3afc-132">assinatura</span><span class="sxs-lookup"><span data-stu-id="c3afc-132">subscription</span></span>](subscription.md) | <span data-ttu-id="c3afc-133">Lista assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="c3afc-133">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="c3afc-134">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="c3afc-134">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="c3afc-135">subscription</span><span class="sxs-lookup"><span data-stu-id="c3afc-135">subscription</span></span>](subscription.md) | <span data-ttu-id="c3afc-136">Leia as propriedades e os relacionamentos do objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="c3afc-136">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="c3afc-137">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="c3afc-137">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="c3afc-138">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c3afc-138">None</span></span> | <span data-ttu-id="c3afc-139">Exclua um objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="c3afc-139">Delete a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c3afc-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3afc-140">Properties</span></span>

| <span data-ttu-id="c3afc-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3afc-141">Property</span></span> | <span data-ttu-id="c3afc-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3afc-142">Type</span></span> | <span data-ttu-id="c3afc-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3afc-143">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="c3afc-144">changeType</span><span class="sxs-lookup"><span data-stu-id="c3afc-144">changeType</span></span> | <span data-ttu-id="c3afc-145">string</span><span class="sxs-lookup"><span data-stu-id="c3afc-145">string</span></span> | <span data-ttu-id="c3afc-146">Indica qual é o tipo de alteração no recurso inscrito que irá emitir uma notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="c3afc-146">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="c3afc-147">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="c3afc-147">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="c3afc-148">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="c3afc-148">Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="c3afc-149">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3afc-149">Required.</span></span> <br><br><span data-ttu-id="c3afc-150">Observação: As notificações de alteração de lista e item raiz da unidade suportam apenas o `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="c3afc-150">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="c3afc-151">Suporte para notificações de alteração de usuário e grupo `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="c3afc-151">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="c3afc-152">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="c3afc-152">notificationUrl</span></span> | <span data-ttu-id="c3afc-153">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3afc-153">string</span></span> | <span data-ttu-id="c3afc-154">A URL do ponto de extremidade que recebe as notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="c3afc-154">The URL of the endpoint that receives the change notifications.</span></span> <span data-ttu-id="c3afc-155">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="c3afc-155">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="c3afc-156">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3afc-156">Required.</span></span> |
| <span data-ttu-id="c3afc-157">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="c3afc-157">lifecycleNotificationUrl</span></span> | <span data-ttu-id="c3afc-158">string</span><span class="sxs-lookup"><span data-stu-id="c3afc-158">string</span></span> | <span data-ttu-id="c3afc-159">A URL do ponto de extremidade que recebe notificações de ciclo de vida, incluindo `subscriptionRemoved` `missed` e notificações.</span><span class="sxs-lookup"><span data-stu-id="c3afc-159">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="c3afc-160">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="c3afc-160">This URL must make use of the HTTPS protocol.</span></span> <span data-ttu-id="c3afc-161">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c3afc-161">Optional.</span></span> <br><br><span data-ttu-id="c3afc-162">[Leia mais sobre](/graph/webhooks-lifecycle) como os recursos do Outlook usam notificações de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="c3afc-162">[Read more](/graph/webhooks-lifecycle) about how Outlook resources use lifecycle notifications.</span></span> |
| <span data-ttu-id="c3afc-163">recurso</span><span class="sxs-lookup"><span data-stu-id="c3afc-163">resource</span></span> | <span data-ttu-id="c3afc-164">string</span><span class="sxs-lookup"><span data-stu-id="c3afc-164">string</span></span> | <span data-ttu-id="c3afc-165">Especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="c3afc-165">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="c3afc-166">Não incluir a URL base (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="c3afc-166">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> <span data-ttu-id="c3afc-167">Consulte os possíveis valores do [caminho](webhooks.md) do recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="c3afc-167">See the possible resource path [values](webhooks.md) for each supported resource.</span></span> <span data-ttu-id="c3afc-168">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3afc-168">Required.</span></span> |
| <span data-ttu-id="c3afc-169">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c3afc-169">expirationDateTime</span></span> | <span data-ttu-id="c3afc-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3afc-170">DateTimeOffset</span></span> | <span data-ttu-id="c3afc-171">Especifica a data e a hora em que a assinatura do webhook expira.</span><span class="sxs-lookup"><span data-stu-id="c3afc-171">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="c3afc-172">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="c3afc-172">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="c3afc-173">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="c3afc-173">See the table below for maximum supported subscription length of time.</span></span> <span data-ttu-id="c3afc-174">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3afc-174">Required.</span></span> |
| <span data-ttu-id="c3afc-175">clientState</span><span class="sxs-lookup"><span data-stu-id="c3afc-175">clientState</span></span> | <span data-ttu-id="c3afc-176">string</span><span class="sxs-lookup"><span data-stu-id="c3afc-176">string</span></span> | <span data-ttu-id="c3afc-177">Especifica o valor da propriedade **clientState** enviada pelo serviço em cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="c3afc-177">Specifies the value of the **clientState** property sent by the service in each change notification.</span></span> <span data-ttu-id="c3afc-178">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="c3afc-178">The maximum length is 255 characters.</span></span> <span data-ttu-id="c3afc-179">O cliente pode verificar se a notificação de alteração veio do serviço comparando o valor da propriedade **clientState** enviada com a assinatura com o valor da propriedade **clientState** recebida com cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="c3afc-179">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="c3afc-180">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c3afc-180">Optional.</span></span> |
| <span data-ttu-id="c3afc-181">id</span><span class="sxs-lookup"><span data-stu-id="c3afc-181">id</span></span> | <span data-ttu-id="c3afc-182">string</span><span class="sxs-lookup"><span data-stu-id="c3afc-182">string</span></span> | <span data-ttu-id="c3afc-p110">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3afc-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="c3afc-185">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="c3afc-185">applicationId</span></span> | <span data-ttu-id="c3afc-186">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3afc-186">string</span></span> | <span data-ttu-id="c3afc-187">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="c3afc-187">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="c3afc-188">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3afc-188">Read-only.</span></span> |
| <span data-ttu-id="c3afc-189">creatorId</span><span class="sxs-lookup"><span data-stu-id="c3afc-189">creatorId</span></span> | <span data-ttu-id="c3afc-190">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3afc-190">string</span></span> | <span data-ttu-id="c3afc-191">Identificador de usuário ou entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="c3afc-191">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="c3afc-192">Se o aplicativo usou permissões delegadas para criar a assinatura, esse campo contém a ID do usuário que o aplicativo chamou em nome dele.</span><span class="sxs-lookup"><span data-stu-id="c3afc-192">If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="c3afc-193">Se o aplicativo usou permissões de aplicativo, esse campo contém a ID da entidade de serviço correspondente ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c3afc-193">If the app used application permissions, this field contains the ID of the service principal corresponding to the app.</span></span> <span data-ttu-id="c3afc-194">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3afc-194">Read-only.</span></span> |
| <span data-ttu-id="c3afc-195">includeResourceData</span><span class="sxs-lookup"><span data-stu-id="c3afc-195">includeResourceData</span></span> | <span data-ttu-id="c3afc-196">Booleano</span><span class="sxs-lookup"><span data-stu-id="c3afc-196">Boolean</span></span> | <span data-ttu-id="c3afc-197">Quando definido como `true`, alterar as notificações [inclui dados de recurso](/graph/webhooks-with-resource-data) (como o conteúdo de uma mensagem de bate-papo).</span><span class="sxs-lookup"><span data-stu-id="c3afc-197">When set to `true`, change notifications [include resource data](/graph/webhooks-with-resource-data) (such as content of a chat message).</span></span> <span data-ttu-id="c3afc-198">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c3afc-198">Optional.</span></span> | 
| <span data-ttu-id="c3afc-199">encryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="c3afc-199">encryptionCertificate</span></span> | <span data-ttu-id="c3afc-200">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3afc-200">string</span></span> | <span data-ttu-id="c3afc-201">Uma representação codificada em Base64 de um certificado com uma chave pública usada para criptografar os dados de recursos nas notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="c3afc-201">A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.</span></span> <span data-ttu-id="c3afc-202">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c3afc-202">Optional.</span></span> <span data-ttu-id="c3afc-203">Obrigatório quando **includeResourceData** é verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="c3afc-203">Required when **includeResourceData** is true.</span></span> | 
| <span data-ttu-id="c3afc-204">encryptionCertificateId</span><span class="sxs-lookup"><span data-stu-id="c3afc-204">encryptionCertificateId</span></span> | <span data-ttu-id="c3afc-205">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3afc-205">string</span></span> | <span data-ttu-id="c3afc-206">Um identificador personalizado fornecido pelo aplicativo para ajudar a identificar o certificado necessário para descriptografar os dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3afc-206">A custom app-provided identifier to help identify the certificate needed to decrypt resource data.</span></span> <span data-ttu-id="c3afc-207">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c3afc-207">Optional.</span></span> <span data-ttu-id="c3afc-208">Obrigatório quando **includeResourceData** é verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="c3afc-208">Required when **includeResourceData** is true.</span></span> |
| <span data-ttu-id="c3afc-209">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="c3afc-209">latestSupportedTlsVersion</span></span> | <span data-ttu-id="c3afc-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3afc-210">String</span></span> | <span data-ttu-id="c3afc-211">Especifica a versão mais recente do protocolo TLS que o ponto de extremidade, especificado por **notificationUrl**, é compatível.</span><span class="sxs-lookup"><span data-stu-id="c3afc-211">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="c3afc-212">Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="c3afc-212">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="c3afc-213">Para os assinantes cujo ponto de extremidade de notificação suporta uma versão menor que a versão recomendada atualmente (TLS 1.2), especificar essa propriedade por uma [linha do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) definida, permite o uso temporário da versão preterida do TLS antes de concluir a atualização para o TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="c3afc-213">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="c3afc-214">Para esses assinantes, não definir essa propriedade pela linha do tempo resultaria em uma falha nas operações da assinatura.</span><span class="sxs-lookup"><span data-stu-id="c3afc-214">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="c3afc-215">Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="c3afc-215">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="c3afc-216">Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="c3afc-216">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="c3afc-217">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="c3afc-217">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="c3afc-218">Resource</span><span class="sxs-lookup"><span data-stu-id="c3afc-218">Resource</span></span>            | <span data-ttu-id="c3afc-219">Tempo de expiração máximo</span><span class="sxs-lookup"><span data-stu-id="c3afc-219">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="c3afc-220">**Alerta** de segurança</span><span class="sxs-lookup"><span data-stu-id="c3afc-220">Security **alert**</span></span>     | <span data-ttu-id="c3afc-221">43200 minutos (em 30 dias )</span><span class="sxs-lookup"><span data-stu-id="c3afc-221">43200 minutes (under 30 days)</span></span>  |
| <span data-ttu-id="c3afc-222">Teams **callRecord**</span><span class="sxs-lookup"><span data-stu-id="c3afc-222">Teams **callRecord**</span></span>    | <span data-ttu-id="c3afc-223">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c3afc-223">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="c3afc-224">Teams **chatMessage**</span><span class="sxs-lookup"><span data-stu-id="c3afc-224">Teams **chatMessage**</span></span>    | <span data-ttu-id="c3afc-225">60 minutos (1 hora)</span><span class="sxs-lookup"><span data-stu-id="c3afc-225">60 minutes (1 hour)</span></span>  |
| <span data-ttu-id="c3afc-226">**Conversa** em grupo</span><span class="sxs-lookup"><span data-stu-id="c3afc-226">Group **conversation**</span></span> | <span data-ttu-id="c3afc-227">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c3afc-227">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c3afc-228">OneDrive **driveItem**</span><span class="sxs-lookup"><span data-stu-id="c3afc-228">OneDrive **driveItem**</span></span>    | <span data-ttu-id="c3afc-229">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c3afc-229">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c3afc-230">**Lista** do Microsoft Office SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c3afc-230">SharePoint **list**</span></span>    | <span data-ttu-id="c3afc-231">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c3afc-231">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c3afc-232">Outlook **mensagem**, **evento**, **contato**</span><span class="sxs-lookup"><span data-stu-id="c3afc-232">Outlook **message**, **event**, **contact**</span></span>              | <span data-ttu-id="c3afc-233">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c3afc-233">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c3afc-234">**usuário**, **grupo**, outros recursos de diretório</span><span class="sxs-lookup"><span data-stu-id="c3afc-234">**user**, **group**, other directory resources</span></span>   | <span data-ttu-id="c3afc-235">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c3afc-235">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c3afc-236">**presence**</span><span class="sxs-lookup"><span data-stu-id="c3afc-236">**presence**</span></span>        | <span data-ttu-id="c3afc-237">60 minutos (1 hora)</span><span class="sxs-lookup"><span data-stu-id="c3afc-237">60 minutes (1 hour)</span></span> |
| <span data-ttu-id="c3afc-238">Impressora **de impressão**</span><span class="sxs-lookup"><span data-stu-id="c3afc-238">Print **printer**</span></span> | <span data-ttu-id="c3afc-239">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c3afc-239">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c3afc-240">**PrintTaskDefinition**</span><span class="sxs-lookup"><span data-stu-id="c3afc-240">Print **printTaskDefinition**</span></span> | <span data-ttu-id="c3afc-241">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c3afc-241">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c3afc-242">**todoTask**</span><span class="sxs-lookup"><span data-stu-id="c3afc-242">**todoTask**</span></span>              | <span data-ttu-id="c3afc-243">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c3afc-243">4230 minutes (under 3 days)</span></span>    |


> <span data-ttu-id="c3afc-244">**Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado.</span><span class="sxs-lookup"><span data-stu-id="c3afc-244">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="c3afc-245">No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.</span><span class="sxs-lookup"><span data-stu-id="c3afc-245">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="c3afc-246">Relações</span><span class="sxs-lookup"><span data-stu-id="c3afc-246">Relationships</span></span>

<span data-ttu-id="c3afc-247">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c3afc-247">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3afc-248">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3afc-248">JSON representation</span></span>

<span data-ttu-id="c3afc-249">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3afc-249">Here is a JSON representation of the resource.</span></span>

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
[impressora]: ./printer.md
[printer]: ./printer.md
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


