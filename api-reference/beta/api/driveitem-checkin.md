---
author: JeremyKelley
description: Faça check-in em um recurso de DriveItem com check-out, que torna a versão do documento disponível para outras pessoas.
title: 'driveItem: checkin'
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c259b4c5c729d3af04876367d1273435b32302f5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955678"
---
# <a name="driveitem-checkin"></a><span data-ttu-id="25fc3-103">driveItem: checkin</span><span class="sxs-lookup"><span data-stu-id="25fc3-103">driveItem: checkin</span></span>

<span data-ttu-id="25fc3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25fc3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25fc3-105">Faça check-in em um recurso de **driveItem** com check-out, que torna a versão do documento disponível para outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="25fc3-105">Check in a checked out **driveItem** resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="25fc3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="25fc3-106">Permissions</span></span>

<span data-ttu-id="25fc3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25fc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25fc3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25fc3-109">Permission type</span></span>      | <span data-ttu-id="25fc3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25fc3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25fc3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25fc3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="25fc3-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25fc3-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="25fc3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25fc3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25fc3-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25fc3-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="25fc3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25fc3-115">Application</span></span> | <span data-ttu-id="25fc3-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25fc3-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25fc3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25fc3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="25fc3-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25fc3-118">Request body</span></span>

<span data-ttu-id="25fc3-119">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25fc3-119">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="25fc3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="25fc3-120">Name</span></span>    | <span data-ttu-id="25fc3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="25fc3-121">Value</span></span>  |                                                <span data-ttu-id="25fc3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="25fc3-122">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="25fc3-123">checkInAs</span><span class="sxs-lookup"><span data-stu-id="25fc3-123">checkInAs</span></span> | <span data-ttu-id="25fc3-124">string</span><span class="sxs-lookup"><span data-stu-id="25fc3-124">string</span></span> | <span data-ttu-id="25fc3-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="25fc3-125">Optional.</span></span> <span data-ttu-id="25fc3-126">O status do documento após a conclusão da operação de check-in.</span><span class="sxs-lookup"><span data-stu-id="25fc3-126">The status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="25fc3-127">Pode ser `published` ou não especificado.</span><span class="sxs-lookup"><span data-stu-id="25fc3-127">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="25fc3-128">comment</span><span class="sxs-lookup"><span data-stu-id="25fc3-128">comment</span></span>   | <span data-ttu-id="25fc3-129">string</span><span class="sxs-lookup"><span data-stu-id="25fc3-129">string</span></span> | <span data-ttu-id="25fc3-130">Um comentário de check-in comentário associado à versão.</span><span class="sxs-lookup"><span data-stu-id="25fc3-130">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="25fc3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25fc3-131">Example</span></span>

<span data-ttu-id="25fc3-132">Este exemplo faz check-in de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="25fc3-132">This example checks in a file identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="25fc3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="25fc3-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="c"></a>[<span data-ttu-id="25fc3-134">C#</span><span class="sxs-lookup"><span data-stu-id="25fc3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25fc3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25fc3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25fc3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25fc3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25fc3-137">Java</span><span class="sxs-lookup"><span data-stu-id="25fc3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkin-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="25fc3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="25fc3-138">Response</span></span>

<span data-ttu-id="25fc3-139">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="25fc3-139">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="25fc3-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="25fc3-140">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->


