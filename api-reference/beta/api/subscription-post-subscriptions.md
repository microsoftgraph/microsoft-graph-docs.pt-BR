---
title: Criar assinatura
description: Assinar um aplicativo de escuta para receber notificações quando as alterações de dados em um recurso do Microsoft Graph.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 002dd88c7db2650be2303e7df6f86ce9a5fbdaa9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527574"
---
# <a name="create-subscription"></a><span data-ttu-id="22283-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="22283-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22283-104">Assinar um aplicativo de escuta para receber notificações quando as alterações de dados em um recurso do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="22283-104">Subscribes a listener application to receive notifications when data on a Microsoft Graph resource changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="22283-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="22283-105">Permissions</span></span>

<span data-ttu-id="22283-106">Criar uma assinatura requer a permissão de leitura para o recurso para o qual o aplicativo receberá notificações.</span><span class="sxs-lookup"><span data-stu-id="22283-106">Creating a subscription requires read permission to the resource for which the app will receive notifications.</span></span> <span data-ttu-id="22283-107">Por exemplo, para obter notificações sobre mensagens, seu aplicativo precisa o `Mail.Read` permissão.</span><span class="sxs-lookup"><span data-stu-id="22283-107">For example, to get notifications about Messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="22283-108">A tabela a seguir lista a permissão sugerida necessária para cada recurso.</span><span class="sxs-lookup"><span data-stu-id="22283-108">The following table lists the suggested permission needed for each resource.</span></span> <span data-ttu-id="22283-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22283-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22283-110">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="22283-110">Resource type / Item</span></span>        | <span data-ttu-id="22283-111">Permissão</span><span class="sxs-lookup"><span data-stu-id="22283-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="22283-112">Contatos</span><span class="sxs-lookup"><span data-stu-id="22283-112">Contacts</span></span>                    | <span data-ttu-id="22283-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="22283-113">Contacts.Read</span></span>       |
| <span data-ttu-id="22283-114">Conversas</span><span class="sxs-lookup"><span data-stu-id="22283-114">Conversations</span></span>               | <span data-ttu-id="22283-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="22283-115">Group.Read.All</span></span>      |
| <span data-ttu-id="22283-116">Eventos</span><span class="sxs-lookup"><span data-stu-id="22283-116">Events</span></span>                      | <span data-ttu-id="22283-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="22283-117">Calendars.Read</span></span>      |
| <span data-ttu-id="22283-118">Mensagens</span><span class="sxs-lookup"><span data-stu-id="22283-118">Messages</span></span>                    | <span data-ttu-id="22283-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="22283-119">Mail.Read</span></span>           |
| <span data-ttu-id="22283-120">Grupos</span><span class="sxs-lookup"><span data-stu-id="22283-120">Groups</span></span>                      | <span data-ttu-id="22283-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="22283-121">Group.Read.All</span></span>      |
| <span data-ttu-id="22283-122">Usuários</span><span class="sxs-lookup"><span data-stu-id="22283-122">Users</span></span>                       | <span data-ttu-id="22283-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="22283-123">User.Read.All</span></span>       |
| <span data-ttu-id="22283-124">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="22283-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="22283-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22283-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="22283-126">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="22283-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="22283-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22283-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="22283-128">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="22283-128">Security alert</span></span>              | <span data-ttu-id="22283-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22283-129">SecurityEvents.ReadWrite.All</span></span> |

> <span data-ttu-id="22283-130">**Observação:** O ponto de extremidade /beta permite que as permissões de aplicativo para a maioria dos recursos.</span><span class="sxs-lookup"><span data-stu-id="22283-130">**Note:** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="22283-131">Não há suporte para conversas em itens de raiz uma unidade OneDrive e de grupo com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="22283-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="22283-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22283-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="22283-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22283-133">Request headers</span></span>

| <span data-ttu-id="22283-134">Nome</span><span class="sxs-lookup"><span data-stu-id="22283-134">Name</span></span>       | <span data-ttu-id="22283-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="22283-135">Type</span></span> | <span data-ttu-id="22283-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="22283-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="22283-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="22283-137">Authorization</span></span>  | <span data-ttu-id="22283-138">string</span><span class="sxs-lookup"><span data-stu-id="22283-138">string</span></span>  | <span data-ttu-id="22283-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22283-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="22283-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="22283-141">Response</span></span>

<span data-ttu-id="22283-142">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22283-142">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22283-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22283-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="22283-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22283-144">Request</span></span>

<span data-ttu-id="22283-145">No corpo da solicitação, fornece uma representação JSON do objeto de [inscrição](../resources/subscription.md) .</span><span class="sxs-lookup"><span data-stu-id="22283-145">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="22283-146">O `clientState` campo é opcional.</span><span class="sxs-lookup"><span data-stu-id="22283-146">The `clientState` field is optional.</span></span>

<span data-ttu-id="22283-147">Esta amostra da solicitação cria uma assinatura de notificações sobre novos emails recebidos pelo usuário atualmente conectado.</span><span class="sxs-lookup"><span data-stu-id="22283-147">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="22283-148">A seguir estão os valores válidos para a propriedade de recurso:</span><span class="sxs-lookup"><span data-stu-id="22283-148">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="22283-149">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="22283-149">Resource type</span></span> | <span data-ttu-id="22283-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="22283-150">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="22283-151">Email</span><span class="sxs-lookup"><span data-stu-id="22283-151">Mail</span></span>|<span data-ttu-id="22283-152">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="22283-152">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="22283-153">me/messages</span><span class="sxs-lookup"><span data-stu-id="22283-153">me/messages</span></span>|
|<span data-ttu-id="22283-154">Contatos</span><span class="sxs-lookup"><span data-stu-id="22283-154">Contacts</span></span>|<span data-ttu-id="22283-155">me/contacts</span><span class="sxs-lookup"><span data-stu-id="22283-155">me/contacts</span></span>|
|<span data-ttu-id="22283-156">Calendários</span><span class="sxs-lookup"><span data-stu-id="22283-156">Calendars</span></span>|<span data-ttu-id="22283-157">me/events</span><span class="sxs-lookup"><span data-stu-id="22283-157">me/events</span></span>|
|<span data-ttu-id="22283-158">Usuários</span><span class="sxs-lookup"><span data-stu-id="22283-158">Users</span></span>|<span data-ttu-id="22283-159">users</span><span class="sxs-lookup"><span data-stu-id="22283-159">users</span></span>|
|<span data-ttu-id="22283-160">Grupos</span><span class="sxs-lookup"><span data-stu-id="22283-160">Groups</span></span>|<span data-ttu-id="22283-161">Grupos</span><span class="sxs-lookup"><span data-stu-id="22283-161">groups</span></span>|
|<span data-ttu-id="22283-162">Conversas</span><span class="sxs-lookup"><span data-stu-id="22283-162">Conversations</span></span>|<span data-ttu-id="22283-163">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="22283-163">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="22283-164">Unidades</span><span class="sxs-lookup"><span data-stu-id="22283-164">Drives</span></span>|<span data-ttu-id="22283-165">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="22283-165">me/drive/root</span></span>|
|<span data-ttu-id="22283-166">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="22283-166">Security alert</span></span>|<span data-ttu-id="22283-167">alertas de segurança /? $filter = status eq 'Novo'</span><span class="sxs-lookup"><span data-stu-id="22283-167">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="22283-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="22283-168">Response</span></span>

<span data-ttu-id="22283-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22283-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="22283-172">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="22283-172">Notification endpoint validation</span></span>

<span data-ttu-id="22283-173">O ponto de extremidade de notificação de inscrição (especificado no `notificationUrl` propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para que as alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="22283-173">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="22283-174">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de solicitação inválida a 400.</span><span class="sxs-lookup"><span data-stu-id="22283-174">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-post-subscriptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
