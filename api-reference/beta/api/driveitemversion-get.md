---
title: Obter um recurso DriveItemVersion (prévia)
description: Recuperar os metadados de uma versão específica de um DriveItem.
localization_priority: Normal
ms.openlocfilehash: f0c5611b769ed5e8adb63550a76016a055245504
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853708"
---
# <a name="get-a-driveitemversion-resource-preview"></a><span data-ttu-id="ccb97-103">Obter um recurso DriveItemVersion (prévia)</span><span class="sxs-lookup"><span data-stu-id="ccb97-103">Get a DriveItemVersion resource (preview)</span></span>

> <span data-ttu-id="ccb97-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ccb97-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ccb97-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ccb97-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ccb97-106">Recuperar os metadados de uma versão específica de um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ccb97-106">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ccb97-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ccb97-107">Permissions</span></span>

<span data-ttu-id="ccb97-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccb97-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccb97-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccb97-110">Permission type</span></span>      | <span data-ttu-id="ccb97-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ccb97-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccb97-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccb97-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ccb97-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccb97-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ccb97-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccb97-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccb97-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccb97-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ccb97-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccb97-116">Application</span></span> | <span data-ttu-id="ccb97-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccb97-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="ccb97-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccb97-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="ccb97-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccb97-119">Response</span></span>

<span data-ttu-id="ccb97-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [DriveItemVersion](../resources/driveitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccb97-120">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="ccb97-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ccb97-121">Example</span></span>

<span data-ttu-id="ccb97-122">Este exemplo recupera uma versão de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="ccb97-122">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="ccb97-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccb97-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="ccb97-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccb97-124">Response</span></span>

<span data-ttu-id="ccb97-125">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="ccb97-125">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="ccb97-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="ccb97-126">Remarks</span></span>

<span data-ttu-id="ccb97-127">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="ccb97-127">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="ccb97-128">Quando seu aplicativo recupera a lista de versões disponíveis de um arquivo, um recurso [DriveItemVersion](../resources/driveitemversion.md) é retornado e fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="ccb97-128">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
