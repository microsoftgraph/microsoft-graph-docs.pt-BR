---
title: Obter conversationMember
description: Recuperar um membro de um chat ou canal.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bd1d7cc150ade0a9c50083d9b9833ae682599b95
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439810"
---
# <a name="get-conversationmember"></a><span data-ttu-id="ceadc-103">Obter conversationMember</span><span class="sxs-lookup"><span data-stu-id="ceadc-103">Get conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ceadc-104">Recuperar um [conversationMember](../resources/conversationmember.md) de um [chat](../resources/chat.md) ou [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="ceadc-104">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ceadc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ceadc-105">Permissions</span></span>

<span data-ttu-id="ceadc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceadc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceadc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ceadc-108">Permission Type</span></span>|<span data-ttu-id="ceadc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ceadc-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="ceadc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ceadc-110">Delegated (work or school account)</span></span>|<span data-ttu-id="ceadc-111">Para o recurso de **usuário** ou **chat** :</span><span class="sxs-lookup"><span data-stu-id="ceadc-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="ceadc-112">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ceadc-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="ceadc-113">Para o recurso de **canal**:</span><span class="sxs-lookup"><span data-stu-id="ceadc-113">For **channel** resource:</span></span><br/><span data-ttu-id="ceadc-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceadc-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="ceadc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ceadc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ceadc-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ceadc-116">Not supported</span></span>|
|<span data-ttu-id="ceadc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ceadc-117">Application</span></span>| <span data-ttu-id="ceadc-118">Para o recurso de **usuário** ou **chat** :</span><span class="sxs-lookup"><span data-stu-id="ceadc-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="ceadc-119">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceadc-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="ceadc-120">Para o recurso de **canal**:</span><span class="sxs-lookup"><span data-stu-id="ceadc-120">For **channel** resource:</span></span><br/><span data-ttu-id="ceadc-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceadc-121">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="ceadc-122">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ceadc-122">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="ceadc-123">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="ceadc-123">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="ceadc-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ceadc-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ceadc-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ceadc-125">Optional query parameters</span></span>

<span data-ttu-id="ceadc-126">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ceadc-126">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ceadc-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ceadc-127">Request headers</span></span>

| <span data-ttu-id="ceadc-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ceadc-128">Header</span></span>       | <span data-ttu-id="ceadc-129">Valor</span><span class="sxs-lookup"><span data-stu-id="ceadc-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ceadc-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="ceadc-130">Authorization</span></span>  | <span data-ttu-id="ceadc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ceadc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ceadc-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ceadc-133">Request body</span></span>

<span data-ttu-id="ceadc-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ceadc-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ceadc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceadc-135">Response</span></span>

<span data-ttu-id="ceadc-136">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ceadc-136">If successful, this method returns a `200 OK` response code and a [channel](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceadc-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ceadc-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="ceadc-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ceadc-138">Request</span></span>

<span data-ttu-id="ceadc-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ceadc-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ceadc-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ceadc-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ceadc-141">C#</span><span class="sxs-lookup"><span data-stu-id="ceadc-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ceadc-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ceadc-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ceadc-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ceadc-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ceadc-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceadc-144">Response</span></span>

<span data-ttu-id="ceadc-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ceadc-145">Here is an example of the response.</span></span>

><span data-ttu-id="ceadc-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ceadc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
