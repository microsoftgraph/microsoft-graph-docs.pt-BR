---
title: Obter conversationMember
description: Recuperar um membro de um chat ou canal.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 05708a121b5cdedecc62c0b23678bf126cfd0662
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436500"
---
# <a name="get-conversationmember"></a><span data-ttu-id="a019f-103">Obter conversationMember</span><span class="sxs-lookup"><span data-stu-id="a019f-103">Get conversationMember</span></span>

<span data-ttu-id="a019f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a019f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a019f-105">Recuperar um [conversationMember](../resources/conversationmember.md) de um [chat](../resources/chat.md) ou [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="a019f-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a019f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a019f-106">Permissions</span></span>

<span data-ttu-id="a019f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a019f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a019f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a019f-109">Permission Type</span></span>|<span data-ttu-id="a019f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a019f-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="a019f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a019f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a019f-112">Para o recurso de **usuário** ou **chat** :</span><span class="sxs-lookup"><span data-stu-id="a019f-112">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="a019f-113">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a019f-113">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="a019f-114">Para o recurso de **canal**:</span><span class="sxs-lookup"><span data-stu-id="a019f-114">For **channel** resource:</span></span><br/><span data-ttu-id="a019f-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a019f-115">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="a019f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a019f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a019f-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a019f-117">Not supported</span></span>|
|<span data-ttu-id="a019f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a019f-118">Application</span></span>| <span data-ttu-id="a019f-119">Para o recurso de **usuário** ou **chat** :</span><span class="sxs-lookup"><span data-stu-id="a019f-119">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="a019f-120">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a019f-120">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="a019f-121">Para o recurso de **canal**:</span><span class="sxs-lookup"><span data-stu-id="a019f-121">For **channel** resource:</span></span><br/><span data-ttu-id="a019f-122">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a019f-122">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="a019f-123">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a019f-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="a019f-124">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="a019f-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="a019f-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a019f-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a019f-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a019f-126">Optional query parameters</span></span>

<span data-ttu-id="a019f-127">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a019f-127">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a019f-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a019f-128">Request headers</span></span>

| <span data-ttu-id="a019f-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a019f-129">Header</span></span>       | <span data-ttu-id="a019f-130">Valor</span><span class="sxs-lookup"><span data-stu-id="a019f-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a019f-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="a019f-131">Authorization</span></span>  | <span data-ttu-id="a019f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a019f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a019f-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a019f-134">Request body</span></span>

<span data-ttu-id="a019f-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a019f-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a019f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a019f-136">Response</span></span>

<span data-ttu-id="a019f-137">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a019f-137">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a019f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a019f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a019f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a019f-139">Request</span></span>

<span data-ttu-id="a019f-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a019f-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a019f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="a019f-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="a019f-142">C#</span><span class="sxs-lookup"><span data-stu-id="a019f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a019f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a019f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a019f-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a019f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a019f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a019f-145">Response</span></span>

<span data-ttu-id="a019f-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a019f-146">Here is an example of the response.</span></span>

><span data-ttu-id="a019f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a019f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "display-name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member get",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
