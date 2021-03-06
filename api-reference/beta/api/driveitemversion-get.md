---
title: Obter um recurso DriveItemVersion (prévia)
description: Recuperar os metadados de uma versão específica de um DriveItem.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: JeremyKelley
ms.openlocfilehash: d5beccc75cb1c6b79995f07ca4cb2dba729761e6
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515713"
---
# <a name="get-a-driveitemversion-resource-preview"></a><span data-ttu-id="fe626-103">Obter um recurso DriveItemVersion (prévia)</span><span class="sxs-lookup"><span data-stu-id="fe626-103">Get a DriveItemVersion resource (preview)</span></span>

<span data-ttu-id="fe626-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe626-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe626-105">Recuperar os metadados de uma versão específica de um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="fe626-105">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe626-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe626-106">Permissions</span></span>

<span data-ttu-id="fe626-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe626-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe626-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe626-109">Permission type</span></span>      | <span data-ttu-id="fe626-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe626-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe626-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe626-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fe626-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe626-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe626-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe626-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe626-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe626-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe626-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe626-115">Application</span></span> | <span data-ttu-id="fe626-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe626-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="fe626-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe626-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/items/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="fe626-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe626-118">Response</span></span>

<span data-ttu-id="fe626-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [DriveItemVersion](../resources/driveitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe626-119">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="fe626-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe626-120">Example</span></span>

<span data-ttu-id="fe626-121">Este exemplo recupera uma versão de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="fe626-121">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="fe626-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe626-122">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="fe626-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe626-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/versions/{version-id}
```
# <a name="c"></a>[<span data-ttu-id="fe626-124">C#</span><span class="sxs-lookup"><span data-stu-id="fe626-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-single-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe626-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe626-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-single-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe626-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe626-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-single-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe626-127">Java</span><span class="sxs-lookup"><span data-stu-id="fe626-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-single-version-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fe626-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe626-128">Response</span></span>

<span data-ttu-id="fe626-129">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="fe626-129">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="fe626-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="fe626-130">Remarks</span></span>

<span data-ttu-id="fe626-131">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="fe626-131">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="fe626-132">Quando seu aplicativo recupera a lista de versões disponíveis de um arquivo, um recurso [DriveItemVersion](../resources/driveitemversion.md) é retornado e fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="fe626-132">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
}
-->


