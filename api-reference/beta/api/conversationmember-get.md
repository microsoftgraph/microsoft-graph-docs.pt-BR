---
title: Obter conversationMember
description: Recuperar um membro de um bate-papo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 3b9fddad9b3378b5e4e6df3fd571b070d71900e3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261121"
---
# <a name="get-conversationmember"></a><span data-ttu-id="786ab-103">Obter conversationMember</span><span class="sxs-lookup"><span data-stu-id="786ab-103">Get conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="786ab-104">Recuperar um [conversationMember](../resources/conversationmember.md) de um [bate-papo](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="786ab-104">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="786ab-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="786ab-105">Permissions</span></span>

<span data-ttu-id="786ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="786ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="786ab-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="786ab-108">Permission Type</span></span>|<span data-ttu-id="786ab-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="786ab-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="786ab-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="786ab-110">Delegated (work or school account)</span></span>|<span data-ttu-id="786ab-111">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="786ab-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="786ab-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="786ab-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="786ab-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="786ab-113">Not supported</span></span>|
|<span data-ttu-id="786ab-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="786ab-114">Application</span></span> |<span data-ttu-id="786ab-115">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="786ab-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="786ab-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="786ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="786ab-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="786ab-117">Optional query parameters</span></span>

<span data-ttu-id="786ab-118">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="786ab-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="786ab-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="786ab-119">Request headers</span></span>

| <span data-ttu-id="786ab-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="786ab-120">Header</span></span>       | <span data-ttu-id="786ab-121">Valor</span><span class="sxs-lookup"><span data-stu-id="786ab-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="786ab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="786ab-122">Authorization</span></span>  | <span data-ttu-id="786ab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="786ab-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="786ab-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="786ab-125">Request body</span></span>

<span data-ttu-id="786ab-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="786ab-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="786ab-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="786ab-127">Response</span></span>

<span data-ttu-id="786ab-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="786ab-128">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="786ab-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="786ab-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="786ab-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="786ab-130">Request</span></span>

<span data-ttu-id="786ab-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="786ab-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="786ab-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="786ab-132">Response</span></span>

<span data-ttu-id="786ab-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="786ab-133">Here is an example of the response.</span></span> 

><span data-ttu-id="786ab-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="786ab-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="786ab-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="786ab-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="786ab-137">C#</span><span class="sxs-lookup"><span data-stu-id="786ab-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_conversation_member-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="786ab-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="786ab-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_conversation_member-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="786ab-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="786ab-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_conversation_member-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/conversationmember-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/conversationmember-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/conversationmember-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
