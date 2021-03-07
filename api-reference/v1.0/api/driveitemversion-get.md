---
title: Obter um recurso DriveItemVersion
description: Recuperar os metadados de uma versão específica de um DriveItem.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: 74076a044dcab00fc25dfe829eaee582d9a0d6b6
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516777"
---
# <a name="get-a-driveitemversion-resource"></a><span data-ttu-id="e18d8-103">Obter um recurso DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="e18d8-103">Get a DriveItemVersion resource</span></span>

<span data-ttu-id="e18d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e18d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e18d8-105">Recuperar os metadados de uma versão específica de um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e18d8-105">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e18d8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e18d8-106">Permissions</span></span>

<span data-ttu-id="e18d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e18d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e18d8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e18d8-109">Permission type</span></span>      | <span data-ttu-id="e18d8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e18d8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e18d8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e18d8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e18d8-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e18d8-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e18d8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e18d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e18d8-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e18d8-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e18d8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e18d8-115">Application</span></span> | <span data-ttu-id="e18d8-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e18d8-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="e18d8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e18d8-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/items/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="e18d8-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="e18d8-118">Response</span></span>

<span data-ttu-id="e18d8-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [DriveItemVersion](../resources/driveitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e18d8-119">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="e18d8-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e18d8-120">Example</span></span>

<span data-ttu-id="e18d8-121">Este exemplo recupera uma versão de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="e18d8-121">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="e18d8-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e18d8-122">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="e18d8-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="e18d8-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/versions/{version-id}
```
# <a name="c"></a>[<span data-ttu-id="e18d8-124">C#</span><span class="sxs-lookup"><span data-stu-id="e18d8-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-single-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e18d8-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e18d8-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-single-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e18d8-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e18d8-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-single-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e18d8-127">Java</span><span class="sxs-lookup"><span data-stu-id="e18d8-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-single-version-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e18d8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e18d8-128">Response</span></span>

<span data-ttu-id="e18d8-129">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="e18d8-129">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="e18d8-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="e18d8-130">Remarks</span></span>

<span data-ttu-id="e18d8-131">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="e18d8-131">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="e18d8-132">Quando seu aplicativo recupera a lista de versões disponíveis de um arquivo, um recurso [DriveItemVersion](../resources/driveitemversion.md) é retornado e fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="e18d8-132">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->

