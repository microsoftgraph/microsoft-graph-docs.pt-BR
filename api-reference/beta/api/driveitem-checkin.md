---
author: JeremyKelley
description: Check-in de um recurso DriveItem com check-out, que disponibiliza a versão do documento para outras pessoas.
ms.date: 09/10/2017
title: Check-in de arquivos
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: ffdddf5e3800d2bfb14038c7bec5b1b8fdcb0809
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321056"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="ef97f-103">Alterações de check-in em um recurso de DriveItem</span><span class="sxs-lookup"><span data-stu-id="ef97f-103">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef97f-104">Check-in de um recurso DriveItem com check-out, que disponibiliza a versão do documento para outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="ef97f-104">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef97f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef97f-105">Permissions</span></span>

<span data-ttu-id="ef97f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef97f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef97f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef97f-108">Permission type</span></span>      | <span data-ttu-id="ef97f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef97f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef97f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef97f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ef97f-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef97f-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef97f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef97f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef97f-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef97f-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef97f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef97f-114">Application</span></span> | <span data-ttu-id="ef97f-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef97f-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef97f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef97f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="ef97f-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef97f-117">Request body</span></span>

<span data-ttu-id="ef97f-118">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef97f-118">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="ef97f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ef97f-119">Name</span></span>    | <span data-ttu-id="ef97f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ef97f-120">Value</span></span>  |                                                <span data-ttu-id="ef97f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef97f-121">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ef97f-122">checkInAs</span><span class="sxs-lookup"><span data-stu-id="ef97f-122">checkInAs</span></span> | <span data-ttu-id="ef97f-123">string</span><span class="sxs-lookup"><span data-stu-id="ef97f-123">string</span></span> | <span data-ttu-id="ef97f-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ef97f-124">Optional.</span></span> <span data-ttu-id="ef97f-125">O status desejado do documento após a conclusão da operação de check-in.</span><span class="sxs-lookup"><span data-stu-id="ef97f-125">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="ef97f-126">Pode ser `published` ou não especificado.</span><span class="sxs-lookup"><span data-stu-id="ef97f-126">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="ef97f-127">comment</span><span class="sxs-lookup"><span data-stu-id="ef97f-127">comment</span></span>   | <span data-ttu-id="ef97f-128">string</span><span class="sxs-lookup"><span data-stu-id="ef97f-128">string</span></span> | <span data-ttu-id="ef97f-129">Um comentário de check-in comentário associado à versão.</span><span class="sxs-lookup"><span data-stu-id="ef97f-129">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="ef97f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef97f-130">Example</span></span>

<span data-ttu-id="ef97f-131">Este exemplo faz check-in de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="ef97f-131">This example checks in a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ef97f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef97f-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ef97f-133">C#</span><span class="sxs-lookup"><span data-stu-id="ef97f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef97f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef97f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ef97f-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ef97f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ef97f-136">Java</span><span class="sxs-lookup"><span data-stu-id="ef97f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkin-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="ef97f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef97f-137">Response</span></span>

<span data-ttu-id="ef97f-138">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="ef97f-138">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="ef97f-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="ef97f-139">Remarks</span></span>


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
