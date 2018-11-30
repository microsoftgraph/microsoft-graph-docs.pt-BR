---
title: tipo de recurso de assinatura
description: 'Uma assinatura permite que um aplicativo cliente receber notificações sobre as alterações de dados no Microsoft Graph. Atualmente, as assinaturas são habilitadas para os seguintes recursos:'
ms.openlocfilehash: 5ece39954d661c6b7ef948d0ed7d514782fbceae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007257"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="8e69a-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="8e69a-104">subscription resource type</span></span>

<span data-ttu-id="8e69a-105">Uma assinatura permite que um aplicativo cliente receber notificações sobre as alterações de dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8e69a-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="8e69a-106">Atualmente, as assinaturas são habilitadas para os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="8e69a-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="8e69a-107">Email, eventos e contatos do Outlook.</span><span class="sxs-lookup"><span data-stu-id="8e69a-107">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="8e69a-108">Conversas de Grupos do Office.</span><span class="sxs-lookup"><span data-stu-id="8e69a-108">Conversations from Office Groups.</span></span>
- <span data-ttu-id="8e69a-109">Itens raiz da unidade do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8e69a-109">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="8e69a-110">Usuários e grupos do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8e69a-110">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="8e69a-111">Alertas do API de segurança do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8e69a-111">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e69a-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e69a-112">JSON representation</span></span>

<span data-ttu-id="8e69a-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e69a-113">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8e69a-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e69a-114">Properties</span></span>

| <span data-ttu-id="8e69a-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e69a-115">Property</span></span> | <span data-ttu-id="8e69a-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e69a-116">Type</span></span> | <span data-ttu-id="8e69a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e69a-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="8e69a-118">changeType</span><span class="sxs-lookup"><span data-stu-id="8e69a-118">changeType</span></span> | <span data-ttu-id="8e69a-119">string</span><span class="sxs-lookup"><span data-stu-id="8e69a-119">string</span></span> | <span data-ttu-id="8e69a-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e69a-120">Required.</span></span> <span data-ttu-id="8e69a-121">Indica o tipo de alteração no recurso inscrito que gerará uma notificação.</span><span class="sxs-lookup"><span data-stu-id="8e69a-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="8e69a-122">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="8e69a-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="8e69a-123">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="8e69a-123">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="8e69a-124">Observação: Notificações de item de raiz de unidade suportam somente a `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="8e69a-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="8e69a-125">Suportam a notificações de usuário e grupo `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="8e69a-125">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="8e69a-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="8e69a-126">notificationUrl</span></span> | <span data-ttu-id="8e69a-127">string</span><span class="sxs-lookup"><span data-stu-id="8e69a-127">string</span></span> | <span data-ttu-id="8e69a-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e69a-128">Required.</span></span> <span data-ttu-id="8e69a-129">A URL do ponto de extremidade que receberá as notificações.</span><span class="sxs-lookup"><span data-stu-id="8e69a-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="8e69a-130">Essa URL deve tornar a usar o HTTPS protocolo.</span><span class="sxs-lookup"><span data-stu-id="8e69a-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="8e69a-131">recurso</span><span class="sxs-lookup"><span data-stu-id="8e69a-131">resource</span></span> | <span data-ttu-id="8e69a-132">string</span><span class="sxs-lookup"><span data-stu-id="8e69a-132">string</span></span> | <span data-ttu-id="8e69a-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e69a-133">Required.</span></span> <span data-ttu-id="8e69a-134">Especifica o recurso que será monitorado para que as alterações.</span><span class="sxs-lookup"><span data-stu-id="8e69a-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="8e69a-135">Não incluir a URL base (`https://graph.microsoft.com/v1.0/`).</span><span class="sxs-lookup"><span data-stu-id="8e69a-135">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="8e69a-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8e69a-136">expirationDateTime</span></span> | [<span data-ttu-id="8e69a-137">dateTime</span><span class="sxs-lookup"><span data-stu-id="8e69a-137">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="8e69a-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e69a-138">Required.</span></span> <span data-ttu-id="8e69a-139">Especifica a data e a hora em que a assinatura de webhook expira.</span><span class="sxs-lookup"><span data-stu-id="8e69a-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="8e69a-140">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="8e69a-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="8e69a-141">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="8e69a-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="8e69a-142">clientState</span><span class="sxs-lookup"><span data-stu-id="8e69a-142">clientState</span></span> | <span data-ttu-id="8e69a-143">string</span><span class="sxs-lookup"><span data-stu-id="8e69a-143">string</span></span> | <span data-ttu-id="8e69a-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8e69a-144">Optional.</span></span> <span data-ttu-id="8e69a-145">Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação.</span><span class="sxs-lookup"><span data-stu-id="8e69a-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="8e69a-146">O comprimento máximo é de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="8e69a-146">The maximum length is 128 characters.</span></span> <span data-ttu-id="8e69a-147">O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação.</span><span class="sxs-lookup"><span data-stu-id="8e69a-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="8e69a-148">id</span><span class="sxs-lookup"><span data-stu-id="8e69a-148">id</span></span> | <span data-ttu-id="8e69a-149">string</span><span class="sxs-lookup"><span data-stu-id="8e69a-149">string</span></span> | <span data-ttu-id="8e69a-p109">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e69a-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="8e69a-152">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="8e69a-152">applicationId</span></span> | <span data-ttu-id="8e69a-153">string</span><span class="sxs-lookup"><span data-stu-id="8e69a-153">string</span></span> | <span data-ttu-id="8e69a-154">Identificador do aplicativo usado para criar a inscrição.</span><span class="sxs-lookup"><span data-stu-id="8e69a-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="8e69a-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e69a-155">Read-only.</span></span> |
| <span data-ttu-id="8e69a-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="8e69a-156">creatorId</span></span> | <span data-ttu-id="8e69a-157">string</span><span class="sxs-lookup"><span data-stu-id="8e69a-157">string</span></span> | <span data-ttu-id="8e69a-158">Identificador do usuário ou da entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="8e69a-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="8e69a-159">Se o aplicativo usado delegadas permissões para criar a assinatura, esse campo contém a id do usuário entrou no de que aplicativo chamado em nome.</span><span class="sxs-lookup"><span data-stu-id="8e69a-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="8e69a-160">Se o aplicativo usado permissões de aplicativo, esse campo contém a id da entidade de serviço correspondente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e69a-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="8e69a-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e69a-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="8e69a-162">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="8e69a-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="8e69a-163">Recurso</span><span class="sxs-lookup"><span data-stu-id="8e69a-163">Resource</span></span>            | <span data-ttu-id="8e69a-164">Tempo de Expiração Máximo</span><span class="sxs-lookup"><span data-stu-id="8e69a-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="8e69a-165">Email</span><span class="sxs-lookup"><span data-stu-id="8e69a-165">Mail</span></span>                | <span data-ttu-id="8e69a-166">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="8e69a-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8e69a-167">Calendário</span><span class="sxs-lookup"><span data-stu-id="8e69a-167">Calendar</span></span>            | <span data-ttu-id="8e69a-168">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="8e69a-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8e69a-169">Contatos</span><span class="sxs-lookup"><span data-stu-id="8e69a-169">Contacts</span></span>            | <span data-ttu-id="8e69a-170">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="8e69a-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8e69a-171">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="8e69a-171">Group conversations</span></span> | <span data-ttu-id="8e69a-172">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="8e69a-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8e69a-173">Itens raiz de unidade</span><span class="sxs-lookup"><span data-stu-id="8e69a-173">Drive root items</span></span>    | <span data-ttu-id="8e69a-174">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="8e69a-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8e69a-175">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="8e69a-175">Security alerts</span></span>     | <span data-ttu-id="8e69a-176">43200 minutos (em 30 dias)</span><span class="sxs-lookup"><span data-stu-id="8e69a-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="8e69a-177">**Observação:** Aplicativos existentes e novos não deve exceder o valor com suporte.</span><span class="sxs-lookup"><span data-stu-id="8e69a-177">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="8e69a-178">No futuro, quaisquer solicitações para criar ou renovar uma assinatura além o valor máximo falhará.</span><span class="sxs-lookup"><span data-stu-id="8e69a-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="8e69a-179">Relações</span><span class="sxs-lookup"><span data-stu-id="8e69a-179">Relationships</span></span>

<span data-ttu-id="8e69a-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e69a-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="8e69a-181">Métodos</span><span class="sxs-lookup"><span data-stu-id="8e69a-181">Methods</span></span>

| <span data-ttu-id="8e69a-182">Método</span><span class="sxs-lookup"><span data-stu-id="8e69a-182">Method</span></span> | <span data-ttu-id="8e69a-183">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8e69a-183">Return Type</span></span> | <span data-ttu-id="8e69a-184">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e69a-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="8e69a-185">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="8e69a-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="8e69a-186">subscription</span><span class="sxs-lookup"><span data-stu-id="8e69a-186">subscription</span></span>](subscription.md) | <span data-ttu-id="8e69a-187">Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="8e69a-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="8e69a-188">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="8e69a-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="8e69a-189">subscription</span><span class="sxs-lookup"><span data-stu-id="8e69a-189">subscription</span></span>](subscription.md) | <span data-ttu-id="8e69a-190">Renova uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="8e69a-190">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="8e69a-191">Inscrições de lista</span><span class="sxs-lookup"><span data-stu-id="8e69a-191">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="8e69a-192">subscription</span><span class="sxs-lookup"><span data-stu-id="8e69a-192">subscription</span></span>](subscription.md) | <span data-ttu-id="8e69a-193">Lista inscrições ativas.</span><span class="sxs-lookup"><span data-stu-id="8e69a-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="8e69a-194">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="8e69a-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="8e69a-195">subscription</span><span class="sxs-lookup"><span data-stu-id="8e69a-195">subscription</span></span>](subscription.md) | <span data-ttu-id="8e69a-196">Lê as propriedades e as relações do objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="8e69a-196">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="8e69a-197">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="8e69a-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="8e69a-198">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="8e69a-198">None</span></span> |<span data-ttu-id="8e69a-199">Exclui um objeto subscription.</span><span class="sxs-lookup"><span data-stu-id="8e69a-199">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
