---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Criar uma nova pasta
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: d052242d13b37085737eed66780452762b97a3f0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443956"
---
# <a name="create-a-new-folder-in-a-drive"></a><span data-ttu-id="5eb78-102">Criar uma nova pasta em uma unidade</span><span class="sxs-lookup"><span data-stu-id="5eb78-102">Create a new folder in a drive</span></span>

<span data-ttu-id="5eb78-103">Criar uma nova pasta ou [DriveItem](../resources/driveitem.md) em um [Drive](../resources/drive.md) com um item pai ou caminho especificado.</span><span class="sxs-lookup"><span data-stu-id="5eb78-103">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="5eb78-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="5eb78-104">Permissions</span></span>

<span data-ttu-id="5eb78-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5eb78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eb78-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5eb78-107">Permission type</span></span>      | <span data-ttu-id="5eb78-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5eb78-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5eb78-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5eb78-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5eb78-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eb78-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5eb78-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5eb78-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5eb78-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eb78-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5eb78-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5eb78-113">Application</span></span> | <span data-ttu-id="5eb78-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eb78-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5eb78-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5eb78-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
POST /me/drive/items/{parent-item-id}/children
POST /sites/{site-id}/drive/items/{parent-item-id}/children
POST /users/{user-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="5eb78-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5eb78-116">Request body</span></span>

<span data-ttu-id="5eb78-117">No corpo da solicitação, forneça uma representação JSON do recurso [DriveItem](../resources/driveitem.md) a criar.</span><span class="sxs-lookup"><span data-stu-id="5eb78-117">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="5eb78-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="5eb78-118">Response</span></span>

<span data-ttu-id="5eb78-119">Se bem sucedido, este método retorna o código de resposta `201 Created` e o recurso [Driveitem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5eb78-119">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5eb78-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5eb78-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="5eb78-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5eb78-121">Request</span></span>

<span data-ttu-id="5eb78-122">Eis um exemplo de solicitação para criar uma nova pasta na raiz do OneDrive do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="5eb78-122">Here is an example of the request to create a new folder in the signed-in user's OneDrive root folder.</span></span>
<span data-ttu-id="5eb78-123">A propriedade `@microsoft.graph.conflictBehavior` usada indica que, se já existe um item com o mesmo nome, o serviço deve escolher um novo nome para a pasta ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="5eb78-123">The `@microsoft.graph.conflictBehavior` property used indicates that if an item already exists with the same name, the service should choose a new name for the folder while creating it.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5eb78-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="5eb78-124">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-folder", "scopes": "files.readwrite" } -->

```http
POST /me/drive/root/children
Content-Type: application/json

{
  "name": "New Folder",
  "folder": { },
  "@microsoft.graph.conflictBehavior": "rename"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5eb78-125">C#</span><span class="sxs-lookup"><span data-stu-id="5eb78-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-folder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5eb78-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="5eb78-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-folder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5eb78-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5eb78-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-folder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5eb78-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5eb78-128">Response</span></span>

<span data-ttu-id="5eb78-129">Se for bem-sucedido, esse método retornará uma pasta recém-criada como um recurso [DriveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="5eb78-129">If successful, this method returns the newly created folder as a [DriveItem][item-resource] resource.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "createdDateTime": "2016-09-20T14:34:00Z",
  "eTag": "343F1FBD-E9B3-4DDE-BCA7-D61AEAFF44E5,1",
  "id": "ACEA49D1-1444-45A9-A1CB-68B1B28AE491",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "lastModifiedDateTime": "2016-09-20T14:34:00Z",
  "name": "New Folder",
  "parentReference": {
    "driveId": "5FE38E3C-051C-4D55-9B83-8A437658275B",
    "id": "E67A8F34-B0AA-46E1-8FF7-0750A29553DF",
    "path": "/drive/root:/"
  },
  "size": 0,
  "folder": {
    "childCount": 0
  }
}
```

## <a name="error-response"></a><span data-ttu-id="5eb78-130">Resposta de erro</span><span class="sxs-lookup"><span data-stu-id="5eb78-130">Error response</span></span>

<span data-ttu-id="5eb78-131">Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="5eb78-131">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[folder-facet]: ../resources/folder.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a folder item in a drive.",
  "keywords": "create,folder,new item",
  "section": "documentation",
  "tocPath": "Items/Create folder",
  "suppressions": [
  ]
} -->
