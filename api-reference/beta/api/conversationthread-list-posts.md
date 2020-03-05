---
title: Listar postagens
description: 'Obtenha as postagens do thread especificado. Você pode especificar a conversa pai e o thread ou, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b7df6ffb23e812dc9f950a976c66ce8a10a8a1b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436318"
---
# <a name="list-posts"></a><span data-ttu-id="6fb7b-104">Listar postagens</span><span class="sxs-lookup"><span data-stu-id="6fb7b-104">List posts</span></span>

<span data-ttu-id="6fb7b-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6fb7b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fb7b-p102">Obtenha as postagens do thread especificado. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="6fb7b-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fb7b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6fb7b-108">Permissions</span></span>
<span data-ttu-id="6fb7b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fb7b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fb7b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fb7b-111">Permission type</span></span>      | <span data-ttu-id="6fb7b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6fb7b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fb7b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fb7b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6fb7b-114">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="6fb7b-114">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="6fb7b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fb7b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fb7b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fb7b-116">Not supported.</span></span>    |
|<span data-ttu-id="6fb7b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fb7b-117">Application</span></span> | <span data-ttu-id="6fb7b-118">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="6fb7b-118">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fb7b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fb7b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="6fb7b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6fb7b-120">Optional query parameters</span></span>
<span data-ttu-id="6fb7b-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6fb7b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6fb7b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fb7b-122">Request headers</span></span>
| <span data-ttu-id="6fb7b-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6fb7b-123">Header</span></span>       | <span data-ttu-id="6fb7b-124">Valor</span><span class="sxs-lookup"><span data-stu-id="6fb7b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6fb7b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fb7b-125">Authorization</span></span>  | <span data-ttu-id="6fb7b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fb7b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6fb7b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fb7b-128">Request body</span></span>
<span data-ttu-id="6fb7b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6fb7b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fb7b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fb7b-130">Response</span></span>

<span data-ttu-id="6fb7b-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Post](../resources/post.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fb7b-131">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6fb7b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fb7b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6fb7b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fb7b-133">Request</span></span>
<span data-ttu-id="6fb7b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fb7b-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6fb7b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fb7b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts
```
# <a name="c"></a>[<span data-ttu-id="6fb7b-136">C#</span><span class="sxs-lookup"><span data-stu-id="6fb7b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-posts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fb7b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fb7b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-posts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fb7b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fb7b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-posts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6fb7b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fb7b-139">Response</span></span>
<span data-ttu-id="6fb7b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6fb7b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts",
    "value":[
        {
            "@odata.etag":"W/\"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK\"",
            "id":"AQMkADgAAAIJbQAAAA==",
            "createdDateTime":"2018-01-11T17:36:17Z",
            "lastModifiedDateTime":"2018-01-11T17:36:17Z",
            "importance": "normal",
            "changeKey":"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK",
            "categories":[

            ],
            "receivedDateTime":"2018-01-11T17:36:17Z",
            "hasAttachments":false,
            "body":{
                "contentType":"html",
                "content":"<html><body></body></html>"
            },
            "from":{
                "emailAddress":{
                    "name":"Marketing",
                    "address":"Marketing@M365B489948.onmicrosoft.com"
                }
            },
            "sender":{
                "emailAddress":{
                    "name":"Marketing",
                    "address":"Marketing@M365B489948.onmicrosoft.com"
                }
            }
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
