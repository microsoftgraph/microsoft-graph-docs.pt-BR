---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Restaurar uma versão anterior de um item de lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ef3b5848b6a6f60bf0515f914e87383e0a6f66bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511552"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="291e8-102">Restaura uma versão anterior de um ListItem</span><span class="sxs-lookup"><span data-stu-id="291e8-102">Restore a previous version of a ListItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="291e8-103">Restaura uma versão anterior de um ListItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="291e8-103">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="291e8-104">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.</span><span class="sxs-lookup"><span data-stu-id="291e8-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="291e8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="291e8-105">Permissions</span></span>

<span data-ttu-id="291e8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="291e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="291e8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="291e8-108">Permission type</span></span>             |         <span data-ttu-id="291e8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="291e8-109">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="291e8-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="291e8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="291e8-111">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="291e8-111">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="291e8-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="291e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="291e8-113">n/d</span><span class="sxs-lookup"><span data-stu-id="291e8-113">n/a</span></span>                                                          |
| <span data-ttu-id="291e8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="291e8-114">Application</span></span>                            | <span data-ttu-id="291e8-115">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="291e8-115">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="291e8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="291e8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="291e8-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="291e8-117">Request body</span></span>

<span data-ttu-id="291e8-118">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="291e8-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="291e8-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="291e8-119">Example</span></span>

<span data-ttu-id="291e8-120">Este exemplo restaura uma versão de um listItem identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="291e8-120">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="291e8-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="291e8-121">Response</span></span>

<span data-ttu-id="291e8-122">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="291e8-122">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/listitemversion-restore.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
