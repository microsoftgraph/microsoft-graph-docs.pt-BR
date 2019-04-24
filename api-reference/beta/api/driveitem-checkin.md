---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Check-in de arquivos
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ea8d4b8ec5399e867bd94c261ce95783f8ea27ba
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454572"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="53879-102">Alterações de check-in em um recurso de DriveItem</span><span class="sxs-lookup"><span data-stu-id="53879-102">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53879-103">Check-in de um recurso DriveItem com check-out, que disponibiliza a versão do documento para outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="53879-103">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="53879-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="53879-104">Permissions</span></span>

<span data-ttu-id="53879-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53879-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53879-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53879-107">Permission type</span></span>      | <span data-ttu-id="53879-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53879-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53879-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53879-109">Delegated (work or school account)</span></span> | <span data-ttu-id="53879-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53879-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="53879-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53879-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53879-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53879-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="53879-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53879-113">Application</span></span> | <span data-ttu-id="53879-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53879-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53879-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53879-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="53879-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53879-116">Request body</span></span>

<span data-ttu-id="53879-117">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53879-117">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="53879-118">Name</span><span class="sxs-lookup"><span data-stu-id="53879-118">Name</span></span>    | <span data-ttu-id="53879-119">Valor</span><span class="sxs-lookup"><span data-stu-id="53879-119">Value</span></span>  |                                                <span data-ttu-id="53879-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="53879-120">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="53879-121">checkInAs</span><span class="sxs-lookup"><span data-stu-id="53879-121">checkInAs</span></span> | <span data-ttu-id="53879-122">string</span><span class="sxs-lookup"><span data-stu-id="53879-122">string</span></span> | <span data-ttu-id="53879-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="53879-123">Optional.</span></span> <span data-ttu-id="53879-124">O status desejado do documento após a conclusão da operação de check-in.</span><span class="sxs-lookup"><span data-stu-id="53879-124">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="53879-125">Pode ser `published` ou não especificado.</span><span class="sxs-lookup"><span data-stu-id="53879-125">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="53879-126">comment</span><span class="sxs-lookup"><span data-stu-id="53879-126">comment</span></span>   | <span data-ttu-id="53879-127">string</span><span class="sxs-lookup"><span data-stu-id="53879-127">string</span></span> | <span data-ttu-id="53879-128">Um comentário de check-in comentário associado à versão.</span><span class="sxs-lookup"><span data-stu-id="53879-128">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="53879-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53879-129">Example</span></span>

<span data-ttu-id="53879-130">Este exemplo faz check-in de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="53879-130">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="53879-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="53879-131">Response</span></span>

<span data-ttu-id="53879-132">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="53879-132">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="53879-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="53879-133">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkin.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
