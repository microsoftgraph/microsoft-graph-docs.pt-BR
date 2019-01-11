---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações quando os dados no Microsoft Graph são alterados.
localization_priority: Priority
ms.openlocfilehash: 07b2c055c49a79f1d9d3407ba8da5a5658766d20
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889625"
---
# <a name="create-subscription"></a><span data-ttu-id="544e9-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="544e9-103">Create subscription</span></span>

<span data-ttu-id="544e9-104">Assina um aplicativo de escuta para receber notificações quando os dados no Microsoft Graph são alterados.</span><span class="sxs-lookup"><span data-stu-id="544e9-104">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="544e9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="544e9-105">Permissions</span></span>

<span data-ttu-id="544e9-p101">Criar uma assinatura exige escopo de leitura para o recurso. Por exemplo, para obter mensagens de notificações, seu aplicativo precisa da permissão `Mail.Read`. A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="544e9-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="544e9-110">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="544e9-110">Resource type / Item</span></span>        | <span data-ttu-id="544e9-111">Permissão</span><span class="sxs-lookup"><span data-stu-id="544e9-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="544e9-112">Contatos</span><span class="sxs-lookup"><span data-stu-id="544e9-112">Contacts</span></span>                    | <span data-ttu-id="544e9-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="544e9-113">Contacts.Read</span></span>       |
| <span data-ttu-id="544e9-114">Conversas</span><span class="sxs-lookup"><span data-stu-id="544e9-114">Conversations</span></span>               | <span data-ttu-id="544e9-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="544e9-115">Group.Read.All</span></span>      |
| <span data-ttu-id="544e9-116">Eventos</span><span class="sxs-lookup"><span data-stu-id="544e9-116">Events</span></span>                      | <span data-ttu-id="544e9-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="544e9-117">Calendars.Read</span></span>      |
| <span data-ttu-id="544e9-118">Mensagens</span><span class="sxs-lookup"><span data-stu-id="544e9-118">Messages</span></span>                    | <span data-ttu-id="544e9-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="544e9-119">Mail.Read</span></span>           |
| <span data-ttu-id="544e9-120">Grupos</span><span class="sxs-lookup"><span data-stu-id="544e9-120">Groups</span></span>                      | <span data-ttu-id="544e9-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="544e9-121">Group.Read.All</span></span>      |
| <span data-ttu-id="544e9-122">Usuários</span><span class="sxs-lookup"><span data-stu-id="544e9-122">Users</span></span>                       | <span data-ttu-id="544e9-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="544e9-123">User.Read.All</span></span>       |
| <span data-ttu-id="544e9-124">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="544e9-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="544e9-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="544e9-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="544e9-126">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="544e9-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="544e9-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="544e9-127">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="544e9-128">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="544e9-128">Security alert</span></span>| <span data-ttu-id="544e9-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="544e9-129">SecurityEvents.ReadWrite.All</span></span> |

 > <span data-ttu-id="544e9-130">**Observação:** O ponto de extremidade /v1.0 permite que as permissões de aplicativo para a maioria dos recursos.</span><span class="sxs-lookup"><span data-stu-id="544e9-130">**Note:** The /v1.0 endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="544e9-131">Não há suporte para conversas em itens de raiz uma unidade OneDrive e de grupo com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="544e9-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="544e9-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="544e9-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="544e9-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="544e9-133">Request headers</span></span>

| <span data-ttu-id="544e9-134">Nome</span><span class="sxs-lookup"><span data-stu-id="544e9-134">Name</span></span>       | <span data-ttu-id="544e9-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="544e9-135">Type</span></span> | <span data-ttu-id="544e9-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="544e9-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="544e9-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="544e9-137">Authorization</span></span>  | <span data-ttu-id="544e9-138">string</span><span class="sxs-lookup"><span data-stu-id="544e9-138">string</span></span>  | <span data-ttu-id="544e9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="544e9-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="544e9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="544e9-141">Response</span></span>

<span data-ttu-id="544e9-142">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="544e9-142">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="544e9-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="544e9-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="544e9-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="544e9-144">Request</span></span>

<span data-ttu-id="544e9-145">Veja a seguir um exemplo da solicitação para enviar uma notificação quando o usuário receber um novo email.</span><span class="sxs-lookup"><span data-stu-id="544e9-145">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="544e9-146">No corpo da solicitação, fornece uma representação JSON do objeto de [inscrição](../resources/subscription.md) .</span><span class="sxs-lookup"><span data-stu-id="544e9-146">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="544e9-147">O `clientState` campo é opcional.</span><span class="sxs-lookup"><span data-stu-id="544e9-147">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="544e9-148">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="544e9-148">Resources examples</span></span>

<span data-ttu-id="544e9-149">Estes são os valores válidos da propriedade de recurso da assinatura:</span><span class="sxs-lookup"><span data-stu-id="544e9-149">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="544e9-150">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="544e9-150">Resource type</span></span> | <span data-ttu-id="544e9-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="544e9-151">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="544e9-152">Email</span><span class="sxs-lookup"><span data-stu-id="544e9-152">Mail</span></span>|<span data-ttu-id="544e9-153">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="544e9-153">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="544e9-154">me/messages</span><span class="sxs-lookup"><span data-stu-id="544e9-154">me/messages</span></span>|
|<span data-ttu-id="544e9-155">Contatos</span><span class="sxs-lookup"><span data-stu-id="544e9-155">Contacts</span></span>|<span data-ttu-id="544e9-156">me/contacts</span><span class="sxs-lookup"><span data-stu-id="544e9-156">me/contacts</span></span>|
|<span data-ttu-id="544e9-157">Calendários</span><span class="sxs-lookup"><span data-stu-id="544e9-157">Calendars</span></span>|<span data-ttu-id="544e9-158">me/events</span><span class="sxs-lookup"><span data-stu-id="544e9-158">me/events</span></span>|
|<span data-ttu-id="544e9-159">Usuários</span><span class="sxs-lookup"><span data-stu-id="544e9-159">Users</span></span>|<span data-ttu-id="544e9-160">users</span><span class="sxs-lookup"><span data-stu-id="544e9-160">users</span></span>|
|<span data-ttu-id="544e9-161">Grupos</span><span class="sxs-lookup"><span data-stu-id="544e9-161">Groups</span></span>|<span data-ttu-id="544e9-162">grupos</span><span class="sxs-lookup"><span data-stu-id="544e9-162">groups</span></span>|
|<span data-ttu-id="544e9-163">Conversas</span><span class="sxs-lookup"><span data-stu-id="544e9-163">Conversations</span></span>|<span data-ttu-id="544e9-164">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="544e9-164">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="544e9-165">Unidades</span><span class="sxs-lookup"><span data-stu-id="544e9-165">Drives</span></span>|<span data-ttu-id="544e9-166">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="544e9-166">me/drive/root</span></span>|
|<span data-ttu-id="544e9-167">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="544e9-167">Security alert</span></span>|<span data-ttu-id="544e9-168">alertas de segurança /? $filter = status eq 'Novo'</span><span class="sxs-lookup"><span data-stu-id="544e9-168">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="544e9-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="544e9-169">Response</span></span>

<span data-ttu-id="544e9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="544e9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="544e9-173">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="544e9-173">Notification endpoint validation</span></span>

<span data-ttu-id="544e9-174">O ponto de extremidade de notificação de inscrição (especificado no `notificationUrl` propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para que as alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="544e9-174">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="544e9-175">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de solicitação inválida a 400.</span><span class="sxs-lookup"><span data-stu-id="544e9-175">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
