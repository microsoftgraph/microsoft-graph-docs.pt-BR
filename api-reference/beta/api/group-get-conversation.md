---
title: Obter conversation
description: Obter um objeto conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7ab1811f1e3113174e757f56cc2d365265a4ede9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593614"
---
# <a name="get-conversation"></a><span data-ttu-id="cbc40-103">Obter conversation</span><span class="sxs-lookup"><span data-stu-id="cbc40-103">Get conversation</span></span>
<span data-ttu-id="cbc40-104">Obter um objeto [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="cbc40-104">Get a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbc40-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbc40-105">Permissions</span></span>
<span data-ttu-id="cbc40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbc40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbc40-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbc40-108">Permission type</span></span>      | <span data-ttu-id="cbc40-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbc40-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbc40-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbc40-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cbc40-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbc40-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cbc40-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbc40-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbc40-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbc40-113">Not supported.</span></span>    |
|<span data-ttu-id="cbc40-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbc40-114">Application</span></span> | <span data-ttu-id="cbc40-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbc40-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbc40-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbc40-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cbc40-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cbc40-117">Optional query parameters</span></span>
<span data-ttu-id="cbc40-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cbc40-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cbc40-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbc40-119">Request headers</span></span>
| <span data-ttu-id="cbc40-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cbc40-120">Header</span></span>       | <span data-ttu-id="cbc40-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cbc40-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cbc40-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbc40-122">Authorization</span></span>  | <span data-ttu-id="cbc40-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbc40-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cbc40-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbc40-125">Request body</span></span>
<span data-ttu-id="cbc40-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cbc40-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbc40-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbc40-127">Response</span></span>
<span data-ttu-id="cbc40-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbc40-128">If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbc40-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbc40-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cbc40-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbc40-130">Request</span></span>
<span data-ttu-id="cbc40-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbc40-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "get_group_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="cbc40-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbc40-132">Response</span></span>
<span data-ttu-id="cbc40-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cbc40-133">The following is an example of the response.</span></span>
><span data-ttu-id="cbc40-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbc40-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cbc40-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="cbc40-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cbc40-137">Basic</span><span class="sxs-lookup"><span data-stu-id="cbc40-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_conversation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cbc40-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cbc40-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_conversation-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-get-conversation.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-get-conversation.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
