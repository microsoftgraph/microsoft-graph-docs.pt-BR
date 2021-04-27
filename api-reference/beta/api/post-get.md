---
title: Obter postagem
description: 'Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado. Você pode especificar o pai '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a29797c1e272b34eedf5534411ea37598dded5d8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049160"
---
# <a name="get-post"></a><span data-ttu-id="c94d7-104">Obter postagem</span><span class="sxs-lookup"><span data-stu-id="c94d7-104">Get post</span></span>

<span data-ttu-id="c94d7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c94d7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c94d7-p102">Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="c94d7-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="c94d7-108">Como o **recurso post** dá suporte a [extensões,](/graph/extensibility-overview)você também pode usar a operação para obter propriedades personalizadas e dados de extensão em uma `GET` instância **de** postagem.</span><span class="sxs-lookup"><span data-stu-id="c94d7-108">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="c94d7-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c94d7-109">Permissions</span></span>
<span data-ttu-id="c94d7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c94d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c94d7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c94d7-112">Permission type</span></span>      | <span data-ttu-id="c94d7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c94d7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c94d7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c94d7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c94d7-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c94d7-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c94d7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c94d7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c94d7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c94d7-117">Not supported.</span></span>    |
|<span data-ttu-id="c94d7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c94d7-118">Application</span></span> | <span data-ttu-id="c94d7-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c94d7-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c94d7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c94d7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c94d7-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c94d7-121">Optional query parameters</span></span>
<span data-ttu-id="c94d7-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c94d7-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c94d7-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c94d7-123">Request headers</span></span>
| <span data-ttu-id="c94d7-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c94d7-124">Header</span></span>       | <span data-ttu-id="c94d7-125">Valor</span><span class="sxs-lookup"><span data-stu-id="c94d7-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c94d7-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c94d7-126">Authorization</span></span>  | <span data-ttu-id="c94d7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c94d7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c94d7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c94d7-129">Request body</span></span>
<span data-ttu-id="c94d7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c94d7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c94d7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c94d7-131">Response</span></span>

<span data-ttu-id="c94d7-132">Se bem sucedido, este método retorna o código de resposta `200 OK` e o objeto [post](../resources/post.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c94d7-132">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c94d7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c94d7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c94d7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c94d7-134">Request</span></span>
<span data-ttu-id="c94d7-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c94d7-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c94d7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c94d7-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts/AQMkADgAAAIJbQAAAA==
```
# <a name="c"></a>[<span data-ttu-id="c94d7-137">C#</span><span class="sxs-lookup"><span data-stu-id="c94d7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c94d7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c94d7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c94d7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c94d7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c94d7-140">Java</span><span class="sxs-lookup"><span data-stu-id="c94d7-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c94d7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c94d7-141">Response</span></span>
<span data-ttu-id="c94d7-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c94d7-142">Here is an example of the response.</span></span> <span data-ttu-id="c94d7-143">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c94d7-143">Note: The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="c94d7-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="c94d7-144">See also</span></span>

- [<span data-ttu-id="c94d7-145">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="c94d7-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c94d7-146">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="c94d7-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="c94d7-147">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="c94d7-147">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
