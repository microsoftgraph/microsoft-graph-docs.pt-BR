---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 4063be8500e67d4630e10d027359774612c0613a
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394443"
---
# <a name="get-subscription"></a><span data-ttu-id="b8baa-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="b8baa-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8baa-104">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="b8baa-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8baa-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8baa-105">Permissions</span></span>

<span data-ttu-id="b8baa-106">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="b8baa-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="b8baa-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8baa-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8baa-108">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="b8baa-108">Supported resource</span></span> | <span data-ttu-id="b8baa-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8baa-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b8baa-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8baa-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8baa-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8baa-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="b8baa-112">callRecord</span><span class="sxs-lookup"><span data-stu-id="b8baa-112">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="b8baa-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8baa-113">Not supported</span></span> | <span data-ttu-id="b8baa-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8baa-114">Not supported</span></span> | <span data-ttu-id="b8baa-115">CallRecords. Read. All</span><span class="sxs-lookup"><span data-stu-id="b8baa-115">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="b8baa-116">contato</span><span class="sxs-lookup"><span data-stu-id="b8baa-116">contact</span></span>](../resources/contact.md) | <span data-ttu-id="b8baa-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b8baa-117">Contacts.Read</span></span> | <span data-ttu-id="b8baa-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b8baa-118">Contacts.Read</span></span> | <span data-ttu-id="b8baa-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b8baa-119">Contacts.Read</span></span> |
|<span data-ttu-id="b8baa-120">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="b8baa-120">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="b8baa-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8baa-121">Not supported</span></span> | <span data-ttu-id="b8baa-122">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8baa-122">Files.ReadWrite</span></span> | <span data-ttu-id="b8baa-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8baa-123">Not supported</span></span> |
|<span data-ttu-id="b8baa-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="b8baa-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="b8baa-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8baa-125">Files.ReadWrite.All</span></span> | <span data-ttu-id="b8baa-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8baa-126">Not supported</span></span> | <span data-ttu-id="b8baa-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8baa-127">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="b8baa-128">evento</span><span class="sxs-lookup"><span data-stu-id="b8baa-128">event</span></span>](../resources/event.md) | <span data-ttu-id="b8baa-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b8baa-129">Calendars.Read</span></span> | <span data-ttu-id="b8baa-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b8baa-130">Calendars.Read</span></span> | <span data-ttu-id="b8baa-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b8baa-131">Calendars.Read</span></span> |
|[<span data-ttu-id="b8baa-132">grupo</span><span class="sxs-lookup"><span data-stu-id="b8baa-132">group</span></span>](../resources/group.md) | <span data-ttu-id="b8baa-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8baa-133">Group.Read.All</span></span> | <span data-ttu-id="b8baa-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8baa-134">Not supported</span></span> | <span data-ttu-id="b8baa-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8baa-135">Group.Read.All</span></span> |
|[<span data-ttu-id="b8baa-136">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="b8baa-136">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="b8baa-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8baa-137">Group.Read.All</span></span> | <span data-ttu-id="b8baa-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8baa-138">Not supported</span></span> | <span data-ttu-id="b8baa-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8baa-139">Not supported</span></span> |
|[<span data-ttu-id="b8baa-140">list</span><span class="sxs-lookup"><span data-stu-id="b8baa-140">list</span></span>](../resources/list.md) | <span data-ttu-id="b8baa-141">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8baa-141">Sites.ReadWrite.All</span></span> | <span data-ttu-id="b8baa-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8baa-142">Not supported</span></span> | <span data-ttu-id="b8baa-143">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8baa-143">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="b8baa-144">message</span><span class="sxs-lookup"><span data-stu-id="b8baa-144">message</span></span>](../resources/message.md) | <span data-ttu-id="b8baa-145">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b8baa-145">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="b8baa-146">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b8baa-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="b8baa-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b8baa-147">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="b8baa-148">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="b8baa-148">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="b8baa-149">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8baa-149">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="b8baa-150">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8baa-150">Not supported</span></span> | <span data-ttu-id="b8baa-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8baa-151">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="b8baa-152">Usuário</span><span class="sxs-lookup"><span data-stu-id="b8baa-152">user</span></span>](../resources/user.md) | <span data-ttu-id="b8baa-153">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8baa-153">User.Read.All</span></span> | <span data-ttu-id="b8baa-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8baa-154">User.Read.All</span></span> | <span data-ttu-id="b8baa-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8baa-155">User.Read.All</span></span> |

> <span data-ttu-id="b8baa-156">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="b8baa-156">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="b8baa-157">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="b8baa-157">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="b8baa-158">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="b8baa-158">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="b8baa-159">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="b8baa-159">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="b8baa-160">As notificações são enviadas pelos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outros objetos driveItem na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="b8baa-160">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="b8baa-161">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="b8baa-161">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="b8baa-162">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="b8baa-162">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="b8baa-163">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="b8baa-163">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="b8baa-164">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="b8baa-164">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="b8baa-165">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="b8baa-165">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="b8baa-166">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="b8baa-166">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="b8baa-167">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8baa-167">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8baa-168">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8baa-168">Optional query parameters</span></span>

<span data-ttu-id="b8baa-169">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8baa-169">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8baa-170">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8baa-170">Request headers</span></span>

| <span data-ttu-id="b8baa-171">Nome</span><span class="sxs-lookup"><span data-stu-id="b8baa-171">Name</span></span>       | <span data-ttu-id="b8baa-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8baa-172">Type</span></span> | <span data-ttu-id="b8baa-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8baa-173">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="b8baa-174">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8baa-174">Authorization</span></span>  | <span data-ttu-id="b8baa-175">string</span><span class="sxs-lookup"><span data-stu-id="b8baa-175">string</span></span>  | <span data-ttu-id="b8baa-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8baa-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8baa-178">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8baa-178">Request body</span></span>

<span data-ttu-id="b8baa-179">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8baa-179">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8baa-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8baa-180">Response</span></span>

<span data-ttu-id="b8baa-181">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8baa-181">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8baa-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8baa-182">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b8baa-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8baa-183">Request</span></span>

<span data-ttu-id="b8baa-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8baa-184">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b8baa-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8baa-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="b8baa-186">C#</span><span class="sxs-lookup"><span data-stu-id="b8baa-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8baa-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8baa-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8baa-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8baa-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b8baa-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8baa-189">Response</span></span>

<span data-ttu-id="b8baa-190">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8baa-190">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
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
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
