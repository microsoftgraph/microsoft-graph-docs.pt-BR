---
author: JeremyKelley
description: Faça check-in em um recurso de DriveItem com check-out, que torna a versão do documento disponível para outras pessoas.
title: 'driveItem: checkin'
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 92200c0e079a885192f2ad1709a1e45bb15370e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982161"
---
# <a name="driveitem-checkin"></a><span data-ttu-id="8cc6d-103">driveItem: checkin</span><span class="sxs-lookup"><span data-stu-id="8cc6d-103">driveItem: checkin</span></span>

<span data-ttu-id="8cc6d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cc6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cc6d-105">Faça check-in em um recurso de **driveItem** com check-out, que torna a versão do documento disponível para outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="8cc6d-105">Check in a checked out **driveItem** resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cc6d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8cc6d-106">Permissions</span></span>

<span data-ttu-id="8cc6d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc6d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cc6d-109">Permission type</span></span>      | <span data-ttu-id="8cc6d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8cc6d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cc6d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cc6d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8cc6d-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc6d-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8cc6d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cc6d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cc6d-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc6d-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8cc6d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cc6d-115">Application</span></span> | <span data-ttu-id="8cc6d-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc6d-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cc6d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc6d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="8cc6d-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc6d-118">Request body</span></span>

<span data-ttu-id="8cc6d-119">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc6d-119">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="8cc6d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8cc6d-120">Name</span></span>    | <span data-ttu-id="8cc6d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8cc6d-121">Value</span></span>  |                                                <span data-ttu-id="8cc6d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc6d-122">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8cc6d-123">checkInAs</span><span class="sxs-lookup"><span data-stu-id="8cc6d-123">checkInAs</span></span> | <span data-ttu-id="8cc6d-124">string</span><span class="sxs-lookup"><span data-stu-id="8cc6d-124">string</span></span> | <span data-ttu-id="8cc6d-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8cc6d-125">Optional.</span></span> <span data-ttu-id="8cc6d-126">O status do documento após a conclusão da operação de check-in.</span><span class="sxs-lookup"><span data-stu-id="8cc6d-126">The status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="8cc6d-127">Pode ser `published` ou não especificado.</span><span class="sxs-lookup"><span data-stu-id="8cc6d-127">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="8cc6d-128">comment</span><span class="sxs-lookup"><span data-stu-id="8cc6d-128">comment</span></span>   | <span data-ttu-id="8cc6d-129">string</span><span class="sxs-lookup"><span data-stu-id="8cc6d-129">string</span></span> | <span data-ttu-id="8cc6d-130">Um comentário de check-in comentário associado à versão.</span><span class="sxs-lookup"><span data-stu-id="8cc6d-130">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="8cc6d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cc6d-131">Example</span></span>

<span data-ttu-id="8cc6d-132">Este exemplo faz check-in de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="8cc6d-132">This example checks in a file identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="8cc6d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc6d-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="c"></a>[<span data-ttu-id="8cc6d-134">C#</span><span class="sxs-lookup"><span data-stu-id="8cc6d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8cc6d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cc6d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cc6d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cc6d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="8cc6d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc6d-137">Response</span></span>

<span data-ttu-id="8cc6d-138">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="8cc6d-138">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="8cc6d-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="8cc6d-139">Remarks</span></span>


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


