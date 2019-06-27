---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Fazer check-out de arquivos
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f5447e9e849797081ae96429aaea664abb835a45
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260253"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="38aab-102">Fazer check-out do recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="38aab-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38aab-103">Check-out de um recurso driveItem para impedir que outras pessoas editem o documento e que suas alterações fiquem visíveis até que o documento passe por [check-in](driveitem-checkin.md).</span><span class="sxs-lookup"><span data-stu-id="38aab-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="38aab-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="38aab-104">Permissions</span></span>

<span data-ttu-id="38aab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38aab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38aab-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38aab-107">Permission type</span></span>      | <span data-ttu-id="38aab-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38aab-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38aab-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38aab-109">Delegated (work or school account)</span></span> | <span data-ttu-id="38aab-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38aab-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="38aab-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38aab-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38aab-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38aab-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="38aab-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38aab-113">Application</span></span> | <span data-ttu-id="38aab-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38aab-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38aab-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38aab-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="38aab-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38aab-116">Request body</span></span>

<span data-ttu-id="38aab-117">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38aab-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="38aab-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38aab-118">Example</span></span>

<span data-ttu-id="38aab-119">Este exemplo faz check-out de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="38aab-119">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="38aab-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="38aab-120">Response</span></span>

<span data-ttu-id="38aab-121">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="38aab-121">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="38aab-122">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="38aab-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="38aab-123">C#</span><span class="sxs-lookup"><span data-stu-id="38aab-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/checkout-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38aab-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="38aab-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/checkout-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="38aab-125">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="38aab-125">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/checkout-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="remarks"></a><span data-ttu-id="38aab-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="38aab-126">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
