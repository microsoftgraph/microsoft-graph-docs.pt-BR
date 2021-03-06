---
title: Listar versões de um DriveItem
description: O OneDrive e o SharePoint podem ser configurados para manter o histórico de arquivos.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: JeremyKelley
ms.openlocfilehash: 3f3c2135f84d5c4b5a71a7a2e003528a72edb8b0
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515531"
---
# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="956c3-103">Listar versões de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="956c3-103">Listing versions of a DriveItem</span></span>

<span data-ttu-id="956c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="956c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="956c3-105">O OneDrive e o SharePoint podem ser configurados para manter o histórico de arquivos.</span><span class="sxs-lookup"><span data-stu-id="956c3-105">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="956c3-106">Dependendo do serviço e da configuração, uma nova versão pode ser criada para cada edição, sempre que o arquivo for salvo, manualmente ou nunca.</span><span class="sxs-lookup"><span data-stu-id="956c3-106">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="956c3-107">Versões anteriores de um documento podem ser retidas por um determinado período dependendo das configurações de administração, que podem ser exclusivas por usuário ou local.</span><span class="sxs-lookup"><span data-stu-id="956c3-107">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="956c3-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="956c3-108">Permissions</span></span>

<span data-ttu-id="956c3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="956c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="956c3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="956c3-111">Permission type</span></span>      | <span data-ttu-id="956c3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="956c3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="956c3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="956c3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="956c3-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="956c3-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="956c3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="956c3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="956c3-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="956c3-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="956c3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="956c3-117">Application</span></span> | <span data-ttu-id="956c3-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="956c3-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="956c3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="956c3-119">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/items/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="956c3-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="956c3-120">Response</span></span>

<span data-ttu-id="956c3-121">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [DriveItemVersion](../resources/driveitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="956c3-121">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="956c3-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="956c3-122">Example</span></span>

<span data-ttu-id="956c3-123">Este exemplo recupera as versões de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="956c3-123">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="956c3-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="956c3-124">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="956c3-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="956c3-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/versions
```
# <a name="c"></a>[<span data-ttu-id="956c3-126">C#</span><span class="sxs-lookup"><span data-stu-id="956c3-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-previous-versions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="956c3-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="956c3-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-previous-versions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="956c3-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="956c3-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-previous-versions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="956c3-129">Java</span><span class="sxs-lookup"><span data-stu-id="956c3-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-previous-versions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="956c3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="956c3-130">Response</span></span>

<span data-ttu-id="956c3-131">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="956c3-131">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="956c3-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="956c3-132">Remarks</span></span>

<span data-ttu-id="956c3-133">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="956c3-133">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="956c3-134">Quando seu aplicativo recupera a lista de versões disponíveis de um arquivo, um recurso [DriveItemVersion](../resources/driveitemversion.md) é retornado e fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="956c3-134">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


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


