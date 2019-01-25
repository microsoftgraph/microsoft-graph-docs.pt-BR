---
title: Tipo de Recurso de Assinatura
description: 'Uma assinatura permite que um aplicativo cliente receber notificações sobre as alterações de dados no Microsoft Graph. Atualmente, as assinaturas são habilitadas para os seguintes recursos:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 265ea807330f833edf0d7b1f6a640e0a1f6f4634
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517264"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="ebb7e-104">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="ebb7e-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebb7e-105">Uma assinatura permite que um aplicativo cliente receber notificações sobre as alterações de dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="ebb7e-106">Atualmente, as assinaturas são habilitadas para os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="ebb7e-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="ebb7e-107">Email, eventos e contatos do Outlook</span><span class="sxs-lookup"><span data-stu-id="ebb7e-107">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="ebb7e-108">Conversas de Grupos do Office.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-108">Conversations from Office Groups.</span></span>
- <span data-ttu-id="ebb7e-109">Itens raiz de unidade no OneDrive</span><span class="sxs-lookup"><span data-stu-id="ebb7e-109">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="ebb7e-110">Usuários e grupos do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-110">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="ebb7e-111">Alertas do API de segurança do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-111">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebb7e-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ebb7e-112">JSON representation</span></span>

<span data-ttu-id="ebb7e-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-113">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="ebb7e-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ebb7e-114">Properties</span></span>

| <span data-ttu-id="ebb7e-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebb7e-115">Property</span></span> | <span data-ttu-id="ebb7e-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebb7e-116">Type</span></span> | <span data-ttu-id="ebb7e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebb7e-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="ebb7e-118">changeType</span><span class="sxs-lookup"><span data-stu-id="ebb7e-118">changeType</span></span> | <span data-ttu-id="ebb7e-119">string</span><span class="sxs-lookup"><span data-stu-id="ebb7e-119">string</span></span> | <span data-ttu-id="ebb7e-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-120">Required.</span></span> <span data-ttu-id="ebb7e-121">Indica o tipo de alteração no recurso inscrito que gerará uma notificação.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="ebb7e-122">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="ebb7e-123">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-123">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="ebb7e-124">Observação: Notificações de item de raiz de unidade suportam somente a `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="ebb7e-125">Suportam a notificações de usuário e grupo `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-125">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="ebb7e-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="ebb7e-126">notificationUrl</span></span> | <span data-ttu-id="ebb7e-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebb7e-127">string</span></span> | <span data-ttu-id="ebb7e-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-128">Required.</span></span> <span data-ttu-id="ebb7e-129">A URL do ponto de extremidade que receberá as notificações.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="ebb7e-130">Essa URL deve tornar a usar o HTTPS protocolo.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="ebb7e-131">recurso</span><span class="sxs-lookup"><span data-stu-id="ebb7e-131">resource</span></span> | <span data-ttu-id="ebb7e-132">string</span><span class="sxs-lookup"><span data-stu-id="ebb7e-132">string</span></span> | <span data-ttu-id="ebb7e-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-133">Required.</span></span> <span data-ttu-id="ebb7e-134">Especifica o recurso que será monitorado para que as alterações.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="ebb7e-135">Não incluir a URL base (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="ebb7e-135">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="ebb7e-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ebb7e-136">expirationDateTime</span></span> | <span data-ttu-id="ebb7e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebb7e-137">DateTimeOffset</span></span> | <span data-ttu-id="ebb7e-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-138">Required.</span></span> <span data-ttu-id="ebb7e-139">Especifica a data e a hora em que a assinatura de webhook expira.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="ebb7e-140">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="ebb7e-141">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="ebb7e-142">clientState</span><span class="sxs-lookup"><span data-stu-id="ebb7e-142">clientState</span></span> | <span data-ttu-id="ebb7e-143">string</span><span class="sxs-lookup"><span data-stu-id="ebb7e-143">string</span></span> | <span data-ttu-id="ebb7e-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-144">Optional.</span></span> <span data-ttu-id="ebb7e-145">Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="ebb7e-146">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-146">The maximum length is 255 characters.</span></span> <span data-ttu-id="ebb7e-147">O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="ebb7e-148">id</span><span class="sxs-lookup"><span data-stu-id="ebb7e-148">id</span></span> | <span data-ttu-id="ebb7e-149">string</span><span class="sxs-lookup"><span data-stu-id="ebb7e-149">string</span></span> | <span data-ttu-id="ebb7e-p109">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="ebb7e-152">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="ebb7e-152">applicationId</span></span> | <span data-ttu-id="ebb7e-153">string</span><span class="sxs-lookup"><span data-stu-id="ebb7e-153">string</span></span> | <span data-ttu-id="ebb7e-154">Identificador do aplicativo usado para criar a inscrição.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="ebb7e-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-155">Read-only.</span></span> |
| <span data-ttu-id="ebb7e-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="ebb7e-156">creatorId</span></span> | <span data-ttu-id="ebb7e-157">string</span><span class="sxs-lookup"><span data-stu-id="ebb7e-157">string</span></span> | <span data-ttu-id="ebb7e-158">Identificador do usuário ou da entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="ebb7e-159">Se o aplicativo usado delegadas permissões para criar a assinatura, esse campo contém a id do usuário entrou no de que aplicativo chamado em nome.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="ebb7e-160">Se o aplicativo usado permissões de aplicativo, esse campo contém a id da entidade de serviço correspondente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="ebb7e-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="ebb7e-162">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="ebb7e-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="ebb7e-163">Recurso</span><span class="sxs-lookup"><span data-stu-id="ebb7e-163">Resource</span></span>            | <span data-ttu-id="ebb7e-164">Tempo de Expiração Máximo</span><span class="sxs-lookup"><span data-stu-id="ebb7e-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="ebb7e-165">Email</span><span class="sxs-lookup"><span data-stu-id="ebb7e-165">Mail</span></span>                | <span data-ttu-id="ebb7e-166">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="ebb7e-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="ebb7e-167">Calendário</span><span class="sxs-lookup"><span data-stu-id="ebb7e-167">Calendar</span></span>            | <span data-ttu-id="ebb7e-168">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="ebb7e-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="ebb7e-169">Contatos</span><span class="sxs-lookup"><span data-stu-id="ebb7e-169">Contacts</span></span>            | <span data-ttu-id="ebb7e-170">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="ebb7e-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="ebb7e-171">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="ebb7e-171">Group conversations</span></span> | <span data-ttu-id="ebb7e-172">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="ebb7e-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="ebb7e-173">Itens raiz de unidade</span><span class="sxs-lookup"><span data-stu-id="ebb7e-173">Drive root items</span></span>    | <span data-ttu-id="ebb7e-174">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="ebb7e-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="ebb7e-175">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="ebb7e-175">Security alerts</span></span>     | <span data-ttu-id="ebb7e-176">43200 minutos (em 30 dias)</span><span class="sxs-lookup"><span data-stu-id="ebb7e-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="ebb7e-177">**Observação:** Aplicativos existentes e novos não deve exceder o valor com suporte.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-177">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="ebb7e-178">No futuro, quaisquer solicitações para criar ou renovar uma assinatura além o valor máximo falhará.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="ebb7e-179">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="ebb7e-179">Relationships</span></span>

<span data-ttu-id="ebb7e-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ebb7e-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="ebb7e-181">Métodos</span><span class="sxs-lookup"><span data-stu-id="ebb7e-181">Methods</span></span>

| <span data-ttu-id="ebb7e-182">Método</span><span class="sxs-lookup"><span data-stu-id="ebb7e-182">Method</span></span> | <span data-ttu-id="ebb7e-183">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ebb7e-183">Return Type</span></span> | <span data-ttu-id="ebb7e-184">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebb7e-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="ebb7e-185">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="ebb7e-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="ebb7e-186">subscription</span><span class="sxs-lookup"><span data-stu-id="ebb7e-186">subscription</span></span>](subscription.md) | <span data-ttu-id="ebb7e-187">Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="ebb7e-188">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="ebb7e-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="ebb7e-189">subscription</span><span class="sxs-lookup"><span data-stu-id="ebb7e-189">subscription</span></span>](subscription.md) | <span data-ttu-id="ebb7e-190">Renove uma assinatura atualizando seu horário de expiração.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-190">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="ebb7e-191">Inscrições de lista</span><span class="sxs-lookup"><span data-stu-id="ebb7e-191">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="ebb7e-192">subscription</span><span class="sxs-lookup"><span data-stu-id="ebb7e-192">subscription</span></span>](subscription.md) | <span data-ttu-id="ebb7e-193">Lista inscrições ativas.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="ebb7e-194">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="ebb7e-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="ebb7e-195">subscription</span><span class="sxs-lookup"><span data-stu-id="ebb7e-195">subscription</span></span>](subscription.md) | <span data-ttu-id="ebb7e-196">Leia as propriedades e os relacionamentos de objeto de inscrição.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-196">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="ebb7e-197">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="ebb7e-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="ebb7e-198">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ebb7e-198">None</span></span> | <span data-ttu-id="ebb7e-199">Exclua um objeto de inscrição.</span><span class="sxs-lookup"><span data-stu-id="ebb7e-199">Delete a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/subscription.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
