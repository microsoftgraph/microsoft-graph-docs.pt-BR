---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Fazer check-out de arquivos
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: acb10e216cbf4537bee78ac7ad9562d2ebdb062f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436491"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="bbc11-102">Fazer check-out do recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="bbc11-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbc11-103">Check-out de um recurso driveItem para impedir que outras pessoas editem o documento e que suas alterações fiquem visíveis até que o documento passe por [check-in](driveitem-checkin.md).</span><span class="sxs-lookup"><span data-stu-id="bbc11-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bbc11-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbc11-104">Permissions</span></span>

<span data-ttu-id="bbc11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbc11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbc11-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbc11-107">Permission type</span></span>      | <span data-ttu-id="bbc11-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbc11-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbc11-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbc11-109">Delegated (work or school account)</span></span> | <span data-ttu-id="bbc11-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbc11-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bbc11-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbc11-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbc11-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbc11-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="bbc11-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbc11-113">Application</span></span> | <span data-ttu-id="bbc11-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbc11-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbc11-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbc11-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="bbc11-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbc11-116">Request body</span></span>

<span data-ttu-id="bbc11-117">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbc11-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="bbc11-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbc11-118">Example</span></span>

<span data-ttu-id="bbc11-119">Este exemplo faz check-out de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="bbc11-119">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bbc11-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbc11-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bbc11-121">C#</span><span class="sxs-lookup"><span data-stu-id="bbc11-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bbc11-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="bbc11-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bbc11-123">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bbc11-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="bbc11-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbc11-124">Response</span></span>

<span data-ttu-id="bbc11-125">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="bbc11-125">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="bbc11-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="bbc11-126">Remarks</span></span>


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
