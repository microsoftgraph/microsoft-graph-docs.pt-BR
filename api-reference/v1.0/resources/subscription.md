---
title: tipo de recurso de assinatura
description: 'Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ebd12c5876ae9bb580ac8466eeb88341bb1a0ae4
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774916"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="23057-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="23057-104">subscription resource type</span></span>

<span data-ttu-id="23057-105">Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="23057-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="23057-106">Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:</span><span class="sxs-lookup"><span data-stu-id="23057-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="23057-107">Um [mensagem][], [evento][], ou [contato][] no Outlook</span><span class="sxs-lookup"><span data-stu-id="23057-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="23057-108">Um [conversa][] de um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="23057-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="23057-109">Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="23057-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="23057-110">Um [usuário][] ou [grupo][] no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="23057-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="23057-111">Um [alerta][] da API de Segurança do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="23057-111">An [alert][] from the Microsoft Graph Security API</span></span>

## <a name="methods"></a><span data-ttu-id="23057-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="23057-112">Methods</span></span>

| <span data-ttu-id="23057-113">Método</span><span class="sxs-lookup"><span data-stu-id="23057-113">Method</span></span> | <span data-ttu-id="23057-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="23057-114">Return Type</span></span> | <span data-ttu-id="23057-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="23057-115">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="23057-116">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="23057-116">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="23057-117">subscription</span><span class="sxs-lookup"><span data-stu-id="23057-117">subscription</span></span>](subscription.md) | <span data-ttu-id="23057-118">Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="23057-118">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="23057-119">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="23057-119">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="23057-120">subscription</span><span class="sxs-lookup"><span data-stu-id="23057-120">subscription</span></span>](subscription.md) | <span data-ttu-id="23057-121">Renova uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="23057-121">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="23057-122">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="23057-122">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="23057-123">assinatura</span><span class="sxs-lookup"><span data-stu-id="23057-123">subscription</span></span>](subscription.md) | <span data-ttu-id="23057-124">Lista assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="23057-124">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="23057-125">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="23057-125">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="23057-126">subscription</span><span class="sxs-lookup"><span data-stu-id="23057-126">subscription</span></span>](subscription.md) | <span data-ttu-id="23057-127">Lê as propriedades e as relações do objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="23057-127">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="23057-128">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="23057-128">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="23057-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="23057-129">None</span></span> | <span data-ttu-id="23057-130">Exclui um objeto assinatura.</span><span class="sxs-lookup"><span data-stu-id="23057-130">Deletes a subscription object.</span></span> |

## <a name="properties"></a><span data-ttu-id="23057-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23057-131">Properties</span></span>

| <span data-ttu-id="23057-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23057-132">Property</span></span> | <span data-ttu-id="23057-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="23057-133">Type</span></span> | <span data-ttu-id="23057-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="23057-134">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="23057-135">changeType</span><span class="sxs-lookup"><span data-stu-id="23057-135">changeType</span></span> | <span data-ttu-id="23057-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23057-136">string</span></span> | <span data-ttu-id="23057-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23057-137">Required.</span></span> <span data-ttu-id="23057-138">Indica o tipo de alteração no recurso inscrito que gerará uma notificação.</span><span class="sxs-lookup"><span data-stu-id="23057-138">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="23057-139">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="23057-139">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="23057-140">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="23057-140">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="23057-141">Observação: As notificações do item na raiz da unidade suportam somente `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="23057-141">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="23057-142">Notificações de grupos e usuário suportam `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="23057-142">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="23057-143">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="23057-143">notificationUrl</span></span> | <span data-ttu-id="23057-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23057-144">string</span></span> | <span data-ttu-id="23057-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23057-145">Required.</span></span> <span data-ttu-id="23057-146">A URL do ponto de extremidade que receberá as notificações.</span><span class="sxs-lookup"><span data-stu-id="23057-146">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="23057-147">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="23057-147">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="23057-148">recurso</span><span class="sxs-lookup"><span data-stu-id="23057-148">resource</span></span> | <span data-ttu-id="23057-149">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23057-149">string</span></span> | <span data-ttu-id="23057-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23057-150">Required.</span></span> <span data-ttu-id="23057-151">Especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="23057-151">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="23057-152">Não incluir a URL base (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="23057-152">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="23057-153">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="23057-153">expirationDateTime</span></span> | [<span data-ttu-id="23057-154">dateTime</span><span class="sxs-lookup"><span data-stu-id="23057-154">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="23057-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23057-155">Required.</span></span> <span data-ttu-id="23057-156">Especifica a data e a hora em que a assinatura do webhook expira.</span><span class="sxs-lookup"><span data-stu-id="23057-156">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="23057-157">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="23057-157">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="23057-158">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="23057-158">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="23057-159">clientState</span><span class="sxs-lookup"><span data-stu-id="23057-159">clientState</span></span> | <span data-ttu-id="23057-160">string</span><span class="sxs-lookup"><span data-stu-id="23057-160">string</span></span> | <span data-ttu-id="23057-161">Opcional.</span><span class="sxs-lookup"><span data-stu-id="23057-161">Optional.</span></span> <span data-ttu-id="23057-162">Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação.</span><span class="sxs-lookup"><span data-stu-id="23057-162">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="23057-163">O comprimento máximo é de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="23057-163">The maximum length is 128 characters.</span></span> <span data-ttu-id="23057-164">O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação.</span><span class="sxs-lookup"><span data-stu-id="23057-164">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="23057-165">id</span><span class="sxs-lookup"><span data-stu-id="23057-165">id</span></span> | <span data-ttu-id="23057-166">string</span><span class="sxs-lookup"><span data-stu-id="23057-166">string</span></span> | <span data-ttu-id="23057-p109">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23057-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="23057-169">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="23057-169">applicationId</span></span> | <span data-ttu-id="23057-170">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23057-170">string</span></span> | <span data-ttu-id="23057-171">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="23057-171">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="23057-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23057-172">Read-only.</span></span> |
| <span data-ttu-id="23057-173">creatorId</span><span class="sxs-lookup"><span data-stu-id="23057-173">creatorId</span></span> | <span data-ttu-id="23057-174">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23057-174">string</span></span> | <span data-ttu-id="23057-175">Identificador de usuário ou entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="23057-175">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="23057-176">Se o aplicativo usado delegada permissões para criar a assinatura, esse campo contém a id do usuário que entrou no aplicativo chamado em nome dele.</span><span class="sxs-lookup"><span data-stu-id="23057-176">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="23057-177">Se o aplicativo usou permissões do aplicativo, esse campo contém a id da entidade de serviço correspondente ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="23057-177">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="23057-178">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="23057-178">Read-only.</span></span> |
| <span data-ttu-id="23057-179">latestSupportedTlsVersion</span><span class="sxs-lookup"><span data-stu-id="23057-179">latestSupportedTlsVersion</span></span> | <span data-ttu-id="23057-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23057-180">String</span></span> | <span data-ttu-id="23057-181">Especifica a versão mais recente do TLS que o ponto de extremidade de notificação tem suporte.</span><span class="sxs-lookup"><span data-stu-id="23057-181">Specifies the latest TLS version that the notification endpoint supports.</span></span> <span data-ttu-id="23057-182">Permite que os assinantes usem uma versão preterida do TLS por um período limitado.</span><span class="sxs-lookup"><span data-stu-id="23057-182">Allows subscribers to use a deprecated version of TLS for a limited period.</span></span> <span data-ttu-id="23057-183">Valores possíveis: **v1_0**, **v1_1**, **v1_2**, **v1_3**.</span><span class="sxs-lookup"><span data-stu-id="23057-183">Possible values: **v1_0**, **v1_1**, **v1_2**, **v1_3**.</span></span> <span data-ttu-id="23057-184">Opcional, o padrão é v1_2.</span><span class="sxs-lookup"><span data-stu-id="23057-184">Optional, defaults to v1_2.</span></span> <span data-ttu-id="23057-185">Se o ponto de extremidade do cliente oferecer suporte para o TLS 1.2 ou superior, essa propriedade não será necessária.</span><span class="sxs-lookup"><span data-stu-id="23057-185">If the client endpoint supports TLS 1.2 or above this property is not needed.</span></span> <span data-ttu-id="23057-186">Se o ponto de extremidade do cliente oferecer suporte apenas para o TLS 1.0 ou 1.1, essa propriedade deverá ser definida como a versão correspondente ou a operação falhará.</span><span class="sxs-lookup"><span data-stu-id="23057-186">If the client endpoint supports only TLS 1.0 or 1.1, this property should be set to the corresponding version or the operation will fail.</span></span> |

### <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="23057-187">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="23057-187">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="23057-188">Resource</span><span class="sxs-lookup"><span data-stu-id="23057-188">Resource</span></span>            | <span data-ttu-id="23057-189">Tempo de expiração máximo</span><span class="sxs-lookup"><span data-stu-id="23057-189">Maximum expiration time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="23057-190">Usuário, grupo, outros recursos de diretório</span><span class="sxs-lookup"><span data-stu-id="23057-190">User, group, other directory resources</span></span>   | <span data-ttu-id="23057-191">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="23057-191">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="23057-192">Correio</span><span class="sxs-lookup"><span data-stu-id="23057-192">Mail</span></span>                | <span data-ttu-id="23057-193">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="23057-193">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="23057-194">Calendário</span><span class="sxs-lookup"><span data-stu-id="23057-194">Calendar</span></span>            | <span data-ttu-id="23057-195">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="23057-195">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="23057-196">Contatos</span><span class="sxs-lookup"><span data-stu-id="23057-196">Contacts</span></span>            | <span data-ttu-id="23057-197">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="23057-197">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="23057-198">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="23057-198">Group conversations</span></span> | <span data-ttu-id="23057-199">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="23057-199">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="23057-200">Itens raiz de unidade</span><span class="sxs-lookup"><span data-stu-id="23057-200">Drive root items</span></span>    | <span data-ttu-id="23057-201">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="23057-201">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="23057-202">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="23057-202">Security alerts</span></span>     | <span data-ttu-id="23057-203">43200 minutos (em 30 dias )</span><span class="sxs-lookup"><span data-stu-id="23057-203">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="23057-204">**Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado.</span><span class="sxs-lookup"><span data-stu-id="23057-204">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="23057-205">No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.</span><span class="sxs-lookup"><span data-stu-id="23057-205">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="23057-206">Relações</span><span class="sxs-lookup"><span data-stu-id="23057-206">Relationships</span></span>

<span data-ttu-id="23057-207">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23057-207">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23057-208">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23057-208">JSON representation</span></span>

<span data-ttu-id="23057-209">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23057-209">Here is a JSON representation of the resource.</span></span>

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
