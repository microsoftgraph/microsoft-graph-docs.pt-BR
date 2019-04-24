---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Restaurar uma versão anterior
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 74ac8e9913b1d199d9baa019de6ea32b38e3654f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454290"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="bab25-102">Restaurar uma versão anterior de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="bab25-102">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bab25-103">Restaura uma versão anterior de um DriveItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="bab25-103">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="bab25-104">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="bab25-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="bab25-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bab25-105">Permissions</span></span>

<span data-ttu-id="bab25-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bab25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bab25-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bab25-108">Permission type</span></span>      | <span data-ttu-id="bab25-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bab25-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bab25-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bab25-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bab25-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bab25-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bab25-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bab25-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bab25-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bab25-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="bab25-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bab25-114">Application</span></span> | <span data-ttu-id="bab25-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bab25-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bab25-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bab25-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="bab25-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bab25-117">Request body</span></span>

<span data-ttu-id="bab25-118">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bab25-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="bab25-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bab25-119">Example</span></span>

<span data-ttu-id="bab25-120">Este exemplo restaura uma versão de um arquivo identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="bab25-120">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="bab25-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="bab25-121">Response</span></span>

<span data-ttu-id="bab25-122">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="bab25-122">If successful, the API call returns a `204 No content`.</span></span>

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
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
