---
title: tipo de recurso de assinatura
description: 'Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cda3163cd7538c418338e5d2c6d1ab0a076b33ff
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159133"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="93cb8-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="93cb8-104">subscription resource type</span></span>

<span data-ttu-id="93cb8-105">Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="93cb8-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="93cb8-106">Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:</span><span class="sxs-lookup"><span data-stu-id="93cb8-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="93cb8-107">Um [mensagem][], [evento][], ou [contato][] no Outlook</span><span class="sxs-lookup"><span data-stu-id="93cb8-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="93cb8-108">Um [conversa][] de um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="93cb8-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="93cb8-109">Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="93cb8-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="93cb8-110">Um [usuário][] ou [grupo][] no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="93cb8-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="93cb8-111">Um [alerta][] da API de Segurança do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="93cb8-111">An [alert][] from the Microsoft Graph Security API</span></span>

<span data-ttu-id="93cb8-112">As expressões da trajetória do recurso com suporte para cada recurso - que podem ser usadas na propriedade do**recurso** da assinatura - estão documentadas no [artigo da visão geral](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="93cb8-112">The resource path expressions supported for each resource - that can be used in the **resource** property of the subscription - are documented in [the overview article](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="93cb8-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="93cb8-113">Methods</span></span>

| <span data-ttu-id="93cb8-114">Método</span><span class="sxs-lookup"><span data-stu-id="93cb8-114">Method</span></span> | <span data-ttu-id="93cb8-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="93cb8-115">Return Type</span></span> | <span data-ttu-id="93cb8-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="93cb8-116">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="93cb8-117">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="93cb8-117">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="93cb8-118">subscription</span><span class="sxs-lookup"><span data-stu-id="93cb8-118">subscription</span></span>](subscription.md) | <span data-ttu-id="93cb8-119">Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="93cb8-119">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="93cb8-120">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="93cb8-120">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="93cb8-121">subscription</span><span class="sxs-lookup"><span data-stu-id="93cb8-121">subscription</span></span>](subscription.md) | <span data-ttu-id="93cb8-122">Renova uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="93cb8-122">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="93cb8-123">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="93cb8-123">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="93cb8-124">assinatura</span><span class="sxs-lookup"><span data-stu-id="93cb8-124">subscription</span></span>](subscription.md) | <span data-ttu-id="93cb8-125">Lista assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="93cb8-125">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="93cb8-126">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="93cb8-126">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="93cb8-127">subscription</span><span class="sxs-lookup"><span data-stu-id="93cb8-127">subscription</span></span>](subscription.md) | <span data-ttu-id="93cb8-128">Lê as propriedades e as relações do objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="93cb8-128">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="93cb8-129">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="93cb8-129">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="93cb8-130">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="93cb8-130">None</span></span> | <span data-ttu-id="93cb8-131">Exclui um objeto assinatura.</span><span class="sxs-lookup"><span data-stu-id="93cb8-131">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="93cb8-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93cb8-132">Properties</span></span>

| <span data-ttu-id="93cb8-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93cb8-133">Property</span></span> | <span data-ttu-id="93cb8-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="93cb8-134">Type</span></span> | <span data-ttu-id="93cb8-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="93cb8-135">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="93cb8-136">changeType</span><span class="sxs-lookup"><span data-stu-id="93cb8-136">changeType</span></span> | <span data-ttu-id="93cb8-137">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93cb8-137">string</span></span> | <span data-ttu-id="93cb8-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93cb8-138">Required.</span></span> <span data-ttu-id="93cb8-139">Indica o tipo de alteração no recurso inscrito que gerará uma notificação.</span><span class="sxs-lookup"><span data-stu-id="93cb8-139">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="93cb8-140">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="93cb8-140">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="93cb8-141">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="93cb8-141">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="93cb8-142">Observação: As notificações do item na raiz da unidade suportam somente `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="93cb8-142">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="93cb8-143">Notificações de grupos e usuário suportam `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="93cb8-143">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="93cb8-144">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="93cb8-144">notificationUrl</span></span> | <span data-ttu-id="93cb8-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93cb8-145">string</span></span> | <span data-ttu-id="93cb8-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93cb8-146">Required.</span></span> <span data-ttu-id="93cb8-147">A URL do ponto de extremidade que receberá as notificações.</span><span class="sxs-lookup"><span data-stu-id="93cb8-147">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="93cb8-148">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="93cb8-148">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="93cb8-149">recurso</span><span class="sxs-lookup"><span data-stu-id="93cb8-149">resource</span></span> | <span data-ttu-id="93cb8-150">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93cb8-150">string</span></span> | <span data-ttu-id="93cb8-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93cb8-151">Required.</span></span> <span data-ttu-id="93cb8-152">Especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="93cb8-152">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="93cb8-153">Não incluir a URL base (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="93cb8-153">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="93cb8-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="93cb8-154">expirationDateTime</span></span> | [<span data-ttu-id="93cb8-155">dateTime</span><span class="sxs-lookup"><span data-stu-id="93cb8-155">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="93cb8-156">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93cb8-156">Required.</span></span> <span data-ttu-id="93cb8-157">Especifica a data e a hora em que a assinatura do webhook expira.</span><span class="sxs-lookup"><span data-stu-id="93cb8-157">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="93cb8-158">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="93cb8-158">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="93cb8-159">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="93cb8-159">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="93cb8-160">clientState</span><span class="sxs-lookup"><span data-stu-id="93cb8-160">clientState</span></span> | <span data-ttu-id="93cb8-161">string</span><span class="sxs-lookup"><span data-stu-id="93cb8-161">string</span></span> | <span data-ttu-id="93cb8-162">Opcional.</span><span class="sxs-lookup"><span data-stu-id="93cb8-162">Optional.</span></span> <span data-ttu-id="93cb8-163">Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação.</span><span class="sxs-lookup"><span data-stu-id="93cb8-163">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="93cb8-164">O comprimento máximo é de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="93cb8-164">The maximum length is 128 characters.</span></span> <span data-ttu-id="93cb8-165">O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação.</span><span class="sxs-lookup"><span data-stu-id="93cb8-165">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="93cb8-166">id</span><span class="sxs-lookup"><span data-stu-id="93cb8-166">id</span></span> | <span data-ttu-id="93cb8-167">string</span><span class="sxs-lookup"><span data-stu-id="93cb8-167">string</span></span> | <span data-ttu-id="93cb8-p109">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93cb8-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="93cb8-170">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="93cb8-170">applicationId</span></span> | <span data-ttu-id="93cb8-171">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93cb8-171">string</span></span> | <span data-ttu-id="93cb8-172">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="93cb8-172">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="93cb8-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93cb8-173">Read-only.</span></span> |
| <span data-ttu-id="93cb8-174">creatorId</span><span class="sxs-lookup"><span data-stu-id="93cb8-174">creatorId</span></span> | <span data-ttu-id="93cb8-175">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93cb8-175">string</span></span> | <span data-ttu-id="93cb8-176">Identificador de usuário ou entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="93cb8-176">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="93cb8-177">Se o aplicativo usado delegada permissões para criar a assinatura, esse campo contém a id do usuário que entrou no aplicativo chamado em nome dele.</span><span class="sxs-lookup"><span data-stu-id="93cb8-177">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="93cb8-178">Se o aplicativo usou permissões do aplicativo, esse campo contém a id da entidade de serviço correspondente ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="93cb8-178">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="93cb8-179">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="93cb8-179">Read-only.</span></span> |
| <span data-ttu-id="93cb8-180">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="93cb8-180">latestSupportedTlsVersion</span></span> | <span data-ttu-id="93cb8-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93cb8-181">String</span></span> | <span data-ttu-id="93cb8-182">Especifica a versão mais recente do protocolo TLS que o ponto de extremidade, especificado por **notificationUrl**, é compatível.</span><span class="sxs-lookup"><span data-stu-id="93cb8-182">Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by **notificationUrl**, supports.</span></span> <span data-ttu-id="93cb8-183">Os valores possíveis são: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span><span class="sxs-lookup"><span data-stu-id="93cb8-183">The possible values are: `v1_0`, `v1_1`, `v1_2`, `v1_3`.</span></span> </br></br><span data-ttu-id="93cb8-184">Para os assinantes cujo ponto de extremidade de notificação suporta uma versão menor que a versão recomendada atualmente (TLS 1.2), especificar essa propriedade por uma [linha do tempo](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) definida, permite o uso temporário da versão preterida do TLS antes de concluir a atualização para o TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="93cb8-184">For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set [timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.</span></span> <span data-ttu-id="93cb8-185">Para esses assinantes, não definir essa propriedade pela linha do tempo resultaria em uma falha nas operações da assinatura.</span><span class="sxs-lookup"><span data-stu-id="93cb8-185">For these subscribers, not setting this property per the timeline would result in subscription operations failing.</span></span> </br></br><span data-ttu-id="93cb8-186">Para os assinantes cujo ponto de extremidade já tem suporte ao TLS 1.2, a configuração dessa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="93cb8-186">For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.</span></span> <span data-ttu-id="93cb8-187">Nesses casos, o Microsoft Graph padroniza a propriedade como `v1_2`.</span><span class="sxs-lookup"><span data-stu-id="93cb8-187">In such cases, Microsoft Graph defaults the property to `v1_2`.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="93cb8-188">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="93cb8-188">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="93cb8-189">Resource</span><span class="sxs-lookup"><span data-stu-id="93cb8-189">Resource</span></span>            | <span data-ttu-id="93cb8-190">Tempo de expiração máximo</span><span class="sxs-lookup"><span data-stu-id="93cb8-190">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="93cb8-191">Usuário, grupo, outros recursos de diretório</span><span class="sxs-lookup"><span data-stu-id="93cb8-191">User, group, other directory resources</span></span>   | <span data-ttu-id="93cb8-192">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="93cb8-192">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="93cb8-193">Correio</span><span class="sxs-lookup"><span data-stu-id="93cb8-193">Mail</span></span>                | <span data-ttu-id="93cb8-194">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="93cb8-194">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="93cb8-195">Calendário</span><span class="sxs-lookup"><span data-stu-id="93cb8-195">Calendar</span></span>            | <span data-ttu-id="93cb8-196">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="93cb8-196">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="93cb8-197">Contatos</span><span class="sxs-lookup"><span data-stu-id="93cb8-197">Contacts</span></span>            | <span data-ttu-id="93cb8-198">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="93cb8-198">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="93cb8-199">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="93cb8-199">Group conversations</span></span> | <span data-ttu-id="93cb8-200">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="93cb8-200">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="93cb8-201">Itens raiz de unidade</span><span class="sxs-lookup"><span data-stu-id="93cb8-201">Drive root items</span></span>    | <span data-ttu-id="93cb8-202">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="93cb8-202">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="93cb8-203">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="93cb8-203">Security alerts</span></span>     | <span data-ttu-id="93cb8-204">43200 minutos (em 30 dias )</span><span class="sxs-lookup"><span data-stu-id="93cb8-204">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="93cb8-205">**Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado.</span><span class="sxs-lookup"><span data-stu-id="93cb8-205">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="93cb8-206">No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.</span><span class="sxs-lookup"><span data-stu-id="93cb8-206">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="93cb8-207">Relações</span><span class="sxs-lookup"><span data-stu-id="93cb8-207">Relationships</span></span>

<span data-ttu-id="93cb8-208">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93cb8-208">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93cb8-209">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93cb8-209">JSON representation</span></span>

<span data-ttu-id="93cb8-210">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93cb8-210">Here is a JSON representation of the resource.</span></span>

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
