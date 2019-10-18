---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Criar uma nova pasta
localization_priority: Priority
ms.prod: sharepoint
description: Criar uma nova pasta ou DriveItem em um Drive com um item pai ou caminho especificado.
doc_type: apiPageType
ms.openlocfilehash: 2395673892bcaa44ec617ca6c69b6eafe62dc7ae
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373417"
---
# <a name="create-a-new-folder-in-a-drive"></a><span data-ttu-id="e2aef-103">Criar uma nova pasta em uma unidade</span><span class="sxs-lookup"><span data-stu-id="e2aef-103">Create a new folder in a drive</span></span>

<span data-ttu-id="e2aef-104">Criar uma nova pasta ou [DriveItem](../resources/driveitem.md) em um [Drive](../resources/drive.md) com um item pai ou caminho especificado.</span><span class="sxs-lookup"><span data-stu-id="e2aef-104">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2aef-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2aef-105">Permissions</span></span>

<span data-ttu-id="e2aef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2aef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2aef-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2aef-108">Permission type</span></span>      | <span data-ttu-id="e2aef-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2aef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2aef-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2aef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e2aef-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2aef-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2aef-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2aef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2aef-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2aef-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2aef-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2aef-114">Application</span></span> | <span data-ttu-id="e2aef-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2aef-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2aef-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2aef-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
POST /me/drive/items/{parent-item-id}/children
POST /sites/{site-id}/drive/items/{parent-item-id}/children
POST /users/{user-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="e2aef-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2aef-117">Request body</span></span>

<span data-ttu-id="e2aef-118">No corpo da solicitação, forneça uma representação JSON do recurso [DriveItem](../resources/driveitem.md) a criar.</span><span class="sxs-lookup"><span data-stu-id="e2aef-118">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="e2aef-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2aef-119">Response</span></span>

<span data-ttu-id="e2aef-120">Se bem sucedido, este método retorna o código de resposta `201 Created` e o recurso [Driveitem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2aef-120">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2aef-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2aef-121">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2aef-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2aef-122">Request</span></span>

<span data-ttu-id="e2aef-123">Eis um exemplo de solicitação para criar uma nova pasta na raiz do OneDrive do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e2aef-123">Here is an example of the request to create a new folder in the signed-in user's OneDrive root folder.</span></span>
<span data-ttu-id="e2aef-124">A propriedade `@microsoft.graph.conflictBehavior` usada indica que, se já existe um item com o mesmo nome, o serviço deve escolher um novo nome para a pasta ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="e2aef-124">The `@microsoft.graph.conflictBehavior` property used indicates that if an item already exists with the same name, the service should choose a new name for the folder while creating it.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e2aef-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2aef-125">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2aef-126">C#</span><span class="sxs-lookup"><span data-stu-id="e2aef-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-folder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2aef-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2aef-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-folder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2aef-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2aef-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-folder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e2aef-129">Java</span><span class="sxs-lookup"><span data-stu-id="e2aef-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-folder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2aef-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2aef-130">Response</span></span>

<span data-ttu-id="e2aef-131">Se for bem-sucedido, esse método retornará uma pasta recém-criada como um recurso [DriveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="e2aef-131">If successful, this method returns the newly created folder as a [DriveItem][item-resource] resource.</span></span>

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

## <a name="error-response"></a><span data-ttu-id="e2aef-132">Resposta de erro</span><span class="sxs-lookup"><span data-stu-id="e2aef-132">Error response</span></span>

<span data-ttu-id="e2aef-133">Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="e2aef-133">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
