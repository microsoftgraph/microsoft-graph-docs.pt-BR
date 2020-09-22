---
title: Obter recurso
description: Recupere os dados binários de um objeto de recurso de arquivo ou imagem.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: b9eb6eb3d69cf89819ece38675893607c042e86b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038232"
---
# <a name="get-resource"></a><span data-ttu-id="a1c08-103">Obter recurso</span><span class="sxs-lookup"><span data-stu-id="a1c08-103">Get resource</span></span>

<span data-ttu-id="a1c08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1c08-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1c08-105">Recupere os dados binários de um objeto de [recurso](../resources/resource.md) de arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="a1c08-105">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1c08-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1c08-106">Permissions</span></span>
<span data-ttu-id="a1c08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1c08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1c08-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1c08-109">Permission type</span></span>      | <span data-ttu-id="a1c08-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1c08-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1c08-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1c08-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a1c08-112">Notes. Read, Notes. ReadWrite, Notes. Read. All, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a1c08-112">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a1c08-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1c08-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1c08-114">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1c08-114">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a1c08-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1c08-115">Application</span></span> | <span data-ttu-id="a1c08-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1c08-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1c08-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1c08-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="a1c08-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1c08-118">Request headers</span></span>
| <span data-ttu-id="a1c08-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a1c08-119">Name</span></span>       | <span data-ttu-id="a1c08-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1c08-120">Type</span></span> | <span data-ttu-id="a1c08-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1c08-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a1c08-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1c08-122">Authorization</span></span>  | <span data-ttu-id="a1c08-123">string</span><span class="sxs-lookup"><span data-stu-id="a1c08-123">string</span></span>  | <span data-ttu-id="a1c08-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1c08-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1c08-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1c08-126">Request body</span></span>
<span data-ttu-id="a1c08-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1c08-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1c08-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1c08-128">Response</span></span>

<span data-ttu-id="a1c08-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e os dados binários de imagem ou arquivo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1c08-129">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="a1c08-130">Observação: as imagens não são renderizadas diretamente em um navegador porque exigem autorização para recuperá-las, como o restante do conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="a1c08-130">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="a1c08-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1c08-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1c08-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1c08-132">Request</span></span>
<span data-ttu-id="a1c08-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1c08-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1c08-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1c08-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
# <a name="c"></a>[<span data-ttu-id="a1c08-135">C#</span><span class="sxs-lookup"><span data-stu-id="a1c08-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1c08-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1c08-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1c08-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1c08-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a1c08-138">Java</span><span class="sxs-lookup"><span data-stu-id="a1c08-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a1c08-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1c08-139">Response</span></span>
<span data-ttu-id="a1c08-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1c08-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

...binary data...
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

