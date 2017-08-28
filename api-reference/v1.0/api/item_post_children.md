# <a name="create-a-new-folder"></a><span data-ttu-id="db85c-101">Criar uma nova pasta</span><span class="sxs-lookup"><span data-stu-id="db85c-101">Create a new folder</span></span>

<span data-ttu-id="db85c-102">Criar uma nova pasta ou [DriveItem](../resources/driveitem.md) em um [Drive](../resources/drive.md) com um item pai ou caminho especificado.</span><span class="sxs-lookup"><span data-stu-id="db85c-102">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="db85c-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="db85c-103">Permissions</span></span>
<span data-ttu-id="db85c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="db85c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="db85c-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db85c-106">Permission type</span></span>      | <span data-ttu-id="db85c-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db85c-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="db85c-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db85c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="db85c-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db85c-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="db85c-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db85c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db85c-111">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db85c-111">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="db85c-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db85c-112">Application</span></span> | <span data-ttu-id="db85c-113">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db85c-113">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="db85c-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db85c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/children
POST /me/drive/items/{parent-item-id}/children
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="db85c-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db85c-115">Request body</span></span>
<span data-ttu-id="db85c-116">No corpo da solicitação, forneça uma representação JSON do recurso [DriveItem](../resources/driveitem.md) a criar.</span><span class="sxs-lookup"><span data-stu-id="db85c-116">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="db85c-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="db85c-117">Response</span></span>

<span data-ttu-id="db85c-118">Se bem sucedido, este método retorna o código de resposta `201 Created` e o recurso [Driveitem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db85c-118">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db85c-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db85c-119">Example</span></span>

##### <a name="request"></a><span data-ttu-id="db85c-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db85c-120">Request</span></span>
<span data-ttu-id="db85c-121">Eis um exemplo de solicitação para criar uma nova pasta na raiz do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="db85c-121">Here is an example of the request to create a new folder in the user's OneDrive root.</span></span>

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

##### <a name="response"></a><span data-ttu-id="db85c-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="db85c-122">Response</span></span>

<span data-ttu-id="db85c-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db85c-123">Here is an example of the response.</span></span>
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
