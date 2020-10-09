---
title: Obter postagem
description: 'Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado. Você pode especificar tanto o pai '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 56c04601808d474e39440ebdce00cc40eec2e569
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405901"
---
# <a name="get-post"></a><span data-ttu-id="14ae6-104">Obter postagem</span><span class="sxs-lookup"><span data-stu-id="14ae6-104">Get post</span></span>

<span data-ttu-id="14ae6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14ae6-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14ae6-p102">Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="14ae6-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="14ae6-108">Como o recurso **post** dá suporte a [extensões](/graph/extensibility-overview), você também pode usar a `GET` operação para obter propriedades personalizadas e dados de extensão em uma instância de **post** .</span><span class="sxs-lookup"><span data-stu-id="14ae6-108">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="14ae6-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="14ae6-109">Permissions</span></span>
<span data-ttu-id="14ae6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14ae6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14ae6-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14ae6-112">Permission type</span></span>      | <span data-ttu-id="14ae6-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14ae6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14ae6-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14ae6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="14ae6-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14ae6-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="14ae6-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14ae6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14ae6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14ae6-117">Not supported.</span></span>    |
|<span data-ttu-id="14ae6-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14ae6-118">Application</span></span> | <span data-ttu-id="14ae6-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14ae6-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14ae6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14ae6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="14ae6-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="14ae6-121">Optional query parameters</span></span>
<span data-ttu-id="14ae6-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="14ae6-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="14ae6-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14ae6-123">Request headers</span></span>
| <span data-ttu-id="14ae6-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14ae6-124">Header</span></span>       | <span data-ttu-id="14ae6-125">Valor</span><span class="sxs-lookup"><span data-stu-id="14ae6-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="14ae6-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="14ae6-126">Authorization</span></span>  | <span data-ttu-id="14ae6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14ae6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="14ae6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14ae6-129">Request body</span></span>
<span data-ttu-id="14ae6-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14ae6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14ae6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="14ae6-131">Response</span></span>

<span data-ttu-id="14ae6-132">Se bem sucedido, este método retorna o código de resposta `200 OK` e o objeto [post](../resources/post.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14ae6-132">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14ae6-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14ae6-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14ae6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14ae6-134">Request</span></span>
<span data-ttu-id="14ae6-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14ae6-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14ae6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="14ae6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
# <a name="c"></a>[<span data-ttu-id="14ae6-137">C#</span><span class="sxs-lookup"><span data-stu-id="14ae6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14ae6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14ae6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14ae6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14ae6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14ae6-140">Java</span><span class="sxs-lookup"><span data-stu-id="14ae6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="14ae6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="14ae6-141">Response</span></span>
<span data-ttu-id="14ae6-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14ae6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="14ae6-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="14ae6-145">See also</span></span>

- [<span data-ttu-id="14ae6-146">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="14ae6-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="14ae6-147">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="14ae6-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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