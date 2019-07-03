---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Restaurar uma versão anterior
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 43d46caf83a028b751a0c21c3bffe69ee0983c11
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436183"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="304f1-102">Restaurar uma versão anterior de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="304f1-102">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="304f1-103">Restaura uma versão anterior de um DriveItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="304f1-103">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="304f1-104">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="304f1-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="304f1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="304f1-105">Permissions</span></span>

<span data-ttu-id="304f1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="304f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="304f1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="304f1-108">Permission type</span></span>      | <span data-ttu-id="304f1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="304f1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="304f1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="304f1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="304f1-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="304f1-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="304f1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="304f1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="304f1-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="304f1-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="304f1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="304f1-114">Application</span></span> | <span data-ttu-id="304f1-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="304f1-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="304f1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="304f1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="304f1-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="304f1-117">Request body</span></span>

<span data-ttu-id="304f1-118">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="304f1-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="304f1-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="304f1-119">Example</span></span>

<span data-ttu-id="304f1-120">Este exemplo restaura uma versão de um arquivo identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="304f1-120">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="304f1-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="304f1-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="304f1-122">C#</span><span class="sxs-lookup"><span data-stu-id="304f1-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="304f1-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="304f1-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="304f1-124">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="304f1-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="304f1-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="304f1-125">Response</span></span>

<span data-ttu-id="304f1-126">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="304f1-126">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

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
