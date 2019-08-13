---
title: Obter postagem
description: 'Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado. Você pode especificar tanto o pai '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1d6a03ea15fdcf3cfec71258b0a8ea19e6a697d9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375734"
---
# <a name="get-post"></a><span data-ttu-id="7a18a-104">Obter postagem</span><span class="sxs-lookup"><span data-stu-id="7a18a-104">Get post</span></span>

<span data-ttu-id="7a18a-p102">Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="7a18a-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="7a18a-107">Como o recurso **post** dá suporte a [extensões](/graph/extensibility-overview), você também pode `GET` usar a operação para obter propriedades personalizadas e dados de extensão em uma instância de **post** .</span><span class="sxs-lookup"><span data-stu-id="7a18a-107">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a18a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a18a-108">Permissions</span></span>
<span data-ttu-id="7a18a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a18a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a18a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a18a-111">Permission type</span></span>      | <span data-ttu-id="7a18a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a18a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a18a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a18a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7a18a-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a18a-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7a18a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a18a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a18a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a18a-116">Not supported.</span></span>    |
|<span data-ttu-id="7a18a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a18a-117">Application</span></span> | <span data-ttu-id="7a18a-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a18a-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a18a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a18a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7a18a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7a18a-120">Optional query parameters</span></span>
<span data-ttu-id="7a18a-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7a18a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7a18a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a18a-122">Request headers</span></span>
| <span data-ttu-id="7a18a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a18a-123">Header</span></span>       | <span data-ttu-id="7a18a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7a18a-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7a18a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a18a-125">Authorization</span></span>  | <span data-ttu-id="7a18a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a18a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7a18a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a18a-128">Request body</span></span>
<span data-ttu-id="7a18a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a18a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a18a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a18a-130">Response</span></span>

<span data-ttu-id="7a18a-131">Se bem sucedido, este método retorna o código de resposta `200 OK` e o objeto [post](../resources/post.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a18a-131">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7a18a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a18a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a18a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a18a-133">Request</span></span>
<span data-ttu-id="7a18a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a18a-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7a18a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a18a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a18a-136">C#</span><span class="sxs-lookup"><span data-stu-id="7a18a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a18a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a18a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a18a-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7a18a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7a18a-139">Java</span><span class="sxs-lookup"><span data-stu-id="7a18a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7a18a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a18a-140">Response</span></span>
<span data-ttu-id="7a18a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a18a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 414

{
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "receivedDateTime": "datetime-value",
  "hasAttachments": true,
  "from": {
    "emailAddress": {
      "name": "name-value",
      "address": "address-value"
    }
  },
  "sender": {
    "emailAddress": {
      "name": "name-value",
      "address": "address-value"
    }
  }
}
```

## <a name="see-also"></a><span data-ttu-id="7a18a-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="7a18a-144">See also</span></span>

- [<span data-ttu-id="7a18a-145">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="7a18a-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7a18a-146">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="7a18a-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
