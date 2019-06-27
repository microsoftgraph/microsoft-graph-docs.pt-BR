---
title: Obter postagem
description: 'Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado. Você pode especificar tanto o pai '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: db98d6bdda0450ac98844e7cc3dcb1b9f7f4be3a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268219"
---
# <a name="get-post"></a><span data-ttu-id="c1c59-104">Obter postagem</span><span class="sxs-lookup"><span data-stu-id="c1c59-104">Get post</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1c59-p102">Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="c1c59-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="c1c59-107">Como o recurso **post** dá suporte a [extensões](/graph/extensibility-overview), você também pode `GET` usar a operação para obter propriedades personalizadas e dados de extensão em uma instância de **post** .</span><span class="sxs-lookup"><span data-stu-id="c1c59-107">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1c59-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c1c59-108">Permissions</span></span>
<span data-ttu-id="c1c59-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1c59-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1c59-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1c59-111">Permission type</span></span>      | <span data-ttu-id="c1c59-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c1c59-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1c59-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1c59-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c1c59-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1c59-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c1c59-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1c59-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1c59-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1c59-116">Not supported.</span></span>    |
|<span data-ttu-id="c1c59-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1c59-117">Application</span></span> | <span data-ttu-id="c1c59-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1c59-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1c59-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1c59-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c1c59-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c1c59-120">Optional query parameters</span></span>
<span data-ttu-id="c1c59-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c1c59-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c1c59-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1c59-122">Request headers</span></span>
| <span data-ttu-id="c1c59-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c1c59-123">Header</span></span>       | <span data-ttu-id="c1c59-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c1c59-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c1c59-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1c59-125">Authorization</span></span>  | <span data-ttu-id="c1c59-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1c59-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1c59-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1c59-128">Request body</span></span>
<span data-ttu-id="c1c59-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c1c59-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1c59-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1c59-130">Response</span></span>

<span data-ttu-id="c1c59-131">Se bem sucedido, este método retorna o código de resposta `200 OK` e o objeto [post](../resources/post.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1c59-131">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c1c59-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1c59-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1c59-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1c59-133">Request</span></span>
<span data-ttu-id="c1c59-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1c59-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts/AQMkADgAAAIJbQAAAA==
```
##### <a name="response"></a><span data-ttu-id="c1c59-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1c59-135">Response</span></span>
<span data-ttu-id="c1c59-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1c59-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c1c59-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c1c59-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c1c59-140">C#</span><span class="sxs-lookup"><span data-stu-id="c1c59-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1c59-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="c1c59-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_post-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c1c59-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c1c59-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_post-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="c1c59-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="c1c59-143">See also</span></span>

- [<span data-ttu-id="c1c59-144">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="c1c59-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c1c59-145">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="c1c59-145">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="c1c59-146">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="c1c59-146">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/post-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/post-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/post-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
