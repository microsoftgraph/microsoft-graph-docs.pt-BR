---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Restaurar uma versão anterior
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e04a46804e5963695e2bd1ee0356e3e754d36ccd
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33588121"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="4f647-102">Restaurar uma versão anterior de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="4f647-102">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f647-103">Restaura uma versão anterior de um DriveItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="4f647-103">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="4f647-104">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="4f647-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f647-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f647-105">Permissions</span></span>

<span data-ttu-id="4f647-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f647-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f647-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f647-108">Permission type</span></span>      | <span data-ttu-id="4f647-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f647-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f647-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f647-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4f647-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f647-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f647-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f647-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f647-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f647-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f647-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f647-114">Application</span></span> | <span data-ttu-id="4f647-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f647-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f647-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f647-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="4f647-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f647-117">Request body</span></span>

<span data-ttu-id="4f647-118">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f647-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="4f647-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f647-119">Example</span></span>

<span data-ttu-id="4f647-120">Este exemplo restaura uma versão de um arquivo identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="4f647-120">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="4f647-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f647-121">Response</span></span>

<span data-ttu-id="4f647-122">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="4f647-122">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4f647-123">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4f647-123">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4f647-124">Basic</span><span class="sxs-lookup"><span data-stu-id="4f647-124">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/restore-item-version-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f647-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f647-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/restore-item-version-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
