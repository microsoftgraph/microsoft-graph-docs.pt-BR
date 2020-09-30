---
title: Listar threads
description: Obtenha todos os threads em uma conversa de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c72e7f29153588a3c1ecc073d5da728ef020834e
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312908"
---
# <a name="list-threads"></a><span data-ttu-id="a5a37-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="a5a37-103">List threads</span></span>

<span data-ttu-id="a5a37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5a37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5a37-105">Obtém todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="a5a37-105">Get all the threads in a group conversation.</span></span>
<span data-ttu-id="a5a37-106">Observação: Você também pode [obter todos os threads de um grupo](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="a5a37-106">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a5a37-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5a37-107">Permissions</span></span>
<span data-ttu-id="a5a37-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5a37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5a37-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5a37-110">Permission type</span></span>      | <span data-ttu-id="a5a37-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5a37-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5a37-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5a37-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a5a37-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5a37-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5a37-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5a37-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5a37-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5a37-115">Not supported.</span></span>    |
|<span data-ttu-id="a5a37-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5a37-116">Application</span></span> | <span data-ttu-id="a5a37-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5a37-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5a37-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5a37-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a5a37-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a5a37-119">Optional query parameters</span></span>
<span data-ttu-id="a5a37-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a5a37-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a5a37-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5a37-121">Request headers</span></span>
| <span data-ttu-id="a5a37-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5a37-122">Header</span></span>       | <span data-ttu-id="a5a37-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a5a37-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5a37-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5a37-124">Authorization</span></span>  | <span data-ttu-id="a5a37-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5a37-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5a37-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5a37-127">Request body</span></span>
<span data-ttu-id="a5a37-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5a37-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5a37-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5a37-129">Response</span></span>

<span data-ttu-id="a5a37-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5a37-130">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a5a37-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5a37-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5a37-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5a37-132">Request</span></span>
<span data-ttu-id="a5a37-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5a37-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5a37-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5a37-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
```
# <a name="c"></a>[<span data-ttu-id="a5a37-135">C#</span><span class="sxs-lookup"><span data-stu-id="a5a37-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5a37-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5a37-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5a37-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5a37-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a5a37-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5a37-138">Response</span></span>
<span data-ttu-id="a5a37-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5a37-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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