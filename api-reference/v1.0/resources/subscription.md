---
title: tipo de recurso de assinatura
description: 'Uma assinatura permite que um aplicativo cliente receba notificações de alteração sobre as alterações nos dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b5f71bdeca19834b8d4721aaa6e8416916a15b58
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491795"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="e3df6-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="e3df6-104">subscription resource type</span></span>

<span data-ttu-id="e3df6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3df6-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3df6-106">Uma assinatura permite que um aplicativo cliente receba notificações de alteração sobre as alterações nos dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e3df6-106">A subscription allows a client app to receive change notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="e3df6-107">Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:</span><span class="sxs-lookup"><span data-stu-id="e3df6-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="e3df6-108">Um [alerta][] do Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="e3df6-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="e3df6-109">Uma [callRecord][] produzida após uma chamada ou reunião no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e3df6-109">A [callRecord][] produced after a call or meeting in Microsoft Teams</span></span>
- <span data-ttu-id="e3df6-110">Um [conversa][] de um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="e3df6-110">A [conversation][] in an Office 365 group</span></span>
- <span data-ttu-id="e3df6-111">Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="e3df6-111">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="e3df6-112">Uma [lista][] em um [site][] do SharePoint</span><span class="sxs-lookup"><span data-stu-id="e3df6-112">A [list][] under a SharePoint [site][]</span></span>
- <span data-ttu-id="e3df6-113">Uma [mensagem][], [evento][] ou [contato][] no Outlook</span><span class="sxs-lookup"><span data-stu-id="e3df6-113">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="e3df6-114">Um [usuário][] ou [grupo][] no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e3df6-114">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="e3df6-115">Consulte [usar o Microsoft Graph API para obter notificações de alteração](webhooks.md) dos possíveis valores de caminho de recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="e3df6-115">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="e3df6-116">Métodos</span><span class="sxs-lookup"><span data-stu-id="e3df6-116">Methods</span></span>

| <span data-ttu-id="e3df6-117">Método</span><span class="sxs-lookup"><span data-stu-id="e3df6-117">Method</span></span> | <span data-ttu-id="e3df6-118">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e3df6-118">Return Type</span></span> | <span data-ttu-id="e3df6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3df6-119">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="e3df6-120">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="e3df6-120">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="e3df6-121">assinatura</span><span class="sxs-lookup"><span data-stu-id="e3df6-121">subscription</span></span>](subscription.md) | <span data-ttu-id="e3df6-122">Assina um aplicativo de escuta para receber notificações de alteração quando os dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="e3df6-122">Subscribes a listener application to receive change notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="e3df6-123">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="e3df6-123">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="e3df6-124">subscription</span><span class="sxs-lookup"><span data-stu-id="e3df6-124">subscription</span></span>](subscription.md) | <span data-ttu-id="e3df6-125">Renova uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="e3df6-125">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="e3df6-126">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="e3df6-126">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="e3df6-127">assinatura</span><span class="sxs-lookup"><span data-stu-id="e3df6-127">subscription</span></span>](subscription.md) | <span data-ttu-id="e3df6-128">Lista assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="e3df6-128">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="e3df6-129">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="e3df6-129">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="e3df6-130">subscription</span><span class="sxs-lookup"><span data-stu-id="e3df6-130">subscription</span></span>](subscription.md) | <span data-ttu-id="e3df6-131">Lê as propriedades e as relações do objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="e3df6-131">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="e3df6-132">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="e3df6-132">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="e3df6-133">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e3df6-133">None</span></span> | <span data-ttu-id="e3df6-134">Exclui um objeto assinatura.</span><span class="sxs-lookup"><span data-stu-id="e3df6-134">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e3df6-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3df6-135">Properties</span></span>

| <span data-ttu-id="e3df6-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3df6-136">Property</span></span> | <span data-ttu-id="e3df6-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3df6-137">Type</span></span> | <span data-ttu-id="e3df6-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3df6-138">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="e3df6-139">changeType</span><span class="sxs-lookup"><span data-stu-id="e3df6-139">changeType</span></span> | <span data-ttu-id="e3df6-140">string</span><span class="sxs-lookup"><span data-stu-id="e3df6-140">string</span></span> | <span data-ttu-id="e3df6-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3df6-141">Required.</span></span> <span data-ttu-id="e3df6-142">Indica o tipo de alteração no recurso inscrito que irá gerar uma notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="e3df6-142">Indicates the type of change in the subscribed resource that will raise a change notification.</span></span> <span data-ttu-id="e3df6-143">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="e3df6-143">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="e3df6-144">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="e3df6-144">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="e3df6-145">Observação: as notificações de alteração de item e de lista da raiz da unidade dão suporte somente a `updated` ChangeType.</span><span class="sxs-lookup"><span data-stu-id="e3df6-145">Note: Drive root item and list change notifications support only the `updated` changeType.</span></span> <span data-ttu-id="e3df6-146">Suporte `updated` e ChangeType de notificações de alteração de grupo e usuário `deleted` .</span><span class="sxs-lookup"><span data-stu-id="e3df6-146">User and group change notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="e3df6-147">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="e3df6-147">notificationUrl</span></span> | <span data-ttu-id="e3df6-148">string</span><span class="sxs-lookup"><span data-stu-id="e3df6-148">string</span></span> | <span data-ttu-id="e3df6-149">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3df6-149">Required.</span></span> <span data-ttu-id="e3df6-150">A URL do ponto de extremidade que receberá as notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="e3df6-150">The URL of the endpoint that will receive the change notifications.</span></span> <span data-ttu-id="e3df6-151">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="e3df6-151">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="e3df6-152">recurso</span><span class="sxs-lookup"><span data-stu-id="e3df6-152">resource</span></span> | <span data-ttu-id="e3df6-153">string</span><span class="sxs-lookup"><span data-stu-id="e3df6-153">string</span></span> | <span data-ttu-id="e3df6-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3df6-154">Required.</span></span> <span data-ttu-id="e3df6-155">Especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="e3df6-155">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="e3df6-156">Não incluir a URL base (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="e3df6-156">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> <span data-ttu-id="e3df6-157">Consulte os possíveis valores do [caminho](webhooks.md) do recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="e3df6-157">See the possible resource path [values](webhooks.md) for each supported resource.</span></span>|
| <span data-ttu-id="e3df6-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e3df6-158">expirationDateTime</span></span> | [<span data-ttu-id="e3df6-159">dateTime</span><span class="sxs-lookup"><span data-stu-id="e3df6-159">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="e3df6-160">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3df6-160">Required.</span></span> <span data-ttu-id="e3df6-161">Especifica a data e a hora em que a assinatura do webhook expira.</span><span class="sxs-lookup"><span data-stu-id="e3df6-161">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="e3df6-162">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="e3df6-162">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="e3df6-163">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="e3df6-163">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="e3df6-164">clientState</span><span class="sxs-lookup"><span data-stu-id="e3df6-164">clientState</span></span> | <span data-ttu-id="e3df6-165">string</span><span class="sxs-lookup"><span data-stu-id="e3df6-165">string</span></span> | <span data-ttu-id="e3df6-166">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e3df6-166">Optional.</span></span> <span data-ttu-id="e3df6-167">Especifica o valor da `clientState` Propriedade enviada pelo serviço em cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="e3df6-167">Specifies the value of the `clientState` property sent by the service in each change notification.</span></span> <span data-ttu-id="e3df6-168">O comprimento máximo é de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="e3df6-168">The maximum length is 128 characters.</span></span> <span data-ttu-id="e3df6-169">O cliente pode verificar se a notificação de alteração veio do serviço, comparando o valor da `clientState` Propriedade enviada com a assinatura com o valor da `clientState` Propriedade recebida com cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="e3df6-169">The client can check that the change notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each change notification.</span></span> |
| <span data-ttu-id="e3df6-170">id</span><span class="sxs-lookup"><span data-stu-id="e3df6-170">id</span></span> | <span data-ttu-id="e3df6-171">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3df6-171">string</span></span> | <span data-ttu-id="e3df6-p109">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e3df6-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="e3df6-174">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="e3df6-174">applicationId</span></span> | <span data-ttu-id="e3df6-175">string</span><span class="sxs-lookup"><span data-stu-id="e3df6-175">string</span></span> | <span data-ttu-id="e3df6-176">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="e3df6-176">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="e3df6-177">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e3df6-177">Read-only.</span></span> |
| <span data-ttu-id="e3df6-178">creatorId</span><span class="sxs-lookup"><span data-stu-id="e3df6-178">creatorId</span></span> | <span data-ttu-id="e3df6-179">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3df6-179">string</span></span> | <span data-ttu-id="e3df6-180">Identificador de usuário ou entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="e3df6-180">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="e3df6-181">Se o aplicativo usado delegada permissões para criar a assinatura, esse campo contém a id do usuário que entrou no aplicativo chamado em nome dele.</span><span class="sxs-lookup"><span data-stu-id="e3df6-181">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="e3df6-182">Se o aplicativo usou permissões do aplicativo, esse campo contém a id da entidade de serviço correspondente ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3df6-182">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="e3df6-183">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="e3df6-183">Read-only.</span></span> |
| <span data-ttu-id="e3df6-184">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="e3df6-184">latestSupportedTlsVersion</span></span> | <span data-ttu-id="e3df6-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3df6-185">String</span></span> | <span data-ttu-id="e3df6-186">Especifica a versão mais recente do protocolo TLS que o ponto de extremidade, especificado por **notificationUrl**, é compatível.</span><span class="sxs-lookup"><span data-stu-id="e3df6-186">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="e3df6-187">Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="e3df6-187">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="e3df6-188">Para os assinantes cujo ponto de extremidade de notificação suporta uma versão menor que a versão recomendada atualmente (TLS 1.2), especificar essa propriedade por uma [linha do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) definida, permite o uso temporário da versão preterida do TLS antes de concluir a atualização para o TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="e3df6-188">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="e3df6-189">Para esses assinantes, não definir essa propriedade pela linha do tempo resultaria em uma falha nas operações da assinatura.</span><span class="sxs-lookup"><span data-stu-id="e3df6-189">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="e3df6-190">Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="e3df6-190">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="e3df6-191">Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="e3df6-191">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="e3df6-192">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="e3df6-192">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="e3df6-193">Resource</span><span class="sxs-lookup"><span data-stu-id="e3df6-193">Resource</span></span>            | <span data-ttu-id="e3df6-194">Tempo de expiração máximo</span><span class="sxs-lookup"><span data-stu-id="e3df6-194">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="e3df6-195">Usuário, grupo, outros recursos de diretório</span><span class="sxs-lookup"><span data-stu-id="e3df6-195">User, group, other directory resources</span></span>   | <span data-ttu-id="e3df6-196">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e3df6-196">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="e3df6-197">Correio</span><span class="sxs-lookup"><span data-stu-id="e3df6-197">Mail</span></span>                | <span data-ttu-id="e3df6-198">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e3df6-198">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="e3df6-199">Calendário</span><span class="sxs-lookup"><span data-stu-id="e3df6-199">Calendar</span></span>            | <span data-ttu-id="e3df6-200">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e3df6-200">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="e3df6-201">Contatos</span><span class="sxs-lookup"><span data-stu-id="e3df6-201">Contacts</span></span>            | <span data-ttu-id="e3df6-202">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e3df6-202">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="e3df6-203">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="e3df6-203">Group conversations</span></span> | <span data-ttu-id="e3df6-204">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e3df6-204">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="e3df6-205">Itens raiz de unidade</span><span class="sxs-lookup"><span data-stu-id="e3df6-205">Drive root items</span></span>    | <span data-ttu-id="e3df6-206">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e3df6-206">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="e3df6-207">Lista do SharePoint</span><span class="sxs-lookup"><span data-stu-id="e3df6-207">SharePoint list</span></span>     | <span data-ttu-id="e3df6-208">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e3df6-208">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="e3df6-209">Teams callRecord</span><span class="sxs-lookup"><span data-stu-id="e3df6-209">Teams callRecord</span></span>    | <span data-ttu-id="e3df6-210">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="e3df6-210">4230 minutes (under 3 days)</span></span>  |
| <span data-ttu-id="e3df6-211">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="e3df6-211">Security alerts</span></span>     | <span data-ttu-id="e3df6-212">43200 minutos (em 30 dias )</span><span class="sxs-lookup"><span data-stu-id="e3df6-212">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="e3df6-213">**Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado.</span><span class="sxs-lookup"><span data-stu-id="e3df6-213">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="e3df6-214">No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.</span><span class="sxs-lookup"><span data-stu-id="e3df6-214">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="e3df6-215">Relações</span><span class="sxs-lookup"><span data-stu-id="e3df6-215">Relationships</span></span>

<span data-ttu-id="e3df6-216">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3df6-216">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3df6-217">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3df6-217">JSON representation</span></span>

<span data-ttu-id="e3df6-218">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3df6-218">Here is a JSON representation of the resource.</span></span>

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
