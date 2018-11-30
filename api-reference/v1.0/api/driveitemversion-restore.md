---
title: Restaurar uma versão anterior de um DriveItem
description: Restaura uma versão anterior de um DriveItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do arquivo.
ms.openlocfilehash: e8272678e048391279d5b2147985d4f1e83f0456
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006827"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="08af6-104">Restaurar uma versão anterior de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="08af6-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="08af6-105">Restaura uma versão anterior de um DriveItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="08af6-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="08af6-106">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="08af6-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="08af6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="08af6-107">Permissions</span></span>

<span data-ttu-id="08af6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08af6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08af6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08af6-110">Permission type</span></span>      | <span data-ttu-id="08af6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08af6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08af6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08af6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08af6-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08af6-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="08af6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08af6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08af6-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08af6-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="08af6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08af6-116">Application</span></span> | <span data-ttu-id="08af6-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08af6-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08af6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08af6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="08af6-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08af6-119">Request body</span></span>

<span data-ttu-id="08af6-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08af6-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="08af6-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08af6-121">Example</span></span>

<span data-ttu-id="08af6-122">Este exemplo restaura uma versão de um arquivo identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="08af6-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="08af6-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="08af6-123">Response</span></span>

<span data-ttu-id="08af6-124">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="08af6-124">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
