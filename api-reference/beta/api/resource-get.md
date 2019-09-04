---
title: Obter recurso
description: Recupere os dados binários de um objeto de recurso de arquivo ou imagem.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: fbdb51394da0ca36f23656358cb545a89667a880
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722619"
---
# <a name="get-resource"></a><span data-ttu-id="3be22-103">Obter recurso</span><span class="sxs-lookup"><span data-stu-id="3be22-103">Get resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3be22-104">Recupere os dados binários de um objeto de [recurso](../resources/onenoteresource.md) de arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="3be22-104">Retrieve the binary data of a file or image [resource](../resources/onenoteresource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3be22-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3be22-105">Permissions</span></span>
<span data-ttu-id="3be22-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3be22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3be22-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3be22-108">Permission type</span></span>      | <span data-ttu-id="3be22-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3be22-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3be22-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3be22-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3be22-111">Notes. Read, Notes. ReadWrite, Notes. Read. All, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3be22-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3be22-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3be22-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3be22-113">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3be22-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3be22-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3be22-114">Application</span></span> | <span data-ttu-id="3be22-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3be22-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3be22-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3be22-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="3be22-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3be22-117">Request headers</span></span>
| <span data-ttu-id="3be22-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3be22-118">Name</span></span>       | <span data-ttu-id="3be22-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="3be22-119">Type</span></span> | <span data-ttu-id="3be22-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3be22-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3be22-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3be22-121">Authorization</span></span>  | <span data-ttu-id="3be22-122">string</span><span class="sxs-lookup"><span data-stu-id="3be22-122">string</span></span>  | <span data-ttu-id="3be22-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3be22-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3be22-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3be22-125">Request body</span></span>
<span data-ttu-id="3be22-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3be22-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3be22-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3be22-127">Response</span></span>

<span data-ttu-id="3be22-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e os dados binários de imagem ou arquivo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3be22-128">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="3be22-129">Observação: as imagens não são renderizadas diretamente em um navegador porque exigem autorização para recuperá-las, como o restante do conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="3be22-129">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="3be22-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3be22-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3be22-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3be22-131">Request</span></span>
<span data-ttu-id="3be22-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3be22-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3be22-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3be22-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/resources/{id}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3be22-134">C#</span><span class="sxs-lookup"><span data-stu-id="3be22-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3be22-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3be22-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3be22-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3be22-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3be22-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3be22-137">Response</span></span>
<span data-ttu-id="3be22-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3be22-138">Here is an example of the response.</span></span>
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
