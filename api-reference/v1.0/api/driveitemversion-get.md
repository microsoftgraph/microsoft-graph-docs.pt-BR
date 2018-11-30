---
title: Obter um recurso DriveItemVersion
description: Recuperar os metadados de uma versão específica de um DriveItem.
ms.openlocfilehash: 1b803e92b7a717514e794da5ac8da04c0ef05f6a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007468"
---
# <a name="get-a-driveitemversion-resource"></a><span data-ttu-id="2b7be-103">Obter um recurso DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="2b7be-103">Get a DriveItemVersion resource</span></span>

<span data-ttu-id="2b7be-104">Recuperar os metadados de uma versão específica de um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2b7be-104">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2b7be-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b7be-105">Permissions</span></span>

<span data-ttu-id="2b7be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b7be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b7be-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b7be-108">Permission type</span></span>      | <span data-ttu-id="2b7be-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b7be-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b7be-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b7be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b7be-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b7be-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b7be-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b7be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b7be-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b7be-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b7be-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b7be-114">Application</span></span> | <span data-ttu-id="2b7be-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b7be-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="2b7be-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b7be-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="2b7be-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b7be-117">Response</span></span>

<span data-ttu-id="2b7be-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [DriveItemVersion](../resources/driveitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b7be-118">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="2b7be-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b7be-119">Example</span></span>

<span data-ttu-id="2b7be-120">Este exemplo recupera uma versão de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="2b7be-120">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="2b7be-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b7be-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="2b7be-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b7be-122">Response</span></span>

<span data-ttu-id="2b7be-123">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="2b7be-123">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="2b7be-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="2b7be-124">Remarks</span></span>

<span data-ttu-id="2b7be-125">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="2b7be-125">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="2b7be-126">Quando seu aplicativo recupera a lista de versões disponíveis de um arquivo, um recurso [DriveItemVersion](../resources/driveitemversion.md) é retornado e fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="2b7be-126">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
