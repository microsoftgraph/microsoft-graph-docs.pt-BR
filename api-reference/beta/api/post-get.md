---
title: Obter postagem
description: 'Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado. Você pode especificar tanto o pai '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ca2bdf89d889713bd5302a601535ec5ecbd6122a
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314112"
---
# <a name="get-post"></a><span data-ttu-id="904e1-104">Obter postagem</span><span class="sxs-lookup"><span data-stu-id="904e1-104">Get post</span></span>

<span data-ttu-id="904e1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="904e1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="904e1-p102">Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="904e1-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="904e1-108">Como o recurso **post** dá suporte a [extensões](/graph/extensibility-overview), você também pode usar a `GET` operação para obter propriedades personalizadas e dados de extensão em uma instância de **post** .</span><span class="sxs-lookup"><span data-stu-id="904e1-108">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="904e1-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="904e1-109">Permissions</span></span>
<span data-ttu-id="904e1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="904e1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="904e1-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="904e1-112">Permission type</span></span>      | <span data-ttu-id="904e1-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="904e1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="904e1-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="904e1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="904e1-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="904e1-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="904e1-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="904e1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="904e1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="904e1-117">Not supported.</span></span>    |
|<span data-ttu-id="904e1-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="904e1-118">Application</span></span> | <span data-ttu-id="904e1-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="904e1-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="904e1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="904e1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="904e1-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="904e1-121">Optional query parameters</span></span>
<span data-ttu-id="904e1-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="904e1-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="904e1-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="904e1-123">Request headers</span></span>
| <span data-ttu-id="904e1-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="904e1-124">Header</span></span>       | <span data-ttu-id="904e1-125">Valor</span><span class="sxs-lookup"><span data-stu-id="904e1-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="904e1-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="904e1-126">Authorization</span></span>  | <span data-ttu-id="904e1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="904e1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="904e1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="904e1-129">Request body</span></span>
<span data-ttu-id="904e1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="904e1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="904e1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="904e1-131">Response</span></span>

<span data-ttu-id="904e1-132">Se bem sucedido, este método retorna o código de resposta `200 OK` e o objeto [post](../resources/post.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="904e1-132">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="904e1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="904e1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="904e1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="904e1-134">Request</span></span>
<span data-ttu-id="904e1-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="904e1-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="904e1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="904e1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts/AQMkADgAAAIJbQAAAA==
```
# <a name="c"></a>[<span data-ttu-id="904e1-137">C#</span><span class="sxs-lookup"><span data-stu-id="904e1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="904e1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="904e1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="904e1-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="904e1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="904e1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="904e1-140">Response</span></span>
<span data-ttu-id="904e1-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="904e1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts/$entity",
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
```

## <a name="see-also"></a><span data-ttu-id="904e1-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="904e1-144">See also</span></span>

- [<span data-ttu-id="904e1-145">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="904e1-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="904e1-146">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="904e1-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="904e1-147">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="904e1-147">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->