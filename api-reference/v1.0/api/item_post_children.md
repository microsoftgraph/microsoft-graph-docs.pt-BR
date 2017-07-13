# <span data-ttu-id="7dcc4-101">Criar uma nova pasta</span><span class="sxs-lookup"><span data-stu-id="7dcc4-101">Create a new folder</span></span>
<a id="create-a-new-folder" class="xliff"></a>

<span data-ttu-id="7dcc4-102">Criar uma nova pasta ou [DriveItem](../resources/driveitem.md) em um [Drive](../resources/drive.md) com um item pai ou caminho especificado.</span><span class="sxs-lookup"><span data-stu-id="7dcc4-102">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <span data-ttu-id="7dcc4-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7dcc4-103">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="7dcc4-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="7dcc4-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="7dcc4-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7dcc4-105">Files.ReadWrite</span></span>
* <span data-ttu-id="7dcc4-106">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dcc4-106">Files.ReadWrite.All</span></span>
* <span data-ttu-id="7dcc4-107">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dcc4-107">Sites.ReadWrite.All</span></span>


## <span data-ttu-id="7dcc4-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dcc4-108">HTTP request</span></span>
<a id="http-request" class="xliff"></a>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/children
POST /me/drive/items/{parent-item-id}/children
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
```

## <span data-ttu-id="7dcc4-109">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7dcc4-109">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="7dcc4-110">No corpo da solicitação, forneça uma representação JSON do recurso [DriveItem](../resources/driveitem.md) a criar.</span><span class="sxs-lookup"><span data-stu-id="7dcc4-110">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>


## <span data-ttu-id="7dcc4-111">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dcc4-111">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="7dcc4-112">Se bem sucedido, este método retorna o código de resposta `201 Created` e o recurso [Driveitem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dcc4-112">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <span data-ttu-id="7dcc4-113">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dcc4-113">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="7dcc4-114">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dcc4-114">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="7dcc4-115">Eis um exemplo de solicitação para criar uma nova pasta na raiz do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="7dcc4-115">Here is an example of the request to create a new folder in the user's OneDrive root.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_from_item"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/children
Content-Type: application/json

{
  "name": "New Folder",
  "folder": { }
}
```

##### <span data-ttu-id="7dcc4-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dcc4-116">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="7dcc4-117">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dcc4-117">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->

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
  "createdDateTime": "20160920T14:34:00Z",
  "eTag": "343F1FBD-E9B3-4DDE-BCA7-D61AEAFF44E5,1",
  "id": "ACEA49D1-1444-45A9-A1CB-68B1B28AE491",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "lastModifiedDateTime": "20160920T14:34:00Z",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create children",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
