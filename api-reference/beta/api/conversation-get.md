---
title: Obter conversation
description: Recupera as propriedades e os relacionamentos do objeto conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 73f36ba54dc057d7cee7fc9f10138896e646aaba
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312033"
---
# <a name="get-conversation"></a><span data-ttu-id="9a58c-103">Obter conversa</span><span class="sxs-lookup"><span data-stu-id="9a58c-103">Get conversation</span></span>

<span data-ttu-id="9a58c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a58c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a58c-105">Recupera as propriedades e os relacionamentos do objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="9a58c-105">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a58c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a58c-106">Permissions</span></span>
<span data-ttu-id="9a58c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a58c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a58c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a58c-109">Permission type</span></span>      | <span data-ttu-id="9a58c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a58c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a58c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a58c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a58c-112">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="9a58c-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="9a58c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a58c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a58c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a58c-114">Not supported.</span></span>    |
|<span data-ttu-id="9a58c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a58c-115">Application</span></span> | <span data-ttu-id="9a58c-116">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="9a58c-116">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a58c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a58c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="9a58c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9a58c-118">Optional query parameters</span></span>
<span data-ttu-id="9a58c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9a58c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9a58c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a58c-120">Request headers</span></span>
| <span data-ttu-id="9a58c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a58c-121">Header</span></span>       | <span data-ttu-id="9a58c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9a58c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9a58c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a58c-123">Authorization</span></span>  | <span data-ttu-id="9a58c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a58c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a58c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a58c-126">Request body</span></span>
<span data-ttu-id="9a58c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a58c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a58c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a58c-128">Response</span></span>

<span data-ttu-id="9a58c-129">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a58c-129">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a58c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a58c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a58c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a58c-131">Request</span></span>
<span data-ttu-id="9a58c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a58c-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a58c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a58c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
# <a name="c"></a>[<span data-ttu-id="9a58c-134">C#</span><span class="sxs-lookup"><span data-stu-id="9a58c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a58c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a58c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a58c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a58c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9a58c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a58c-137">Response</span></span>
<span data-ttu-id="9a58c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a58c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
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