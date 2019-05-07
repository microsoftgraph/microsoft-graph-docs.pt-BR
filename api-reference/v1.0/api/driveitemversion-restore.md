---
title: Restaurar uma versão anterior de um DriveItem
description: Restaura uma versão anterior de um DriveItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do arquivo.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 53a8f5e40e06ef90662a55c44ca718bc82f4fb4b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616225"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="56d4f-104">Restaurar uma versão anterior de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="56d4f-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="56d4f-105">Restaura uma versão anterior de um DriveItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="56d4f-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="56d4f-106">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="56d4f-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="56d4f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="56d4f-107">Permissions</span></span>

<span data-ttu-id="56d4f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56d4f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56d4f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56d4f-110">Permission type</span></span>      | <span data-ttu-id="56d4f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56d4f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56d4f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56d4f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="56d4f-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d4f-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="56d4f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56d4f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56d4f-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d4f-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="56d4f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56d4f-116">Application</span></span> | <span data-ttu-id="56d4f-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d4f-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56d4f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56d4f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="56d4f-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56d4f-119">Request body</span></span>

<span data-ttu-id="56d4f-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56d4f-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="56d4f-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56d4f-121">Example</span></span>

<span data-ttu-id="56d4f-122">Este exemplo restaura uma versão de um arquivo identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="56d4f-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="56d4f-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="56d4f-123">Response</span></span>

<span data-ttu-id="56d4f-124">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="56d4f-124">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="56d4f-125">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="56d4f-125">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="56d4f-126">Basic</span><span class="sxs-lookup"><span data-stu-id="56d4f-126">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/restore-item-version-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56d4f-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56d4f-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/restore-item-version-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
