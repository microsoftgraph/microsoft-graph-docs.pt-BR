# <a name="update-driveitem-properties"></a><span data-ttu-id="8e372-101">Atualizar propriedades de DriveItem</span><span class="sxs-lookup"><span data-stu-id="8e372-101">Update DriveItem properties</span></span>

<span data-ttu-id="8e372-102">Atualize os metadados de um [DriveItem](../resources/driveitem.md) por ID ou caminho.</span><span class="sxs-lookup"><span data-stu-id="8e372-102">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="8e372-103">Também é possível usar a atualização para [mover um item](item_move.md) para outro pai ao atualizar a propriedade **parentReference** do item.</span><span class="sxs-lookup"><span data-stu-id="8e372-103">You can also use update to [move an item](item_move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e372-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e372-104">Permissions</span></span>
<span data-ttu-id="8e372-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e372-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8e372-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e372-107">Permission type</span></span>      | <span data-ttu-id="8e372-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e372-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e372-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e372-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8e372-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e372-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8e372-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e372-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e372-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e372-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8e372-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e372-113">Application</span></span> | <span data-ttu-id="8e372-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e372-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e372-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e372-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="8e372-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e372-116">Request headers</span></span>

| <span data-ttu-id="8e372-117">Nome</span><span class="sxs-lookup"><span data-stu-id="8e372-117">Name</span></span>          | <span data-ttu-id="8e372-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e372-118">Type</span></span>   | <span data-ttu-id="8e372-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e372-119">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8e372-120">if-match</span><span class="sxs-lookup"><span data-stu-id="8e372-120">if-match</span></span>      | <span data-ttu-id="8e372-121">String</span><span class="sxs-lookup"><span data-stu-id="8e372-121">String</span></span> | <span data-ttu-id="8e372-122">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à eTag atual da pasta, uma resposta `412 Precondition Failed` será exibida.</span><span class="sxs-lookup"><span data-stu-id="8e372-122">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e372-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e372-123">Request body</span></span>
<span data-ttu-id="8e372-p102">No corpo da solicitação, forneça os valores para as propriedades que devem ser atualizadas. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, seu aplicativo não deve incluir propriedades que não tenham sido alteradas.</span><span class="sxs-lookup"><span data-stu-id="8e372-p102">In the request body, supply the values for properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="8e372-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e372-127">Response</span></span>

<span data-ttu-id="8e372-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e372-128">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e372-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e372-129">Example</span></span>
<span data-ttu-id="8e372-130">Este exemplo renomeia o driveItem.</span><span class="sxs-lookup"><span data-stu-id="8e372-130">This example renames the driveItem.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-file-name.docx"
}
```

##### <a name="response"></a><span data-ttu-id="8e372-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e372-131">Response</span></span>

<span data-ttu-id="8e372-p103">O exemplo a seguir mostra a resposta. Esta resposta está truncada para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="8e372-p103">The following example shows the response. This response is truncated for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
    "name": "new-file-name.docx",
    "file": { }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update item"
}-->
