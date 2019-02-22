---
title: tipo de recurso Subscription
description: 'Uma assinatura permite que um aplicativo cliente receba notificações sobre alterações nos dados no Microsoft Graph. No momento, as assinaturas estão habilitadas para os seguintes recursos:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9de48cc6a3e5dde459673117d9ee00a34477faf6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163935"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="dad27-104">tipo de recurso Subscription</span><span class="sxs-lookup"><span data-stu-id="dad27-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dad27-105">Uma assinatura permite que um aplicativo cliente receba notificações sobre alterações nos dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="dad27-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="dad27-106">No momento, as assinaturas estão habilitadas para os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="dad27-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="dad27-107">Uma [mensagem][], [evento][]ou [contato][] no Outlook</span><span class="sxs-lookup"><span data-stu-id="dad27-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="dad27-108">Uma [conversa][] de um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="dad27-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="dad27-109">Conteúdo na hierarquia de uma pasta raiz [driveItem][] no onedrive for Business ou em uma pasta raiz ou subpasta [driveItem][] no onedrive pessoal de um usuário</span><span class="sxs-lookup"><span data-stu-id="dad27-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="dad27-110">Um [usuário][] ou [grupo][] no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="dad27-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="dad27-111">Um [alerta][] da API de segurança do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="dad27-111">An [alert][] from the Microsoft Graph Security API</span></span>


## <a name="json-representation"></a><span data-ttu-id="dad27-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dad27-112">JSON representation</span></span>

<span data-ttu-id="dad27-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dad27-113">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="dad27-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dad27-114">Properties</span></span>

| <span data-ttu-id="dad27-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dad27-115">Property</span></span> | <span data-ttu-id="dad27-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="dad27-116">Type</span></span> | <span data-ttu-id="dad27-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="dad27-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="dad27-118">changeType</span><span class="sxs-lookup"><span data-stu-id="dad27-118">changeType</span></span> | <span data-ttu-id="dad27-119">string</span><span class="sxs-lookup"><span data-stu-id="dad27-119">string</span></span> | <span data-ttu-id="dad27-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dad27-120">Required.</span></span> <span data-ttu-id="dad27-121">Indica o tipo de alteração no recurso inscrito que gerará uma notificação.</span><span class="sxs-lookup"><span data-stu-id="dad27-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="dad27-122">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="dad27-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="dad27-123">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="dad27-123">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="dad27-124">Observação: as notificações de item raiz da unidade `updated` dão suporte somente a ChangeType.</span><span class="sxs-lookup"><span data-stu-id="dad27-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="dad27-125">Suporte e `deleted` ChangeType para `updated` notificações de grupo e usuário.</span><span class="sxs-lookup"><span data-stu-id="dad27-125">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="dad27-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="dad27-126">notificationUrl</span></span> | <span data-ttu-id="dad27-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dad27-127">string</span></span> | <span data-ttu-id="dad27-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dad27-128">Required.</span></span> <span data-ttu-id="dad27-129">A URL do ponto de extremidade que receberá as notificações.</span><span class="sxs-lookup"><span data-stu-id="dad27-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="dad27-130">Essa URL deve fazer uso do protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="dad27-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="dad27-131">recurso</span><span class="sxs-lookup"><span data-stu-id="dad27-131">resource</span></span> | <span data-ttu-id="dad27-132">string</span><span class="sxs-lookup"><span data-stu-id="dad27-132">string</span></span> | <span data-ttu-id="dad27-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dad27-133">Required.</span></span> <span data-ttu-id="dad27-134">Especifica o recurso que será monitorado para alterações.</span><span class="sxs-lookup"><span data-stu-id="dad27-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="dad27-135">Não inclua a URL base (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="dad27-135">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="dad27-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dad27-136">expirationDateTime</span></span> | <span data-ttu-id="dad27-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dad27-137">DateTimeOffset</span></span> | <span data-ttu-id="dad27-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dad27-138">Required.</span></span> <span data-ttu-id="dad27-139">Especifica a data e a hora em que a assinatura de webhook expira.</span><span class="sxs-lookup"><span data-stu-id="dad27-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="dad27-140">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="dad27-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="dad27-141">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="dad27-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="dad27-142">clientState</span><span class="sxs-lookup"><span data-stu-id="dad27-142">clientState</span></span> | <span data-ttu-id="dad27-143">string</span><span class="sxs-lookup"><span data-stu-id="dad27-143">string</span></span> | <span data-ttu-id="dad27-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dad27-144">Optional.</span></span> <span data-ttu-id="dad27-145">Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação.</span><span class="sxs-lookup"><span data-stu-id="dad27-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="dad27-146">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="dad27-146">The maximum length is 255 characters.</span></span> <span data-ttu-id="dad27-147">O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação.</span><span class="sxs-lookup"><span data-stu-id="dad27-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="dad27-148">id</span><span class="sxs-lookup"><span data-stu-id="dad27-148">id</span></span> | <span data-ttu-id="dad27-149">string</span><span class="sxs-lookup"><span data-stu-id="dad27-149">string</span></span> | <span data-ttu-id="dad27-p109">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dad27-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="dad27-152">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="dad27-152">applicationId</span></span> | <span data-ttu-id="dad27-153">string</span><span class="sxs-lookup"><span data-stu-id="dad27-153">string</span></span> | <span data-ttu-id="dad27-154">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="dad27-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="dad27-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dad27-155">Read-only.</span></span> |
| <span data-ttu-id="dad27-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="dad27-156">creatorId</span></span> | <span data-ttu-id="dad27-157">string</span><span class="sxs-lookup"><span data-stu-id="dad27-157">string</span></span> | <span data-ttu-id="dad27-158">Identificador da entidade de serviço ou usuário que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="dad27-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="dad27-159">Se o aplicativo usou permissões delegadas para criar a assinatura, este campo conterá a ID do usuário conectado o aplicativo chamado em nome de.</span><span class="sxs-lookup"><span data-stu-id="dad27-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="dad27-160">Se o aplicativo usava permissões de aplicativo, este campo contém a ID da entidade de serviço correspondente ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dad27-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="dad27-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dad27-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="dad27-162">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="dad27-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="dad27-163">Recurso</span><span class="sxs-lookup"><span data-stu-id="dad27-163">Resource</span></span>            | <span data-ttu-id="dad27-164">Tempo de Expiração Máximo</span><span class="sxs-lookup"><span data-stu-id="dad27-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="dad27-165">Email</span><span class="sxs-lookup"><span data-stu-id="dad27-165">Mail</span></span>                | <span data-ttu-id="dad27-166">4230 minutos (abaixo de 3 dias)</span><span class="sxs-lookup"><span data-stu-id="dad27-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dad27-167">Calendário</span><span class="sxs-lookup"><span data-stu-id="dad27-167">Calendar</span></span>            | <span data-ttu-id="dad27-168">4230 minutos (abaixo de 3 dias)</span><span class="sxs-lookup"><span data-stu-id="dad27-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dad27-169">Contatos</span><span class="sxs-lookup"><span data-stu-id="dad27-169">Contacts</span></span>            | <span data-ttu-id="dad27-170">4230 minutos (abaixo de 3 dias)</span><span class="sxs-lookup"><span data-stu-id="dad27-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dad27-171">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="dad27-171">Group conversations</span></span> | <span data-ttu-id="dad27-172">4230 minutos (abaixo de 3 dias)</span><span class="sxs-lookup"><span data-stu-id="dad27-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dad27-173">Itens raiz de unidade</span><span class="sxs-lookup"><span data-stu-id="dad27-173">Drive root items</span></span>    | <span data-ttu-id="dad27-174">4230 minutos (abaixo de 3 dias)</span><span class="sxs-lookup"><span data-stu-id="dad27-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="dad27-175">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="dad27-175">Security alerts</span></span>     | <span data-ttu-id="dad27-176">43200 minutos (menos de 30 dias)</span><span class="sxs-lookup"><span data-stu-id="dad27-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="dad27-177">**Observação:** Aplicativos existentes e novos aplicativos não devem exceder o valor com suporte.</span><span class="sxs-lookup"><span data-stu-id="dad27-177">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="dad27-178">No futuro, todas as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.</span><span class="sxs-lookup"><span data-stu-id="dad27-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="dad27-179">Relações</span><span class="sxs-lookup"><span data-stu-id="dad27-179">Relationships</span></span>

<span data-ttu-id="dad27-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dad27-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="dad27-181">Métodos</span><span class="sxs-lookup"><span data-stu-id="dad27-181">Methods</span></span>

| <span data-ttu-id="dad27-182">Método</span><span class="sxs-lookup"><span data-stu-id="dad27-182">Method</span></span> | <span data-ttu-id="dad27-183">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dad27-183">Return Type</span></span> | <span data-ttu-id="dad27-184">Descrição</span><span class="sxs-lookup"><span data-stu-id="dad27-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="dad27-185">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="dad27-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="dad27-186">subscription</span><span class="sxs-lookup"><span data-stu-id="dad27-186">subscription</span></span>](subscription.md) | <span data-ttu-id="dad27-187">Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="dad27-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="dad27-188">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="dad27-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="dad27-189">subscription</span><span class="sxs-lookup"><span data-stu-id="dad27-189">subscription</span></span>](subscription.md) | <span data-ttu-id="dad27-190">ReNovar uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="dad27-190">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="dad27-191">Listar assinaturas</span><span class="sxs-lookup"><span data-stu-id="dad27-191">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="dad27-192">subscription</span><span class="sxs-lookup"><span data-stu-id="dad27-192">subscription</span></span>](subscription.md) | <span data-ttu-id="dad27-193">Lista assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="dad27-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="dad27-194">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="dad27-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="dad27-195">subscription</span><span class="sxs-lookup"><span data-stu-id="dad27-195">subscription</span></span>](subscription.md) | <span data-ttu-id="dad27-196">Leia as propriedades e as relações do objeto Subscription.</span><span class="sxs-lookup"><span data-stu-id="dad27-196">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="dad27-197">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="dad27-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="dad27-198">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="dad27-198">None</span></span> | <span data-ttu-id="dad27-199">Excluir um objeto Subscription.</span><span class="sxs-lookup"><span data-stu-id="dad27-199">Delete a subscription object.</span></span> |

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
