---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 5d2590afad93560bab0a72eb8edd007779f4711b
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108575"
---
# <a name="get-subscription"></a><span data-ttu-id="44a67-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="44a67-103">Get subscription</span></span>

<span data-ttu-id="44a67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44a67-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44a67-105">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="44a67-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="44a67-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="44a67-106">Permissions</span></span>

<span data-ttu-id="44a67-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="44a67-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="44a67-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44a67-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44a67-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="44a67-109">Supported resource</span></span> | <span data-ttu-id="44a67-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44a67-110">Delegated (work or school account)</span></span> | <span data-ttu-id="44a67-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44a67-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44a67-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44a67-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="44a67-113">contato</span><span class="sxs-lookup"><span data-stu-id="44a67-113">contact</span></span>](../resources/contact.md) | <span data-ttu-id="44a67-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="44a67-114">Contacts.Read</span></span> | <span data-ttu-id="44a67-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="44a67-115">Contacts.Read</span></span> | <span data-ttu-id="44a67-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="44a67-116">Contacts.Read</span></span> |
|<span data-ttu-id="44a67-117">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="44a67-117">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="44a67-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="44a67-118">Not supported</span></span> | <span data-ttu-id="44a67-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44a67-119">Files.ReadWrite</span></span> | <span data-ttu-id="44a67-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="44a67-120">Not supported</span></span> |
|<span data-ttu-id="44a67-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="44a67-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="44a67-122">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44a67-122">Files.ReadWrite.All</span></span> | <span data-ttu-id="44a67-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="44a67-123">Not supported</span></span> | <span data-ttu-id="44a67-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44a67-124">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="44a67-125">evento</span><span class="sxs-lookup"><span data-stu-id="44a67-125">event</span></span>](../resources/event.md) | <span data-ttu-id="44a67-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="44a67-126">Calendars.Read</span></span> | <span data-ttu-id="44a67-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="44a67-127">Calendars.Read</span></span> | <span data-ttu-id="44a67-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="44a67-128">Calendars.Read</span></span> |
|[<span data-ttu-id="44a67-129">grupo</span><span class="sxs-lookup"><span data-stu-id="44a67-129">group</span></span>](../resources/group.md) | <span data-ttu-id="44a67-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="44a67-130">Group.Read.All</span></span> | <span data-ttu-id="44a67-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="44a67-131">Not supported</span></span> | <span data-ttu-id="44a67-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="44a67-132">Group.Read.All</span></span> |
|[<span data-ttu-id="44a67-133">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="44a67-133">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="44a67-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="44a67-134">Group.Read.All</span></span> | <span data-ttu-id="44a67-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="44a67-135">Not supported</span></span> | <span data-ttu-id="44a67-136">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="44a67-136">Not supported</span></span> |
|[<span data-ttu-id="44a67-137">list</span><span class="sxs-lookup"><span data-stu-id="44a67-137">list</span></span>](../resources/list.md) | <span data-ttu-id="44a67-138">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44a67-138">Sites.ReadWrite.All</span></span> | <span data-ttu-id="44a67-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="44a67-139">Not supported</span></span> | <span data-ttu-id="44a67-140">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44a67-140">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="44a67-141">message</span><span class="sxs-lookup"><span data-stu-id="44a67-141">message</span></span>](../resources/message.md) | <span data-ttu-id="44a67-142">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="44a67-142">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="44a67-143">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="44a67-143">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="44a67-144">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="44a67-144">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="44a67-145">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="44a67-145">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="44a67-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44a67-146">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="44a67-147">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="44a67-147">Not supported</span></span> | <span data-ttu-id="44a67-148">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44a67-148">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="44a67-149">Usuário</span><span class="sxs-lookup"><span data-stu-id="44a67-149">user</span></span>](../resources/user.md) | <span data-ttu-id="44a67-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="44a67-150">User.Read.All</span></span> | <span data-ttu-id="44a67-151">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="44a67-151">User.Read.All</span></span> | <span data-ttu-id="44a67-152">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="44a67-152">User.Read.All</span></span> |

> <span data-ttu-id="44a67-153">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="44a67-153">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="44a67-154">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="44a67-154">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="44a67-155">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="44a67-155">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="44a67-156">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="44a67-156">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="44a67-157">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="44a67-157">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="44a67-158">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="44a67-158">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="44a67-159">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="44a67-159">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="44a67-160">Isso significa que, por exemplo, você não pode usar os calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="44a67-160">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="44a67-161">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="44a67-161">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="44a67-162">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="44a67-162">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="44a67-163">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="44a67-163">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="44a67-164">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44a67-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44a67-165">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="44a67-165">Optional query parameters</span></span>

<span data-ttu-id="44a67-166">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="44a67-166">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44a67-167">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44a67-167">Request headers</span></span>

| <span data-ttu-id="44a67-168">Nome</span><span class="sxs-lookup"><span data-stu-id="44a67-168">Name</span></span>       | <span data-ttu-id="44a67-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="44a67-169">Type</span></span> | <span data-ttu-id="44a67-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="44a67-170">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="44a67-171">Autorização</span><span class="sxs-lookup"><span data-stu-id="44a67-171">Authorization</span></span>  | <span data-ttu-id="44a67-172">string</span><span class="sxs-lookup"><span data-stu-id="44a67-172">string</span></span>  | <span data-ttu-id="44a67-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44a67-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44a67-175">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44a67-175">Request body</span></span>

<span data-ttu-id="44a67-176">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="44a67-176">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44a67-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="44a67-177">Response</span></span>

<span data-ttu-id="44a67-178">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44a67-178">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44a67-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44a67-179">Example</span></span>

##### <a name="request"></a><span data-ttu-id="44a67-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44a67-180">Request</span></span>

<span data-ttu-id="44a67-181">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44a67-181">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="44a67-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="44a67-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="44a67-183">C#</span><span class="sxs-lookup"><span data-stu-id="44a67-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44a67-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44a67-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44a67-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44a67-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44a67-186">Java</span><span class="sxs-lookup"><span data-stu-id="44a67-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="44a67-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="44a67-187">Response</span></span>

<span data-ttu-id="44a67-188">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44a67-188">Here is an example of the response.</span></span>
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
