---
title: Obter conversation
description: Obter um objeto conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2d75fcb6998fc9dfe059c30d984b08f3403f9007
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323609"
---
# <a name="get-conversation"></a><span data-ttu-id="dea5a-103">Obter conversation</span><span class="sxs-lookup"><span data-stu-id="dea5a-103">Get conversation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dea5a-104">Obter um objeto [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="dea5a-104">Get a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dea5a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dea5a-105">Permissions</span></span>
<span data-ttu-id="dea5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dea5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dea5a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dea5a-108">Permission type</span></span>      | <span data-ttu-id="dea5a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dea5a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dea5a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dea5a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dea5a-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dea5a-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dea5a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dea5a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dea5a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dea5a-113">Not supported.</span></span>    |
|<span data-ttu-id="dea5a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dea5a-114">Application</span></span> | <span data-ttu-id="dea5a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dea5a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dea5a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dea5a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dea5a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dea5a-117">Optional query parameters</span></span>
<span data-ttu-id="dea5a-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dea5a-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dea5a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dea5a-119">Request headers</span></span>
| <span data-ttu-id="dea5a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dea5a-120">Header</span></span>       | <span data-ttu-id="dea5a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dea5a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dea5a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dea5a-122">Authorization</span></span>  | <span data-ttu-id="dea5a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dea5a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dea5a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dea5a-125">Request body</span></span>
<span data-ttu-id="dea5a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dea5a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dea5a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="dea5a-127">Response</span></span>
<span data-ttu-id="dea5a-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dea5a-128">If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dea5a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dea5a-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="dea5a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dea5a-130">Request</span></span>
<span data-ttu-id="dea5a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dea5a-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dea5a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="dea5a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_conversation"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dea5a-133">C#</span><span class="sxs-lookup"><span data-stu-id="dea5a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dea5a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dea5a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dea5a-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dea5a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dea5a-136">Java</span><span class="sxs-lookup"><span data-stu-id="dea5a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dea5a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="dea5a-137">Response</span></span>
<span data-ttu-id="dea5a-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dea5a-138">The following is an example of the response.</span></span>
><span data-ttu-id="dea5a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dea5a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 644

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
