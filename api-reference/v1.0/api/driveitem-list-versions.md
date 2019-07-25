---
title: Listando versões de um DriveItem
description: O OneDrive e o SharePoint podem ser configurados para manter o histórico de arquivos.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2020cfeaaf8a47ca92312a3650813f910d9b9006
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881717"
---
# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="87224-103">Listando versões de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="87224-103">Listing versions of a DriveItem</span></span>

<span data-ttu-id="87224-104">O OneDrive e o SharePoint podem ser configurados para manter o histórico de arquivos.</span><span class="sxs-lookup"><span data-stu-id="87224-104">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="87224-105">Dependendo do serviço e da configuração, uma nova versão pode ser criada para cada edição, sempre que o arquivo for salvo, manualmente ou nunca.</span><span class="sxs-lookup"><span data-stu-id="87224-105">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="87224-106">Versões anteriores de um documento podem ser retidas por um determinado período dependendo das configurações de administração, que podem ser exclusivas por usuário ou local.</span><span class="sxs-lookup"><span data-stu-id="87224-106">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="87224-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="87224-107">Permissions</span></span>

<span data-ttu-id="87224-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87224-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87224-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87224-110">Permission type</span></span>      | <span data-ttu-id="87224-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87224-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87224-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87224-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87224-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87224-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="87224-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87224-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87224-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87224-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="87224-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87224-116">Application</span></span> | <span data-ttu-id="87224-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87224-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="87224-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87224-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="87224-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="87224-119">Response</span></span>

<span data-ttu-id="87224-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [DriveItemVersion](../resources/driveitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87224-120">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="87224-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87224-121">Example</span></span>

<span data-ttu-id="87224-122">Este exemplo recupera as versões de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="87224-122">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="87224-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87224-123">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="87224-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="87224-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="87224-125">C#</span><span class="sxs-lookup"><span data-stu-id="87224-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-previous-versions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="87224-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="87224-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-previous-versions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="87224-127">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="87224-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-previous-versions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="87224-128">Java</span><span class="sxs-lookup"><span data-stu-id="87224-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-previous-versions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="87224-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="87224-129">Response</span></span>

<span data-ttu-id="87224-130">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="87224-130">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
      "size": 123
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z",
      "size": 62
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z",
      "size": 16
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="87224-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="87224-131">Remarks</span></span>

<span data-ttu-id="87224-132">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="87224-132">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="87224-133">Quando seu aplicativo recupera a lista de versões disponíveis de um arquivo, um recurso [DriveItemVersion](../resources/driveitemversion.md) é retornado e fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="87224-133">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->
