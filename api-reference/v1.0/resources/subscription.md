---
title: tipo de recurso de assinatura
description: 'Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a490257ccc1ba17e7e425c24126c24689c612a9b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533600"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="1e2d4-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="1e2d4-104">subscription resource type</span></span>

<span data-ttu-id="1e2d4-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e2d4-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1e2d4-106">Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-106">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="1e2d4-107">Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:</span><span class="sxs-lookup"><span data-stu-id="1e2d4-107">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="1e2d4-108">Um [alerta][] do Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="1e2d4-108">An [alert][] from the Microsoft Graph Security API</span></span>
- <span data-ttu-id="1e2d4-109">Um [conversa][] de um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="1e2d4-109">A [conversation][] in an Office 365 group</span></span>
- <span data-ttu-id="1e2d4-110">Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="1e2d4-110">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="1e2d4-111">Uma [mensagem][], [evento][] ou [contato][] no Outlook</span><span class="sxs-lookup"><span data-stu-id="1e2d4-111">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="1e2d4-112">Um [usuário][] ou [grupo][] no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1e2d4-112">A [user][] or [group][] in Azure Active Directory</span></span>

<span data-ttu-id="1e2d4-113">Consulte [usar o Microsoft Graph API para obter notificações de alteração](webhooks.md) dos possíveis valores de caminho de recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-113">See [Use the Microsoft Graph API to get change notifications](webhooks.md) for the possible resource path values for each supported resource.</span></span>

## <a name="methods"></a><span data-ttu-id="1e2d4-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="1e2d4-114">Methods</span></span>

| <span data-ttu-id="1e2d4-115">Método</span><span class="sxs-lookup"><span data-stu-id="1e2d4-115">Method</span></span> | <span data-ttu-id="1e2d4-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1e2d4-116">Return Type</span></span> | <span data-ttu-id="1e2d4-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e2d4-117">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="1e2d4-118">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="1e2d4-118">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="1e2d4-119">subscription</span><span class="sxs-lookup"><span data-stu-id="1e2d4-119">subscription</span></span>](subscription.md) | <span data-ttu-id="1e2d4-120">Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-120">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="1e2d4-121">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="1e2d4-121">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="1e2d4-122">subscription</span><span class="sxs-lookup"><span data-stu-id="1e2d4-122">subscription</span></span>](subscription.md) | <span data-ttu-id="1e2d4-123">Renova uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-123">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="1e2d4-124">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="1e2d4-124">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="1e2d4-125">assinatura</span><span class="sxs-lookup"><span data-stu-id="1e2d4-125">subscription</span></span>](subscription.md) | <span data-ttu-id="1e2d4-126">Lista assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-126">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="1e2d4-127">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="1e2d4-127">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="1e2d4-128">subscription</span><span class="sxs-lookup"><span data-stu-id="1e2d4-128">subscription</span></span>](subscription.md) | <span data-ttu-id="1e2d4-129">Lê as propriedades e as relações do objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-129">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="1e2d4-130">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="1e2d4-130">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="1e2d4-131">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1e2d4-131">None</span></span> | <span data-ttu-id="1e2d4-132">Exclui um objeto assinatura.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-132">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1e2d4-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e2d4-133">Properties</span></span>

| <span data-ttu-id="1e2d4-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e2d4-134">Property</span></span> | <span data-ttu-id="1e2d4-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e2d4-135">Type</span></span> | <span data-ttu-id="1e2d4-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e2d4-136">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="1e2d4-137">changeType</span><span class="sxs-lookup"><span data-stu-id="1e2d4-137">changeType</span></span> | <span data-ttu-id="1e2d4-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e2d4-138">string</span></span> | <span data-ttu-id="1e2d4-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-139">Required.</span></span> <span data-ttu-id="1e2d4-140">Indica o tipo de alteração no recurso inscrito que gerará uma notificação.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-140">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="1e2d4-141">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-141">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="1e2d4-142">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-142">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="1e2d4-143">Observação: As notificações do item na raiz da unidade suportam somente `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-143">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="1e2d4-144">Notificações de grupos e usuário suportam `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-144">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="1e2d4-145">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="1e2d4-145">notificationUrl</span></span> | <span data-ttu-id="1e2d4-146">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e2d4-146">string</span></span> | <span data-ttu-id="1e2d4-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-147">Required.</span></span> <span data-ttu-id="1e2d4-148">A URL do ponto de extremidade que receberá as notificações.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-148">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="1e2d4-149">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-149">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="1e2d4-150">recurso</span><span class="sxs-lookup"><span data-stu-id="1e2d4-150">resource</span></span> | <span data-ttu-id="1e2d4-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e2d4-151">string</span></span> | <span data-ttu-id="1e2d4-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-152">Required.</span></span> <span data-ttu-id="1e2d4-153">Especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-153">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="1e2d4-154">Não incluir a URL base (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="1e2d4-154">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> <span data-ttu-id="1e2d4-155">Consulte os possíveis valores do [caminho](webhooks.md) do recurso de cada recurso suportado.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-155">See the possible resource path [values](webhooks.md) for each supported resource.</span></span>|
| <span data-ttu-id="1e2d4-156">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1e2d4-156">expirationDateTime</span></span> | [<span data-ttu-id="1e2d4-157">dateTime</span><span class="sxs-lookup"><span data-stu-id="1e2d4-157">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="1e2d4-158">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-158">Required.</span></span> <span data-ttu-id="1e2d4-159">Especifica a data e a hora em que a assinatura do webhook expira.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-159">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="1e2d4-160">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-160">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="1e2d4-161">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-161">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="1e2d4-162">clientState</span><span class="sxs-lookup"><span data-stu-id="1e2d4-162">clientState</span></span> | <span data-ttu-id="1e2d4-163">string</span><span class="sxs-lookup"><span data-stu-id="1e2d4-163">string</span></span> | <span data-ttu-id="1e2d4-164">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-164">Optional.</span></span> <span data-ttu-id="1e2d4-165">Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-165">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="1e2d4-166">O comprimento máximo é de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-166">The maximum length is 128 characters.</span></span> <span data-ttu-id="1e2d4-167">O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-167">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="1e2d4-168">id</span><span class="sxs-lookup"><span data-stu-id="1e2d4-168">id</span></span> | <span data-ttu-id="1e2d4-169">string</span><span class="sxs-lookup"><span data-stu-id="1e2d4-169">string</span></span> | <span data-ttu-id="1e2d4-p109">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="1e2d4-172">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="1e2d4-172">applicationId</span></span> | <span data-ttu-id="1e2d4-173">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e2d4-173">string</span></span> | <span data-ttu-id="1e2d4-174">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-174">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="1e2d4-175">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-175">Read-only.</span></span> |
| <span data-ttu-id="1e2d4-176">creatorId</span><span class="sxs-lookup"><span data-stu-id="1e2d4-176">creatorId</span></span> | <span data-ttu-id="1e2d4-177">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e2d4-177">string</span></span> | <span data-ttu-id="1e2d4-178">Identificador de usuário ou entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-178">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="1e2d4-179">Se o aplicativo usado delegada permissões para criar a assinatura, esse campo contém a id do usuário que entrou no aplicativo chamado em nome dele.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-179">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="1e2d4-180">Se o aplicativo usou permissões do aplicativo, esse campo contém a id da entidade de serviço correspondente ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-180">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="1e2d4-181">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-181">Read-only.</span></span> |
| <span data-ttu-id="1e2d4-182">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="1e2d4-182">latestSupportedTlsVersion</span></span> | <span data-ttu-id="1e2d4-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e2d4-183">String</span></span> | <span data-ttu-id="1e2d4-184">Especifica a versão mais recente do protocolo TLS que o ponto de extremidade, especificado por **notificationUrl**, é compatível.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-184">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="1e2d4-185">Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-185">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="1e2d4-186">Para os assinantes cujo ponto de extremidade de notificação suporta uma versão menor que a versão recomendada atualmente (TLS 1.2), especificar essa propriedade por uma [linha do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) definida, permite o uso temporário da versão preterida do TLS antes de concluir a atualização para o TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-186">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="1e2d4-187">Para esses assinantes, não definir essa propriedade pela linha do tempo resultaria em uma falha nas operações da assinatura.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-187">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="1e2d4-188">Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-188">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="1e2d4-189">Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-189">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="1e2d4-190">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="1e2d4-190">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="1e2d4-191">Resource</span><span class="sxs-lookup"><span data-stu-id="1e2d4-191">Resource</span></span>            | <span data-ttu-id="1e2d4-192">Tempo de expiração máximo</span><span class="sxs-lookup"><span data-stu-id="1e2d4-192">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="1e2d4-193">Usuário, grupo, outros recursos de diretório</span><span class="sxs-lookup"><span data-stu-id="1e2d4-193">User, group, other directory resources</span></span>   | <span data-ttu-id="1e2d4-194">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="1e2d4-194">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1e2d4-195">Correio</span><span class="sxs-lookup"><span data-stu-id="1e2d4-195">Mail</span></span>                | <span data-ttu-id="1e2d4-196">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="1e2d4-196">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1e2d4-197">Calendário</span><span class="sxs-lookup"><span data-stu-id="1e2d4-197">Calendar</span></span>            | <span data-ttu-id="1e2d4-198">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="1e2d4-198">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1e2d4-199">Contatos</span><span class="sxs-lookup"><span data-stu-id="1e2d4-199">Contacts</span></span>            | <span data-ttu-id="1e2d4-200">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="1e2d4-200">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1e2d4-201">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="1e2d4-201">Group conversations</span></span> | <span data-ttu-id="1e2d4-202">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="1e2d4-202">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1e2d4-203">Itens raiz de unidade</span><span class="sxs-lookup"><span data-stu-id="1e2d4-203">Drive root items</span></span>    | <span data-ttu-id="1e2d4-204">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="1e2d4-204">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1e2d4-205">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="1e2d4-205">Security alerts</span></span>     | <span data-ttu-id="1e2d4-206">43200 minutos (em 30 dias )</span><span class="sxs-lookup"><span data-stu-id="1e2d4-206">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="1e2d4-207">**Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-207">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="1e2d4-208">No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-208">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="1e2d4-209">Relações</span><span class="sxs-lookup"><span data-stu-id="1e2d4-209">Relationships</span></span>

<span data-ttu-id="1e2d4-210">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1e2d4-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e2d4-211">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e2d4-211">JSON representation</span></span>

<span data-ttu-id="1e2d4-212">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e2d4-212">Here is a JSON representation of the resource.</span></span>

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
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
