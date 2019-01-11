---
title: Obter um recurso DriveItemVersion
description: Recuperar os metadados de uma versão específica de um DriveItem.
localization_priority: Normal
ms.openlocfilehash: d16e6bf6a9fa797f952109a773cfd4227696e032
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868338"
---
# <a name="get-a-driveitemversion-resource"></a><span data-ttu-id="8a4fb-103">Obter um recurso DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="8a4fb-103">Get a DriveItemVersion resource</span></span>

<span data-ttu-id="8a4fb-104">Recuperar os metadados de uma versão específica de um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8a4fb-104">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8a4fb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a4fb-105">Permissions</span></span>

<span data-ttu-id="8a4fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a4fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a4fb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a4fb-108">Permission type</span></span>      | <span data-ttu-id="8a4fb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a4fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a4fb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a4fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8a4fb-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4fb-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a4fb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a4fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a4fb-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4fb-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a4fb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a4fb-114">Application</span></span> | <span data-ttu-id="8a4fb-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4fb-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="8a4fb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a4fb-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="8a4fb-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a4fb-117">Response</span></span>

<span data-ttu-id="8a4fb-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [DriveItemVersion](../resources/driveitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a4fb-118">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="8a4fb-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a4fb-119">Example</span></span>

<span data-ttu-id="8a4fb-120">Este exemplo recupera uma versão de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="8a4fb-120">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="8a4fb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a4fb-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="8a4fb-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a4fb-122">Response</span></span>

<span data-ttu-id="8a4fb-123">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="8a4fb-123">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "D4990684-58CE-4FAB-9B87-D6C49E74F298",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "size": 123
}
```

## <a name="remarks"></a><span data-ttu-id="8a4fb-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="8a4fb-124">Remarks</span></span>

<span data-ttu-id="8a4fb-125">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="8a4fb-125">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="8a4fb-126">Quando seu aplicativo recupera a lista de versões disponíveis de um arquivo, um recurso [DriveItemVersion](../resources/driveitemversion.md) é retornado e fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="8a4fb-126">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
