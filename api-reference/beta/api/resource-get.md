---
title: Obter recurso
description: Recupere os dados binários de um objeto de recurso de arquivo ou imagem.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 9fe2b1a23f3079022c20ab16e9b8d8efb4a1e759
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453902"
---
# <a name="get-resource"></a><span data-ttu-id="4bef4-103">Obter recurso</span><span class="sxs-lookup"><span data-stu-id="4bef4-103">Get resource</span></span>

<span data-ttu-id="4bef4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4bef4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bef4-105">Recupere os dados binários de um objeto de [recurso](../resources/onenoteresource.md) de arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="4bef4-105">Retrieve the binary data of a file or image [resource](../resources/onenoteresource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4bef4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4bef4-106">Permissions</span></span>
<span data-ttu-id="4bef4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bef4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bef4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bef4-109">Permission type</span></span>      | <span data-ttu-id="4bef4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4bef4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bef4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bef4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4bef4-112">Notes. Read, Notes. ReadWrite, Notes. Read. All, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4bef4-112">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4bef4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bef4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bef4-114">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4bef4-114">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4bef4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bef4-115">Application</span></span> | <span data-ttu-id="4bef4-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bef4-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bef4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bef4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="4bef4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bef4-118">Request headers</span></span>
| <span data-ttu-id="4bef4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4bef4-119">Name</span></span>       | <span data-ttu-id="4bef4-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bef4-120">Type</span></span> | <span data-ttu-id="4bef4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bef4-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4bef4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bef4-122">Authorization</span></span>  | <span data-ttu-id="4bef4-123">string</span><span class="sxs-lookup"><span data-stu-id="4bef4-123">string</span></span>  | <span data-ttu-id="4bef4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bef4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bef4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bef4-126">Request body</span></span>
<span data-ttu-id="4bef4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4bef4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bef4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bef4-128">Response</span></span>

<span data-ttu-id="4bef4-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e os dados binários de imagem ou arquivo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bef4-129">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="4bef4-130">Observação: as imagens não são renderizadas diretamente em um navegador porque exigem autorização para recuperá-las, como o restante do conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="4bef4-130">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="4bef4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bef4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bef4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bef4-132">Request</span></span>
<span data-ttu-id="4bef4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bef4-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4bef4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bef4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/resources/{id}/content
```
# <a name="c"></a>[<span data-ttu-id="4bef4-135">C#</span><span class="sxs-lookup"><span data-stu-id="4bef4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4bef4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4bef4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4bef4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4bef4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4bef4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bef4-138">Response</span></span>
<span data-ttu-id="4bef4-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bef4-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

...binary data...
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
