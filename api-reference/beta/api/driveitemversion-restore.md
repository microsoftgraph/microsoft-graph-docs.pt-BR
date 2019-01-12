---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Restaurar uma versão anterior
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9f8492b3a6e4b01b61288b235cc0dfa19ffd78d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946074"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="13ee5-102">Restaurar uma versão anterior de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="13ee5-102">Restore a previous version of a DriveItem</span></span>

> <span data-ttu-id="13ee5-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="13ee5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13ee5-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="13ee5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13ee5-105">Restaura uma versão anterior de um DriveItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="13ee5-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="13ee5-106">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="13ee5-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="13ee5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="13ee5-107">Permissions</span></span>

<span data-ttu-id="13ee5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13ee5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13ee5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13ee5-110">Permission type</span></span>      | <span data-ttu-id="13ee5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13ee5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13ee5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13ee5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="13ee5-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13ee5-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="13ee5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13ee5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13ee5-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13ee5-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="13ee5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13ee5-116">Application</span></span> | <span data-ttu-id="13ee5-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13ee5-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13ee5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13ee5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="13ee5-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13ee5-119">Request body</span></span>

<span data-ttu-id="13ee5-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13ee5-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="13ee5-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13ee5-121">Example</span></span>

<span data-ttu-id="13ee5-122">Este exemplo restaura uma versão de um arquivo identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="13ee5-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="13ee5-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="13ee5-123">Response</span></span>

<span data-ttu-id="13ee5-124">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="13ee5-124">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
