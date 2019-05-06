---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Check-in de arquivos
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 982a581d44e39e6ddcc7bb3a52da64cd2a2eaf55
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589353"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="5d935-102">Alterações de check-in em um recurso de DriveItem</span><span class="sxs-lookup"><span data-stu-id="5d935-102">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d935-103">Check-in de um recurso DriveItem com check-out, que disponibiliza a versão do documento para outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="5d935-103">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d935-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d935-104">Permissions</span></span>

<span data-ttu-id="5d935-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d935-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d935-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d935-107">Permission type</span></span>      | <span data-ttu-id="5d935-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d935-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d935-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d935-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5d935-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d935-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d935-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d935-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d935-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d935-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d935-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d935-113">Application</span></span> | <span data-ttu-id="5d935-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d935-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d935-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d935-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="5d935-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d935-116">Request body</span></span>

<span data-ttu-id="5d935-117">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d935-117">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="5d935-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5d935-118">Name</span></span>    | <span data-ttu-id="5d935-119">Valor</span><span class="sxs-lookup"><span data-stu-id="5d935-119">Value</span></span>  |                                                <span data-ttu-id="5d935-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d935-120">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5d935-121">checkInAs</span><span class="sxs-lookup"><span data-stu-id="5d935-121">checkInAs</span></span> | <span data-ttu-id="5d935-122">string</span><span class="sxs-lookup"><span data-stu-id="5d935-122">string</span></span> | <span data-ttu-id="5d935-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5d935-123">Optional.</span></span> <span data-ttu-id="5d935-124">O status desejado do documento após a conclusão da operação de check-in.</span><span class="sxs-lookup"><span data-stu-id="5d935-124">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="5d935-125">Pode ser `published` ou não especificado.</span><span class="sxs-lookup"><span data-stu-id="5d935-125">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="5d935-126">comment</span><span class="sxs-lookup"><span data-stu-id="5d935-126">comment</span></span>   | <span data-ttu-id="5d935-127">string</span><span class="sxs-lookup"><span data-stu-id="5d935-127">string</span></span> | <span data-ttu-id="5d935-128">Um comentário de check-in comentário associado à versão.</span><span class="sxs-lookup"><span data-stu-id="5d935-128">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="5d935-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d935-129">Example</span></span>

<span data-ttu-id="5d935-130">Este exemplo faz check-in de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="5d935-130">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="5d935-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d935-131">Response</span></span>

<span data-ttu-id="5d935-132">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="5d935-132">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5d935-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5d935-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5d935-134">Basic</span><span class="sxs-lookup"><span data-stu-id="5d935-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/checkin-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5d935-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d935-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/checkin-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="remarks"></a><span data-ttu-id="5d935-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="5d935-136">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkin.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-checkin.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
