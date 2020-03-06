---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 88d897b5e508a83a78e1c2151081247d732150b4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509742"
---
# <a name="get-subscription"></a><span data-ttu-id="faab0-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="faab0-103">Get subscription</span></span>

<span data-ttu-id="faab0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="faab0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="faab0-105">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="faab0-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="faab0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="faab0-106">Permissions</span></span>

<span data-ttu-id="faab0-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="faab0-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="faab0-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faab0-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="faab0-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="faab0-109">Supported resource</span></span> | <span data-ttu-id="faab0-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="faab0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="faab0-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="faab0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="faab0-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="faab0-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="faab0-113">contato</span><span class="sxs-lookup"><span data-stu-id="faab0-113">contact</span></span>](../resources/contact.md) | <span data-ttu-id="faab0-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="faab0-114">Contacts.Read</span></span> | <span data-ttu-id="faab0-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="faab0-115">Contacts.Read</span></span> | <span data-ttu-id="faab0-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="faab0-116">Contacts.Read</span></span> |
|<span data-ttu-id="faab0-117">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="faab0-117">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="faab0-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="faab0-118">Not supported</span></span> | <span data-ttu-id="faab0-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="faab0-119">Files.ReadWrite</span></span> | <span data-ttu-id="faab0-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="faab0-120">Not supported</span></span> |
|<span data-ttu-id="faab0-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="faab0-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="faab0-122">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faab0-122">Files.ReadWrite.All</span></span> | <span data-ttu-id="faab0-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="faab0-123">Not supported</span></span> | <span data-ttu-id="faab0-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faab0-124">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="faab0-125">evento</span><span class="sxs-lookup"><span data-stu-id="faab0-125">event</span></span>](../resources/event.md) | <span data-ttu-id="faab0-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="faab0-126">Calendars.Read</span></span> | <span data-ttu-id="faab0-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="faab0-127">Calendars.Read</span></span> | <span data-ttu-id="faab0-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="faab0-128">Calendars.Read</span></span> |
|[<span data-ttu-id="faab0-129">grupo</span><span class="sxs-lookup"><span data-stu-id="faab0-129">group</span></span>](../resources/group.md) | <span data-ttu-id="faab0-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="faab0-130">Group.Read.All</span></span> | <span data-ttu-id="faab0-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="faab0-131">Not supported</span></span> | <span data-ttu-id="faab0-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="faab0-132">Group.Read.All</span></span> |
|[<span data-ttu-id="faab0-133">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="faab0-133">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="faab0-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="faab0-134">Group.Read.All</span></span> | <span data-ttu-id="faab0-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="faab0-135">Not supported</span></span> | <span data-ttu-id="faab0-136">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="faab0-136">Not supported</span></span> |
|[<span data-ttu-id="faab0-137">message</span><span class="sxs-lookup"><span data-stu-id="faab0-137">message</span></span>](../resources/message.md) | <span data-ttu-id="faab0-138">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="faab0-138">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="faab0-139">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="faab0-139">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="faab0-140">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="faab0-140">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="faab0-141">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="faab0-141">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="faab0-142">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faab0-142">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="faab0-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="faab0-143">Not supported</span></span> | <span data-ttu-id="faab0-144">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faab0-144">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="faab0-145">Usuário</span><span class="sxs-lookup"><span data-stu-id="faab0-145">user</span></span>](../resources/user.md) | <span data-ttu-id="faab0-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="faab0-146">User.Read.All</span></span> | <span data-ttu-id="faab0-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="faab0-147">User.Read.All</span></span> | <span data-ttu-id="faab0-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="faab0-148">User.Read.All</span></span> |

> <span data-ttu-id="faab0-149">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="faab0-149">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="faab0-150">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="faab0-150">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="faab0-151">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="faab0-151">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="faab0-152">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="faab0-152">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="faab0-153">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="faab0-153">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="faab0-154">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="faab0-154">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="faab0-155">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="faab0-155">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="faab0-156">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="faab0-156">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="faab0-157">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="faab0-157">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="faab0-158">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="faab0-158">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="faab0-159">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="faab0-159">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="faab0-160">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="faab0-160">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="faab0-161">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="faab0-161">Optional query parameters</span></span>

<span data-ttu-id="faab0-162">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="faab0-162">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="faab0-163">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="faab0-163">Request headers</span></span>

| <span data-ttu-id="faab0-164">Nome</span><span class="sxs-lookup"><span data-stu-id="faab0-164">Name</span></span>       | <span data-ttu-id="faab0-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="faab0-165">Type</span></span> | <span data-ttu-id="faab0-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="faab0-166">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="faab0-167">Autorização</span><span class="sxs-lookup"><span data-stu-id="faab0-167">Authorization</span></span>  | <span data-ttu-id="faab0-168">string</span><span class="sxs-lookup"><span data-stu-id="faab0-168">string</span></span>  | <span data-ttu-id="faab0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="faab0-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="faab0-171">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="faab0-171">Request body</span></span>

<span data-ttu-id="faab0-172">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="faab0-172">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="faab0-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="faab0-173">Response</span></span>

<span data-ttu-id="faab0-174">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="faab0-174">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faab0-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="faab0-175">Example</span></span>

##### <a name="request"></a><span data-ttu-id="faab0-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="faab0-176">Request</span></span>

<span data-ttu-id="faab0-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="faab0-177">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="faab0-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="faab0-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="faab0-179">C#</span><span class="sxs-lookup"><span data-stu-id="faab0-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="faab0-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="faab0-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="faab0-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="faab0-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="faab0-182">Java</span><span class="sxs-lookup"><span data-stu-id="faab0-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="faab0-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="faab0-183">Response</span></span>

<span data-ttu-id="faab0-184">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="faab0-184">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string",
  "latestSupportedTlsVersion": "v1_2"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
