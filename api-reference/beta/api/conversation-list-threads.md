---
title: Listar threads
description: Obtenha todos os threads em uma conversa de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 25c54509c40076a220093b1034c545f534ed6eda
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047032"
---
# <a name="list-threads"></a><span data-ttu-id="78881-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="78881-103">List threads</span></span>

<span data-ttu-id="78881-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78881-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78881-105">Obtém todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="78881-105">Get all the threads in a group conversation.</span></span>
<span data-ttu-id="78881-106">Observação: Você também pode [obter todos os threads de um grupo](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="78881-106">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="78881-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="78881-107">Permissions</span></span>
<span data-ttu-id="78881-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78881-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78881-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78881-110">Permission type</span></span>      | <span data-ttu-id="78881-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78881-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78881-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78881-112">Delegated (work or school account)</span></span> | <span data-ttu-id="78881-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78881-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="78881-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78881-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78881-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78881-115">Not supported.</span></span>    |
|<span data-ttu-id="78881-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78881-116">Application</span></span> | <span data-ttu-id="78881-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78881-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78881-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78881-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="78881-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="78881-119">Optional query parameters</span></span>
<span data-ttu-id="78881-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="78881-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="78881-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78881-121">Request headers</span></span>
| <span data-ttu-id="78881-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78881-122">Header</span></span>       | <span data-ttu-id="78881-123">Valor</span><span class="sxs-lookup"><span data-stu-id="78881-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="78881-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="78881-124">Authorization</span></span>  | <span data-ttu-id="78881-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78881-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="78881-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78881-127">Request body</span></span>
<span data-ttu-id="78881-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78881-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78881-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="78881-129">Response</span></span>

<span data-ttu-id="78881-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78881-130">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="78881-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78881-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78881-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78881-132">Request</span></span>
<span data-ttu-id="78881-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78881-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="78881-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="78881-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
```
# <a name="c"></a>[<span data-ttu-id="78881-135">C#</span><span class="sxs-lookup"><span data-stu-id="78881-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78881-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78881-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78881-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78881-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78881-138">Java</span><span class="sxs-lookup"><span data-stu-id="78881-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threads-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="78881-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="78881-139">Response</span></span>
<span data-ttu-id="78881-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78881-140">Here is an example of the response.</span></span> <span data-ttu-id="78881-141">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="78881-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
