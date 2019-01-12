---
title: tipo de recurso de assinatura
description: 'Uma assinatura permite que um aplicativo cliente receber notificações sobre as alterações de dados no Microsoft Graph. Atualmente, as assinaturas são habilitadas para os seguintes recursos:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 0f6baa3ca36b91c8a4dd38086a7fc0eebdcf46e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982460"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="af8a1-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="af8a1-104">subscription resource type</span></span>

> <span data-ttu-id="af8a1-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="af8a1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af8a1-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="af8a1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="af8a1-107">Uma assinatura permite que um aplicativo cliente receber notificações sobre as alterações de dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="af8a1-107">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="af8a1-108">Atualmente, as assinaturas são habilitadas para os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="af8a1-108">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="af8a1-109">Email, eventos e contatos do Outlook.</span><span class="sxs-lookup"><span data-stu-id="af8a1-109">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="af8a1-110">Conversas de Grupos do Office.</span><span class="sxs-lookup"><span data-stu-id="af8a1-110">Conversations from Office Groups.</span></span>
- <span data-ttu-id="af8a1-111">Itens raiz da unidade do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="af8a1-111">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="af8a1-112">Usuários e grupos do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="af8a1-112">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="af8a1-113">Alertas do API de segurança do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="af8a1-113">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af8a1-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af8a1-114">JSON representation</span></span>

<span data-ttu-id="af8a1-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af8a1-115">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="af8a1-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af8a1-116">Properties</span></span>

| <span data-ttu-id="af8a1-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af8a1-117">Property</span></span> | <span data-ttu-id="af8a1-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="af8a1-118">Type</span></span> | <span data-ttu-id="af8a1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="af8a1-119">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="af8a1-120">changeType</span><span class="sxs-lookup"><span data-stu-id="af8a1-120">changeType</span></span> | <span data-ttu-id="af8a1-121">string</span><span class="sxs-lookup"><span data-stu-id="af8a1-121">string</span></span> | <span data-ttu-id="af8a1-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af8a1-122">Required.</span></span> <span data-ttu-id="af8a1-123">Indica o tipo de alteração no recurso inscrito que gerará uma notificação.</span><span class="sxs-lookup"><span data-stu-id="af8a1-123">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="af8a1-124">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="af8a1-124">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="af8a1-125">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="af8a1-125">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="af8a1-126">Observação: Notificações de item de raiz de unidade suportam somente a `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="af8a1-126">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="af8a1-127">Suportam a notificações de usuário e grupo `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="af8a1-127">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="af8a1-128">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="af8a1-128">notificationUrl</span></span> | <span data-ttu-id="af8a1-129">string</span><span class="sxs-lookup"><span data-stu-id="af8a1-129">string</span></span> | <span data-ttu-id="af8a1-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af8a1-130">Required.</span></span> <span data-ttu-id="af8a1-131">A URL do ponto de extremidade que receberá as notificações.</span><span class="sxs-lookup"><span data-stu-id="af8a1-131">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="af8a1-132">Essa URL deve tornar a usar o HTTPS protocolo.</span><span class="sxs-lookup"><span data-stu-id="af8a1-132">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="af8a1-133">recurso</span><span class="sxs-lookup"><span data-stu-id="af8a1-133">resource</span></span> | <span data-ttu-id="af8a1-134">string</span><span class="sxs-lookup"><span data-stu-id="af8a1-134">string</span></span> | <span data-ttu-id="af8a1-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af8a1-135">Required.</span></span> <span data-ttu-id="af8a1-136">Especifica o recurso que será monitorado para que as alterações.</span><span class="sxs-lookup"><span data-stu-id="af8a1-136">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="af8a1-137">Não incluir a URL base (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="af8a1-137">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="af8a1-138">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="af8a1-138">expirationDateTime</span></span> | <span data-ttu-id="af8a1-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af8a1-139">DateTimeOffset</span></span> | <span data-ttu-id="af8a1-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af8a1-140">Required.</span></span> <span data-ttu-id="af8a1-141">Especifica a data e a hora em que a assinatura de webhook expira.</span><span class="sxs-lookup"><span data-stu-id="af8a1-141">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="af8a1-142">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="af8a1-142">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="af8a1-143">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="af8a1-143">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="af8a1-144">clientState</span><span class="sxs-lookup"><span data-stu-id="af8a1-144">clientState</span></span> | <span data-ttu-id="af8a1-145">string</span><span class="sxs-lookup"><span data-stu-id="af8a1-145">string</span></span> | <span data-ttu-id="af8a1-146">Opcional.</span><span class="sxs-lookup"><span data-stu-id="af8a1-146">Optional.</span></span> <span data-ttu-id="af8a1-147">Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação.</span><span class="sxs-lookup"><span data-stu-id="af8a1-147">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="af8a1-148">The maximum length is 255 characters.</span><span class="sxs-lookup"><span data-stu-id="af8a1-148">The maximum length is 255 characters.</span></span> <span data-ttu-id="af8a1-149">O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação.</span><span class="sxs-lookup"><span data-stu-id="af8a1-149">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="af8a1-150">id</span><span class="sxs-lookup"><span data-stu-id="af8a1-150">id</span></span> | <span data-ttu-id="af8a1-151">string</span><span class="sxs-lookup"><span data-stu-id="af8a1-151">string</span></span> | <span data-ttu-id="af8a1-p110">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af8a1-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="af8a1-154">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="af8a1-154">applicationId</span></span> | <span data-ttu-id="af8a1-155">string</span><span class="sxs-lookup"><span data-stu-id="af8a1-155">string</span></span> | <span data-ttu-id="af8a1-156">Identificador do aplicativo usado para criar a inscrição.</span><span class="sxs-lookup"><span data-stu-id="af8a1-156">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="af8a1-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af8a1-157">Read-only.</span></span> |
| <span data-ttu-id="af8a1-158">creatorId</span><span class="sxs-lookup"><span data-stu-id="af8a1-158">creatorId</span></span> | <span data-ttu-id="af8a1-159">string</span><span class="sxs-lookup"><span data-stu-id="af8a1-159">string</span></span> | <span data-ttu-id="af8a1-160">Identificador do usuário ou da entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="af8a1-160">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="af8a1-161">Se o aplicativo usado delegadas permissões para criar a assinatura, esse campo contém a id do usuário entrou no de que aplicativo chamado em nome.</span><span class="sxs-lookup"><span data-stu-id="af8a1-161">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="af8a1-162">Se o aplicativo usado permissões de aplicativo, esse campo contém a id da entidade de serviço correspondente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="af8a1-162">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="af8a1-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af8a1-163">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="af8a1-164">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="af8a1-164">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="af8a1-165">Recurso</span><span class="sxs-lookup"><span data-stu-id="af8a1-165">Resource</span></span>            | <span data-ttu-id="af8a1-166">Tempo de Expiração Máximo</span><span class="sxs-lookup"><span data-stu-id="af8a1-166">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="af8a1-167">Email</span><span class="sxs-lookup"><span data-stu-id="af8a1-167">Mail</span></span>                | <span data-ttu-id="af8a1-168">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="af8a1-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="af8a1-169">Calendário</span><span class="sxs-lookup"><span data-stu-id="af8a1-169">Calendar</span></span>            | <span data-ttu-id="af8a1-170">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="af8a1-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="af8a1-171">Contatos</span><span class="sxs-lookup"><span data-stu-id="af8a1-171">Contacts</span></span>            | <span data-ttu-id="af8a1-172">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="af8a1-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="af8a1-173">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="af8a1-173">Group conversations</span></span> | <span data-ttu-id="af8a1-174">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="af8a1-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="af8a1-175">Itens raiz de unidade</span><span class="sxs-lookup"><span data-stu-id="af8a1-175">Drive root items</span></span>    | <span data-ttu-id="af8a1-176">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="af8a1-176">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="af8a1-177">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="af8a1-177">Security alerts</span></span>     | <span data-ttu-id="af8a1-178">43200 minutos (em 30 dias)</span><span class="sxs-lookup"><span data-stu-id="af8a1-178">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="af8a1-179">**Observação:** Aplicativos existentes e novos não deve exceder o valor com suporte.</span><span class="sxs-lookup"><span data-stu-id="af8a1-179">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="af8a1-180">No futuro, quaisquer solicitações para criar ou renovar uma assinatura além o valor máximo falhará.</span><span class="sxs-lookup"><span data-stu-id="af8a1-180">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="af8a1-181">Relações</span><span class="sxs-lookup"><span data-stu-id="af8a1-181">Relationships</span></span>

<span data-ttu-id="af8a1-182">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af8a1-182">None</span></span>

## <a name="methods"></a><span data-ttu-id="af8a1-183">Métodos</span><span class="sxs-lookup"><span data-stu-id="af8a1-183">Methods</span></span>

| <span data-ttu-id="af8a1-184">Método</span><span class="sxs-lookup"><span data-stu-id="af8a1-184">Method</span></span> | <span data-ttu-id="af8a1-185">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="af8a1-185">Return Type</span></span> | <span data-ttu-id="af8a1-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="af8a1-186">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="af8a1-187">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="af8a1-187">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="af8a1-188">subscription</span><span class="sxs-lookup"><span data-stu-id="af8a1-188">subscription</span></span>](subscription.md) | <span data-ttu-id="af8a1-189">Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="af8a1-189">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="af8a1-190">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="af8a1-190">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="af8a1-191">subscription</span><span class="sxs-lookup"><span data-stu-id="af8a1-191">subscription</span></span>](subscription.md) | <span data-ttu-id="af8a1-192">Renove uma assinatura atualizando seu horário de expiração.</span><span class="sxs-lookup"><span data-stu-id="af8a1-192">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="af8a1-193">Inscrições de lista</span><span class="sxs-lookup"><span data-stu-id="af8a1-193">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="af8a1-194">subscription</span><span class="sxs-lookup"><span data-stu-id="af8a1-194">subscription</span></span>](subscription.md) | <span data-ttu-id="af8a1-195">Lista inscrições ativas.</span><span class="sxs-lookup"><span data-stu-id="af8a1-195">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="af8a1-196">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="af8a1-196">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="af8a1-197">subscription</span><span class="sxs-lookup"><span data-stu-id="af8a1-197">subscription</span></span>](subscription.md) | <span data-ttu-id="af8a1-198">Leia as propriedades e os relacionamentos de objeto de inscrição.</span><span class="sxs-lookup"><span data-stu-id="af8a1-198">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="af8a1-199">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="af8a1-199">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="af8a1-200">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="af8a1-200">None</span></span> | <span data-ttu-id="af8a1-201">Exclua um objeto de inscrição.</span><span class="sxs-lookup"><span data-stu-id="af8a1-201">Delete a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
