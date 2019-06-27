---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Check-in de arquivos
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 75e2831d08b79060ca73821213440993265fbd2a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260267"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="6147f-102">Alterações de check-in em um recurso de DriveItem</span><span class="sxs-lookup"><span data-stu-id="6147f-102">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6147f-103">Check-in de um recurso DriveItem com check-out, que disponibiliza a versão do documento para outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="6147f-103">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="6147f-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="6147f-104">Permissions</span></span>

<span data-ttu-id="6147f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6147f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6147f-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6147f-107">Permission type</span></span>      | <span data-ttu-id="6147f-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6147f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6147f-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6147f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="6147f-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6147f-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6147f-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6147f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6147f-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6147f-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6147f-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6147f-113">Application</span></span> | <span data-ttu-id="6147f-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6147f-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6147f-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6147f-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="6147f-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6147f-116">Request body</span></span>

<span data-ttu-id="6147f-117">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6147f-117">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="6147f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6147f-118">Name</span></span>    | <span data-ttu-id="6147f-119">Valor</span><span class="sxs-lookup"><span data-stu-id="6147f-119">Value</span></span>  |                                                <span data-ttu-id="6147f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6147f-120">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6147f-121">checkInAs</span><span class="sxs-lookup"><span data-stu-id="6147f-121">checkInAs</span></span> | <span data-ttu-id="6147f-122">string</span><span class="sxs-lookup"><span data-stu-id="6147f-122">string</span></span> | <span data-ttu-id="6147f-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6147f-123">Optional.</span></span> <span data-ttu-id="6147f-124">O status desejado do documento após a conclusão da operação de check-in.</span><span class="sxs-lookup"><span data-stu-id="6147f-124">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="6147f-125">Pode ser `published` ou não especificado.</span><span class="sxs-lookup"><span data-stu-id="6147f-125">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="6147f-126">comment</span><span class="sxs-lookup"><span data-stu-id="6147f-126">comment</span></span>   | <span data-ttu-id="6147f-127">string</span><span class="sxs-lookup"><span data-stu-id="6147f-127">string</span></span> | <span data-ttu-id="6147f-128">Um comentário de check-in comentário associado à versão.</span><span class="sxs-lookup"><span data-stu-id="6147f-128">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="6147f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6147f-129">Example</span></span>

<span data-ttu-id="6147f-130">Este exemplo faz check-in de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="6147f-130">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="6147f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6147f-131">Response</span></span>

<span data-ttu-id="6147f-132">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="6147f-132">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6147f-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6147f-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6147f-134">C#</span><span class="sxs-lookup"><span data-stu-id="6147f-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/checkin-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6147f-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="6147f-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/checkin-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6147f-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6147f-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/checkin-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="remarks"></a><span data-ttu-id="6147f-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="6147f-137">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkin.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-checkin.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-checkin.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
