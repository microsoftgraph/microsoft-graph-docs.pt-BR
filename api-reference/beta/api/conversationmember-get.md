---
title: Obter conversationMember
description: Recuperar um membro de um bate-papo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 58087819631a9d86464d17307755d6add0af4d73
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536103"
---
# <a name="get-conversationmember"></a><span data-ttu-id="af010-103">Obter conversationMember</span><span class="sxs-lookup"><span data-stu-id="af010-103">Get conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af010-104">Recuperar um [conversationMember](../resources/conversationmember.md) de um [bate-papo](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="af010-104">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="af010-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="af010-105">Permissions</span></span>

<span data-ttu-id="af010-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af010-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af010-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af010-108">Permission Type</span></span>|<span data-ttu-id="af010-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af010-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="af010-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af010-110">Delegated (work or school account)</span></span>|<span data-ttu-id="af010-111">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af010-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="af010-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af010-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af010-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="af010-113">Not supported</span></span>|
|<span data-ttu-id="af010-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af010-114">Application</span></span> |<span data-ttu-id="af010-115">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af010-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af010-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af010-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="af010-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="af010-117">Optional query parameters</span></span>

<span data-ttu-id="af010-118">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="af010-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af010-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af010-119">Request headers</span></span>

| <span data-ttu-id="af010-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af010-120">Header</span></span>       | <span data-ttu-id="af010-121">Valor</span><span class="sxs-lookup"><span data-stu-id="af010-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="af010-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="af010-122">Authorization</span></span>  | <span data-ttu-id="af010-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af010-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="af010-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af010-125">Request body</span></span>

<span data-ttu-id="af010-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af010-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af010-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="af010-127">Response</span></span>

<span data-ttu-id="af010-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af010-128">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af010-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af010-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="af010-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af010-130">Request</span></span>

<span data-ttu-id="af010-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af010-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="af010-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="af010-132">Response</span></span>

<span data-ttu-id="af010-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af010-133">Here is an example of the response.</span></span> 

><span data-ttu-id="af010-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af010-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="af010-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="af010-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="af010-137">C#</span><span class="sxs-lookup"><span data-stu-id="af010-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_conversation_member-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="af010-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="af010-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_conversation_member-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/conversationmember-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/conversationmember-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->