---
title: Criar assinatura
description: Assinar um aplicativo de escuta para receber notificações quando as alterações de dados em um recurso do Microsoft Graph.
localization_priority: Normal
ms.openlocfilehash: 5b7f465e556d1fb752bcb2d3c962fd6444d462c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805050"
---
# <a name="create-subscription"></a><span data-ttu-id="11777-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="11777-103">Create subscription</span></span>

> <span data-ttu-id="11777-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="11777-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11777-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="11777-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="11777-106">Assinar um aplicativo de escuta para receber notificações quando as alterações de dados em um recurso do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="11777-106">Subscribes a listener application to receive notifications when data on a Microsoft Graph resource changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="11777-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="11777-107">Permissions</span></span>

<span data-ttu-id="11777-108">Criar uma assinatura requer a permissão de leitura para o recurso para o qual o aplicativo receberá notificações.</span><span class="sxs-lookup"><span data-stu-id="11777-108">Creating a subscription requires read permission to the resource for which the app will receive notifications.</span></span> <span data-ttu-id="11777-109">Por exemplo, para obter notificações sobre mensagens, seu aplicativo precisa o `Mail.Read` permissão.</span><span class="sxs-lookup"><span data-stu-id="11777-109">For example, to get notifications about Messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="11777-110">A tabela a seguir lista a permissão sugerida necessária para cada recurso.</span><span class="sxs-lookup"><span data-stu-id="11777-110">The following table lists the suggested permission needed for each resource.</span></span> <span data-ttu-id="11777-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11777-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11777-112">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="11777-112">Resource type / Item</span></span>        | <span data-ttu-id="11777-113">Permissão</span><span class="sxs-lookup"><span data-stu-id="11777-113">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="11777-114">Contatos</span><span class="sxs-lookup"><span data-stu-id="11777-114">Contacts</span></span>                    | <span data-ttu-id="11777-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="11777-115">Contacts.Read</span></span>       |
| <span data-ttu-id="11777-116">Conversas</span><span class="sxs-lookup"><span data-stu-id="11777-116">Conversations</span></span>               | <span data-ttu-id="11777-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="11777-117">Group.Read.All</span></span>      |
| <span data-ttu-id="11777-118">Eventos</span><span class="sxs-lookup"><span data-stu-id="11777-118">Events</span></span>                      | <span data-ttu-id="11777-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="11777-119">Calendars.Read</span></span>      |
| <span data-ttu-id="11777-120">Mensagens</span><span class="sxs-lookup"><span data-stu-id="11777-120">Messages</span></span>                    | <span data-ttu-id="11777-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="11777-121">Mail.Read</span></span>           |
| <span data-ttu-id="11777-122">Grupos</span><span class="sxs-lookup"><span data-stu-id="11777-122">Groups</span></span>                      | <span data-ttu-id="11777-123">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="11777-123">Group.Read.All</span></span>      |
| <span data-ttu-id="11777-124">Usuários</span><span class="sxs-lookup"><span data-stu-id="11777-124">Users</span></span>                       | <span data-ttu-id="11777-125">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="11777-125">User.Read.All</span></span>       |
| <span data-ttu-id="11777-126">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="11777-126">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="11777-127">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11777-127">Files.ReadWrite</span></span>     |
| <span data-ttu-id="11777-128">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="11777-128">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="11777-129">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11777-129">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="11777-130">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="11777-130">Security alert</span></span>              | <span data-ttu-id="11777-131">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11777-131">SecurityEvents.ReadWrite.All</span></span> |

> <span data-ttu-id="11777-132">**Observação:** O ponto de extremidade /beta permite que as permissões de aplicativo para a maioria dos recursos.</span><span class="sxs-lookup"><span data-stu-id="11777-132">**Note:** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="11777-133">Não há suporte para conversas em itens de raiz uma unidade OneDrive e de grupo com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11777-133">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="11777-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11777-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="11777-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11777-135">Request headers</span></span>

| <span data-ttu-id="11777-136">Nome</span><span class="sxs-lookup"><span data-stu-id="11777-136">Name</span></span>       | <span data-ttu-id="11777-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="11777-137">Type</span></span> | <span data-ttu-id="11777-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="11777-138">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="11777-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="11777-139">Authorization</span></span>  | <span data-ttu-id="11777-140">string</span><span class="sxs-lookup"><span data-stu-id="11777-140">string</span></span>  | <span data-ttu-id="11777-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11777-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="11777-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="11777-143">Response</span></span>

<span data-ttu-id="11777-144">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11777-144">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11777-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11777-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="11777-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11777-146">Request</span></span>

<span data-ttu-id="11777-147">No corpo da solicitação, fornece uma representação JSON do objeto de [inscrição](../resources/subscription.md) .</span><span class="sxs-lookup"><span data-stu-id="11777-147">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="11777-148">O `clientState` campo é opcional.</span><span class="sxs-lookup"><span data-stu-id="11777-148">The `clientState` field is optional.</span></span>

<span data-ttu-id="11777-149">Esta amostra da solicitação cria uma assinatura de notificações sobre novos emails recebidos pelo usuário atualmente conectado.</span><span class="sxs-lookup"><span data-stu-id="11777-149">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
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

<span data-ttu-id="11777-150">A seguir estão os valores válidos para a propriedade de recurso:</span><span class="sxs-lookup"><span data-stu-id="11777-150">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="11777-151">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="11777-151">Resource type</span></span> | <span data-ttu-id="11777-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="11777-152">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="11777-153">Email</span><span class="sxs-lookup"><span data-stu-id="11777-153">Mail</span></span>|<span data-ttu-id="11777-154">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="11777-154">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="11777-155">me/messages</span><span class="sxs-lookup"><span data-stu-id="11777-155">me/messages</span></span>|
|<span data-ttu-id="11777-156">Contatos</span><span class="sxs-lookup"><span data-stu-id="11777-156">Contacts</span></span>|<span data-ttu-id="11777-157">me/contacts</span><span class="sxs-lookup"><span data-stu-id="11777-157">me/contacts</span></span>|
|<span data-ttu-id="11777-158">Calendários</span><span class="sxs-lookup"><span data-stu-id="11777-158">Calendars</span></span>|<span data-ttu-id="11777-159">me/events</span><span class="sxs-lookup"><span data-stu-id="11777-159">me/events</span></span>|
|<span data-ttu-id="11777-160">Usuários</span><span class="sxs-lookup"><span data-stu-id="11777-160">Users</span></span>|<span data-ttu-id="11777-161">users</span><span class="sxs-lookup"><span data-stu-id="11777-161">users</span></span>|
|<span data-ttu-id="11777-162">Grupos</span><span class="sxs-lookup"><span data-stu-id="11777-162">Groups</span></span>|<span data-ttu-id="11777-163">grupos</span><span class="sxs-lookup"><span data-stu-id="11777-163">groups</span></span>|
|<span data-ttu-id="11777-164">Conversas</span><span class="sxs-lookup"><span data-stu-id="11777-164">Conversations</span></span>|<span data-ttu-id="11777-165">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="11777-165">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="11777-166">Unidades</span><span class="sxs-lookup"><span data-stu-id="11777-166">Drives</span></span>|<span data-ttu-id="11777-167">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="11777-167">me/drive/root</span></span>|
|<span data-ttu-id="11777-168">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="11777-168">Security alert</span></span>|<span data-ttu-id="11777-169">alertas de segurança /? $filter = status eq 'Novo'</span><span class="sxs-lookup"><span data-stu-id="11777-169">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="11777-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="11777-170">Response</span></span>

<span data-ttu-id="11777-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11777-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="11777-174">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="11777-174">Notification endpoint validation</span></span>

<span data-ttu-id="11777-175">O ponto de extremidade de notificação de inscrição (especificado no `notificationUrl` propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para que as alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="11777-175">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="11777-176">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de solicitação inválida a 400.</span><span class="sxs-lookup"><span data-stu-id="11777-176">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
