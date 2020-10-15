---
title: Listar threads
description: Obtenha todos os threads em uma conversa de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: cade38bd630d84a0b6e550daf7e85b81943b6247
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461444"
---
# <a name="list-threads"></a><span data-ttu-id="036b7-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="036b7-103">List threads</span></span>

<span data-ttu-id="036b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="036b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="036b7-105">Obtém todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="036b7-105">Get all the threads in a group conversation.</span></span>

<span data-ttu-id="036b7-106">Observação: Você também pode [obter todos os threads de um grupo](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="036b7-106">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="036b7-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="036b7-107">Permissions</span></span>
<span data-ttu-id="036b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="036b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="036b7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="036b7-110">Permission type</span></span>      | <span data-ttu-id="036b7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="036b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="036b7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="036b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="036b7-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="036b7-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="036b7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="036b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="036b7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="036b7-115">Not supported.</span></span>    |
|<span data-ttu-id="036b7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="036b7-116">Application</span></span> | <span data-ttu-id="036b7-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="036b7-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="036b7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="036b7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="036b7-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="036b7-119">Optional query parameters</span></span>
<span data-ttu-id="036b7-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="036b7-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="036b7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="036b7-121">Request headers</span></span>
| <span data-ttu-id="036b7-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="036b7-122">Header</span></span>       | <span data-ttu-id="036b7-123">Valor</span><span class="sxs-lookup"><span data-stu-id="036b7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="036b7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="036b7-124">Authorization</span></span>  | <span data-ttu-id="036b7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="036b7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="036b7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="036b7-127">Request body</span></span>
<span data-ttu-id="036b7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="036b7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="036b7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="036b7-129">Response</span></span>

<span data-ttu-id="036b7-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="036b7-130">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="036b7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="036b7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="036b7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="036b7-132">Request</span></span>
<span data-ttu-id="036b7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="036b7-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="036b7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="036b7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
```
# <a name="c"></a>[<span data-ttu-id="036b7-135">C#</span><span class="sxs-lookup"><span data-stu-id="036b7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="036b7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="036b7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="036b7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="036b7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="036b7-138">Java</span><span class="sxs-lookup"><span data-stu-id="036b7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threads-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="036b7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="036b7-139">Response</span></span>
<span data-ttu-id="036b7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="036b7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "lastDeliveredDateTime": "datetime-value",
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
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
