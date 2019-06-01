---
title: tipo de recurso de assinatura
description: 'Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 30671dcd93b4593015a5c3cf2eeddac8d7e00c4d
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536771"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="18bb0-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="18bb0-104">subscription resource type</span></span>

<span data-ttu-id="18bb0-105">Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="18bb0-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="18bb0-106">Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:</span><span class="sxs-lookup"><span data-stu-id="18bb0-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="18bb0-107">Um [mensagem][], [evento][], ou [contato][] no Outlook</span><span class="sxs-lookup"><span data-stu-id="18bb0-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="18bb0-108">Um [conversa][] de um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="18bb0-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="18bb0-109">Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="18bb0-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="18bb0-110">Um [usuário][] ou [grupo][] no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="18bb0-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="18bb0-111">Um [alerta][] da API de Segurança do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="18bb0-111">An [alert][] from the Microsoft Graph Security API</span></span>

## <a name="json-representation"></a><span data-ttu-id="18bb0-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18bb0-112">JSON representation</span></span>

<span data-ttu-id="18bb0-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18bb0-113">Here is a JSON representation of the resource.</span></span>

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
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="18bb0-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18bb0-114">Properties</span></span>

| <span data-ttu-id="18bb0-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18bb0-115">Property</span></span> | <span data-ttu-id="18bb0-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="18bb0-116">Type</span></span> | <span data-ttu-id="18bb0-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="18bb0-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="18bb0-118">changeType</span><span class="sxs-lookup"><span data-stu-id="18bb0-118">changeType</span></span> | <span data-ttu-id="18bb0-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18bb0-119">string</span></span> | <span data-ttu-id="18bb0-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18bb0-120">Required.</span></span> <span data-ttu-id="18bb0-121">Indica o tipo de alteração no recurso inscrito que gerará uma notificação.</span><span class="sxs-lookup"><span data-stu-id="18bb0-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="18bb0-122">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="18bb0-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="18bb0-123">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="18bb0-123">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="18bb0-124">Observação: As notificações do item na raiz da unidade suportam somente `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="18bb0-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="18bb0-125">Notificações de grupos e usuário suportam `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="18bb0-125">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="18bb0-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="18bb0-126">notificationUrl</span></span> | <span data-ttu-id="18bb0-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18bb0-127">string</span></span> | <span data-ttu-id="18bb0-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18bb0-128">Required.</span></span> <span data-ttu-id="18bb0-129">A URL do ponto de extremidade que receberá as notificações.</span><span class="sxs-lookup"><span data-stu-id="18bb0-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="18bb0-130">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="18bb0-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="18bb0-131">recurso</span><span class="sxs-lookup"><span data-stu-id="18bb0-131">resource</span></span> | <span data-ttu-id="18bb0-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18bb0-132">string</span></span> | <span data-ttu-id="18bb0-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18bb0-133">Required.</span></span> <span data-ttu-id="18bb0-134">Especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="18bb0-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="18bb0-135">Não incluir a URL base (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="18bb0-135">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="18bb0-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="18bb0-136">expirationDateTime</span></span> | [<span data-ttu-id="18bb0-137">dateTime</span><span class="sxs-lookup"><span data-stu-id="18bb0-137">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="18bb0-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18bb0-138">Required.</span></span> <span data-ttu-id="18bb0-139">Especifica a data e a hora em que a assinatura do webhook expira.</span><span class="sxs-lookup"><span data-stu-id="18bb0-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="18bb0-140">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="18bb0-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="18bb0-141">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="18bb0-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="18bb0-142">clientState</span><span class="sxs-lookup"><span data-stu-id="18bb0-142">clientState</span></span> | <span data-ttu-id="18bb0-143">string</span><span class="sxs-lookup"><span data-stu-id="18bb0-143">string</span></span> | <span data-ttu-id="18bb0-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="18bb0-144">Optional.</span></span> <span data-ttu-id="18bb0-145">Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação.</span><span class="sxs-lookup"><span data-stu-id="18bb0-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="18bb0-146">O comprimento máximo é de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="18bb0-146">The maximum length is 128 characters.</span></span> <span data-ttu-id="18bb0-147">O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação.</span><span class="sxs-lookup"><span data-stu-id="18bb0-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="18bb0-148">id</span><span class="sxs-lookup"><span data-stu-id="18bb0-148">id</span></span> | <span data-ttu-id="18bb0-149">string</span><span class="sxs-lookup"><span data-stu-id="18bb0-149">string</span></span> | <span data-ttu-id="18bb0-p109">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="18bb0-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="18bb0-152">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="18bb0-152">applicationId</span></span> | <span data-ttu-id="18bb0-153">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18bb0-153">string</span></span> | <span data-ttu-id="18bb0-154">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="18bb0-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="18bb0-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="18bb0-155">Read-only.</span></span> |
| <span data-ttu-id="18bb0-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="18bb0-156">creatorId</span></span> | <span data-ttu-id="18bb0-157">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18bb0-157">string</span></span> | <span data-ttu-id="18bb0-158">Identificador de usuário ou entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="18bb0-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="18bb0-159">Se o aplicativo usado delegada permissões para criar a assinatura, esse campo contém a id do usuário que entrou no aplicativo chamado em nome dele.</span><span class="sxs-lookup"><span data-stu-id="18bb0-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="18bb0-160">Se o aplicativo usou permissões do aplicativo, esse campo contém a id da entidade de serviço correspondente ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18bb0-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="18bb0-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="18bb0-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="18bb0-162">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="18bb0-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="18bb0-163">Recurso</span><span class="sxs-lookup"><span data-stu-id="18bb0-163">Resource</span></span>            | <span data-ttu-id="18bb0-164">Tempo de Expiração Máximo</span><span class="sxs-lookup"><span data-stu-id="18bb0-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="18bb0-165">Usuário, grupo, outros recursos de diretório</span><span class="sxs-lookup"><span data-stu-id="18bb0-165">User, group, other directory resources</span></span>   | <span data-ttu-id="18bb0-166">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="18bb0-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="18bb0-167">Correio</span><span class="sxs-lookup"><span data-stu-id="18bb0-167">Mail</span></span>                | <span data-ttu-id="18bb0-168">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="18bb0-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="18bb0-169">Calendário</span><span class="sxs-lookup"><span data-stu-id="18bb0-169">Calendar</span></span>            | <span data-ttu-id="18bb0-170">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="18bb0-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="18bb0-171">Contatos</span><span class="sxs-lookup"><span data-stu-id="18bb0-171">Contacts</span></span>            | <span data-ttu-id="18bb0-172">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="18bb0-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="18bb0-173">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="18bb0-173">Group conversations</span></span> | <span data-ttu-id="18bb0-174">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="18bb0-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="18bb0-175">Itens raiz de unidade</span><span class="sxs-lookup"><span data-stu-id="18bb0-175">Drive root items</span></span>    | <span data-ttu-id="18bb0-176">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="18bb0-176">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="18bb0-177">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="18bb0-177">Security alerts</span></span>     | <span data-ttu-id="18bb0-178">43200 minutos (em 30 dias )</span><span class="sxs-lookup"><span data-stu-id="18bb0-178">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="18bb0-179">**Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado.</span><span class="sxs-lookup"><span data-stu-id="18bb0-179">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="18bb0-180">No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.</span><span class="sxs-lookup"><span data-stu-id="18bb0-180">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="18bb0-181">Relações</span><span class="sxs-lookup"><span data-stu-id="18bb0-181">Relationships</span></span>

<span data-ttu-id="18bb0-182">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="18bb0-182">None</span></span>

## <a name="methods"></a><span data-ttu-id="18bb0-183">Métodos</span><span class="sxs-lookup"><span data-stu-id="18bb0-183">Methods</span></span>

| <span data-ttu-id="18bb0-184">Método</span><span class="sxs-lookup"><span data-stu-id="18bb0-184">Method</span></span> | <span data-ttu-id="18bb0-185">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="18bb0-185">Return Type</span></span> | <span data-ttu-id="18bb0-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="18bb0-186">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="18bb0-187">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="18bb0-187">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="18bb0-188">subscription</span><span class="sxs-lookup"><span data-stu-id="18bb0-188">subscription</span></span>](subscription.md) | <span data-ttu-id="18bb0-189">Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="18bb0-189">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="18bb0-190">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="18bb0-190">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="18bb0-191">subscription</span><span class="sxs-lookup"><span data-stu-id="18bb0-191">subscription</span></span>](subscription.md) | <span data-ttu-id="18bb0-192">Renova uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="18bb0-192">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="18bb0-193">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="18bb0-193">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="18bb0-194">assinatura</span><span class="sxs-lookup"><span data-stu-id="18bb0-194">subscription</span></span>](subscription.md) | <span data-ttu-id="18bb0-195">Lista assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="18bb0-195">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="18bb0-196">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="18bb0-196">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="18bb0-197">subscription</span><span class="sxs-lookup"><span data-stu-id="18bb0-197">subscription</span></span>](subscription.md) | <span data-ttu-id="18bb0-198">Lê as propriedades e as relações do objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="18bb0-198">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="18bb0-199">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="18bb0-199">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="18bb0-200">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="18bb0-200">None</span></span> |<span data-ttu-id="18bb0-201">Exclui um objeto assinatura.</span><span class="sxs-lookup"><span data-stu-id="18bb0-201">Deletes a subscription object.</span></span> |

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
