---
title: tipo de recurso de assinatura
description: 'Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:'
localization_priority: Normal
author: piotrci
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d70c6d56a95c8725d214b99a4ad45f0245b51173
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008100"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="c0bf1-104">tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="c0bf1-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0bf1-105">Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="c0bf1-106">Atualmente, as assinaturas estão habilitadas para as seguintes coleções de recursos:</span><span class="sxs-lookup"><span data-stu-id="c0bf1-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="c0bf1-107">Um [mensagem][], [evento][], ou [contato][] no Outlook</span><span class="sxs-lookup"><span data-stu-id="c0bf1-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="c0bf1-108">Um [conversa][] de um grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="c0bf1-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="c0bf1-109">Conteúdo da hierarquia de uma pasta raiz [driveItem][] no OneDrive for Business ou de uma pasta raiz ou uma subpasta [driveItem][] no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="c0bf1-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="c0bf1-110">Um [usuário][] ou [grupo][] no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c0bf1-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="c0bf1-111">Um [alerta][] da API de Segurança do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c0bf1-111">An [alert][] from the Microsoft Graph Security API</span></span>


## <a name="json-representation"></a><span data-ttu-id="c0bf1-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0bf1-112">JSON representation</span></span>

<span data-ttu-id="c0bf1-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-113">Here is a JSON representation of the resource.</span></span>

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
  "lifecycleNotificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="c0bf1-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0bf1-114">Properties</span></span>

| <span data-ttu-id="c0bf1-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0bf1-115">Property</span></span> | <span data-ttu-id="c0bf1-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0bf1-116">Type</span></span> | <span data-ttu-id="c0bf1-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0bf1-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="c0bf1-118">changeType</span><span class="sxs-lookup"><span data-stu-id="c0bf1-118">changeType</span></span> | <span data-ttu-id="c0bf1-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0bf1-119">string</span></span> | <span data-ttu-id="c0bf1-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-120">Required.</span></span> <span data-ttu-id="c0bf1-121">Indica o tipo de alteração no recurso inscrito que gerará uma notificação.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="c0bf1-122">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="c0bf1-123">Vários valores podem ser combinados usando uma lista separada por vírgula.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-123">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="c0bf1-124">Observação: As notificações do item na raiz da unidade suportam somente `updated` changeType.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="c0bf1-125">Notificações de grupos e usuário suportam `updated` e `deleted` changeType.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-125">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="c0bf1-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="c0bf1-126">notificationUrl</span></span> | <span data-ttu-id="c0bf1-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0bf1-127">string</span></span> | <span data-ttu-id="c0bf1-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-128">Required.</span></span> <span data-ttu-id="c0bf1-129">A URL do ponto de extremidade que recebe as notificações.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-129">The URL of the endpoint that receives the notifications.</span></span> <span data-ttu-id="c0bf1-130">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="c0bf1-131">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="c0bf1-131">lifecycleNotificationUrl</span></span> | <span data-ttu-id="c0bf1-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0bf1-132">string</span></span> | <span data-ttu-id="c0bf1-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-133">Optional.</span></span> <span data-ttu-id="c0bf1-134">A URL do ponto de extremidade que recebe notificações de ciclo `subscriptionRemoved` de `missed` vida, incluindo e notificações.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-134">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="c0bf1-135">Se não for fornecido, as notificações serão entregues ao **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-135">If not provided, those notifications will be delivered to **notificationUrl**.</span></span> <span data-ttu-id="c0bf1-136">[Leia mais](/graph/webhooks-outlook-authz.md) sobre como os recursos do Outlook usam notificações de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-136">[Read more](/graph/webhooks-outlook-authz.md) about how Outlook resources use lifecycle notifications.</span></span>  <span data-ttu-id="c0bf1-137">Esta URL deve usar o protocolo HTTPS.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-137">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="c0bf1-138">recurso</span><span class="sxs-lookup"><span data-stu-id="c0bf1-138">resource</span></span> | <span data-ttu-id="c0bf1-139">string</span><span class="sxs-lookup"><span data-stu-id="c0bf1-139">string</span></span> | <span data-ttu-id="c0bf1-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-140">Required.</span></span> <span data-ttu-id="c0bf1-141">Especifica o recurso que será monitorado para detectar alterações.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-141">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="c0bf1-142">Não incluir a URL base (`https://graph.microsoft.com/beta/`).</span><span class="sxs-lookup"><span data-stu-id="c0bf1-142">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="c0bf1-143">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c0bf1-143">expirationDateTime</span></span> | <span data-ttu-id="c0bf1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0bf1-144">DateTimeOffset</span></span> | <span data-ttu-id="c0bf1-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-145">Required.</span></span> <span data-ttu-id="c0bf1-146">Especifica a data e a hora em que a assinatura do webhook expira.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-146">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="c0bf1-147">O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-147">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="c0bf1-148">Confira na tabela abaixo o tempo máximo permitido para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-148">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="c0bf1-149">clientState</span><span class="sxs-lookup"><span data-stu-id="c0bf1-149">clientState</span></span> | <span data-ttu-id="c0bf1-150">string</span><span class="sxs-lookup"><span data-stu-id="c0bf1-150">string</span></span> | <span data-ttu-id="c0bf1-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-151">Optional.</span></span> <span data-ttu-id="c0bf1-152">Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-152">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="c0bf1-153">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-153">The maximum length is 255 characters.</span></span> <span data-ttu-id="c0bf1-154">O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-154">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="c0bf1-155">id</span><span class="sxs-lookup"><span data-stu-id="c0bf1-155">id</span></span> | <span data-ttu-id="c0bf1-156">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0bf1-156">string</span></span> | <span data-ttu-id="c0bf1-p110">Identificador exclusivo da assinatura. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="c0bf1-159">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="c0bf1-159">applicationId</span></span> | <span data-ttu-id="c0bf1-160">string</span><span class="sxs-lookup"><span data-stu-id="c0bf1-160">string</span></span> | <span data-ttu-id="c0bf1-161">Identificador do aplicativo usado para criar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-161">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="c0bf1-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-162">Read-only.</span></span> |
| <span data-ttu-id="c0bf1-163">creatorId</span><span class="sxs-lookup"><span data-stu-id="c0bf1-163">creatorId</span></span> | <span data-ttu-id="c0bf1-164">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0bf1-164">string</span></span> | <span data-ttu-id="c0bf1-165">Identificador de usuário ou entidade de serviço que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-165">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="c0bf1-166">Se o aplicativo usado delegada permissões para criar a assinatura, esse campo contém a id do usuário que entrou no aplicativo chamado em nome dele.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-166">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="c0bf1-167">Se o aplicativo usou permissões do aplicativo, esse campo contém a id da entidade de serviço correspondente ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-167">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="c0bf1-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-168">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="c0bf1-169">Tamanho máximo da assinatura por tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="c0bf1-169">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="c0bf1-170">Recurso</span><span class="sxs-lookup"><span data-stu-id="c0bf1-170">Resource</span></span>            | <span data-ttu-id="c0bf1-171">Tempo de Expiração Máximo</span><span class="sxs-lookup"><span data-stu-id="c0bf1-171">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="c0bf1-172">Usuário, grupo, outros recursos de diretório</span><span class="sxs-lookup"><span data-stu-id="c0bf1-172">User, group, other directory resources</span></span>   | <span data-ttu-id="c0bf1-173">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c0bf1-173">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c0bf1-174">Email</span><span class="sxs-lookup"><span data-stu-id="c0bf1-174">Mail</span></span>                | <span data-ttu-id="c0bf1-175">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c0bf1-175">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c0bf1-176">Calendário</span><span class="sxs-lookup"><span data-stu-id="c0bf1-176">Calendar</span></span>            | <span data-ttu-id="c0bf1-177">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c0bf1-177">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c0bf1-178">Contatos</span><span class="sxs-lookup"><span data-stu-id="c0bf1-178">Contacts</span></span>            | <span data-ttu-id="c0bf1-179">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c0bf1-179">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c0bf1-180">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="c0bf1-180">Group conversations</span></span> | <span data-ttu-id="c0bf1-181">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c0bf1-181">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c0bf1-182">Itens raiz de unidade</span><span class="sxs-lookup"><span data-stu-id="c0bf1-182">Drive root items</span></span>    | <span data-ttu-id="c0bf1-183">4230 minutos (em 3 dias)</span><span class="sxs-lookup"><span data-stu-id="c0bf1-183">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="c0bf1-184">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="c0bf1-184">Security alerts</span></span>     | <span data-ttu-id="c0bf1-185">43200 minutos (em 30 dias )</span><span class="sxs-lookup"><span data-stu-id="c0bf1-185">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="c0bf1-186">**Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor suportado.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-186">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="c0bf1-187">No futuro, as solicitações para criar ou renovar uma assinatura além do valor máximo falharão.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-187">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="c0bf1-188">Relações</span><span class="sxs-lookup"><span data-stu-id="c0bf1-188">Relationships</span></span>

<span data-ttu-id="c0bf1-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0bf1-189">None</span></span>

## <a name="methods"></a><span data-ttu-id="c0bf1-190">Métodos</span><span class="sxs-lookup"><span data-stu-id="c0bf1-190">Methods</span></span>

| <span data-ttu-id="c0bf1-191">Método</span><span class="sxs-lookup"><span data-stu-id="c0bf1-191">Method</span></span> | <span data-ttu-id="c0bf1-192">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c0bf1-192">Return Type</span></span> | <span data-ttu-id="c0bf1-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0bf1-193">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="c0bf1-194">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="c0bf1-194">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="c0bf1-195">subscription</span><span class="sxs-lookup"><span data-stu-id="c0bf1-195">subscription</span></span>](subscription.md) | <span data-ttu-id="c0bf1-196">Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-196">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="c0bf1-197">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="c0bf1-197">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="c0bf1-198">subscription</span><span class="sxs-lookup"><span data-stu-id="c0bf1-198">subscription</span></span>](subscription.md) | <span data-ttu-id="c0bf1-199">Renovar uma assinatura atualizando seu tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-199">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="c0bf1-200">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="c0bf1-200">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="c0bf1-201">assinatura</span><span class="sxs-lookup"><span data-stu-id="c0bf1-201">subscription</span></span>](subscription.md) | <span data-ttu-id="c0bf1-202">Lista assinaturas ativas.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-202">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="c0bf1-203">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="c0bf1-203">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="c0bf1-204">subscription</span><span class="sxs-lookup"><span data-stu-id="c0bf1-204">subscription</span></span>](subscription.md) | <span data-ttu-id="c0bf1-205">Leia as propriedades e as relações do objeto Subscription.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-205">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="c0bf1-206">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="c0bf1-206">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="c0bf1-207">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c0bf1-207">None</span></span> | <span data-ttu-id="c0bf1-208">Excluir um objeto Subscription.</span><span class="sxs-lookup"><span data-stu-id="c0bf1-208">Delete a subscription object.</span></span> |

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
  "suppressions": []
}
-->
