---
title: Obter um recurso DriveItemVersion (prévia)
description: Recuperar os metadados de uma versão específica de um DriveItem.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 62f9e68ce53c2caa422053b355729054073bf754
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33588142"
---
# <a name="get-a-driveitemversion-resource-preview"></a><span data-ttu-id="f819e-103">Obter um recurso DriveItemVersion (prévia)</span><span class="sxs-lookup"><span data-stu-id="f819e-103">Get a DriveItemVersion resource (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f819e-104">Recuperar os metadados de uma versão específica de um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f819e-104">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f819e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f819e-105">Permissions</span></span>

<span data-ttu-id="f819e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f819e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f819e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f819e-108">Permission type</span></span>      | <span data-ttu-id="f819e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f819e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f819e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f819e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f819e-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f819e-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f819e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f819e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f819e-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f819e-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f819e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f819e-114">Application</span></span> | <span data-ttu-id="f819e-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f819e-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="f819e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f819e-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="f819e-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="f819e-117">Response</span></span>

<span data-ttu-id="f819e-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [DriveItemVersion](../resources/driveitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f819e-118">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="f819e-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f819e-119">Example</span></span>

<span data-ttu-id="f819e-120">Este exemplo recupera uma versão de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="f819e-120">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="f819e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f819e-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="f819e-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="f819e-122">Response</span></span>

<span data-ttu-id="f819e-123">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="f819e-123">This returns a collection of versions:</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f819e-124">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f819e-124">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f819e-125">Basic</span><span class="sxs-lookup"><span data-stu-id="f819e-125">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-single-version-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f819e-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f819e-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-single-version-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="f819e-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="f819e-127">Remarks</span></span>

<span data-ttu-id="f819e-128">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="f819e-128">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="f819e-129">Quando seu aplicativo recupera a lista de versões disponíveis de um arquivo, um recurso [DriveItemVersion](../resources/driveitemversion.md) é retornado e fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="f819e-129">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitemversion-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitemversion-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
