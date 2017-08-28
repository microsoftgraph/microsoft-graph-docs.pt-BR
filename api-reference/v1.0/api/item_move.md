# <a name="move-a-driveitem"></a><span data-ttu-id="b299c-101">Mover um DriveItem</span><span class="sxs-lookup"><span data-stu-id="b299c-101">Move a DriveItem</span></span>

<span data-ttu-id="b299c-p101">Para mover um DriveItem para um novo item pai, o aplicativo solicita a atualização de **parentReference** do DriveItem a ser movido. Este é um caso especial do método [Update](item_update.md). O aplicativo pode combinar a movimentação de um item para um novo contêiner e a atualização de outras propriedades do item em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="b299c-p101">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move. This is a special case of the [Update](item_update.md) method. Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="b299c-105">Não é possível mover itens entre [Unidades](../resources/drive.md) usando esta solicitação.</span><span class="sxs-lookup"><span data-stu-id="b299c-105">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="b299c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b299c-106">Permissions</span></span>
<span data-ttu-id="b299c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b299c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b299c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b299c-109">Permission type</span></span>      | <span data-ttu-id="b299c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b299c-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="b299c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b299c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b299c-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b299c-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="b299c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b299c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b299c-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b299c-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="b299c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b299c-115">Application</span></span> | <span data-ttu-id="b299c-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b299c-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b299c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b299c-117">HTTP request</span></span>

```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="b299c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b299c-118">Request headers</span></span>

| <span data-ttu-id="b299c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b299c-119">Name</span></span>          | <span data-ttu-id="b299c-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b299c-120">Type</span></span>   | <span data-ttu-id="b299c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b299c-121">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b299c-122">if-match</span><span class="sxs-lookup"><span data-stu-id="b299c-122">if-match</span></span>      | <span data-ttu-id="b299c-123">String</span><span class="sxs-lookup"><span data-stu-id="b299c-123">String</span></span> | <span data-ttu-id="b299c-124">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à eTag atual da pasta, uma resposta `412 Precondition Failed` será exibida.</span><span class="sxs-lookup"><span data-stu-id="b299c-124">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b299c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b299c-125">Request body</span></span>
<span data-ttu-id="b299c-p103">No corpo da solicitação, forneça o novo valor para a propriedade **parentReference**. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b299c-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="b299c-p104">**Observação:** Ao mover itens para a raiz de um OneDrive, não é possível usar a sintaxe `"id:" "root"`. É preciso usar a ID real da pasta raiz ou usar `{"path": "/drive/root"}` para a referência do pai.</span><span class="sxs-lookup"><span data-stu-id="b299c-p104">**Note:** When moving items to the root of a OneDrive you cannot use the `"id:" "root"` syntax. You either need to use the real ID of the root folder, or use `{"path": "/drive/root"}` for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="b299c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b299c-131">Response</span></span>

<span data-ttu-id="b299c-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b299c-132">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b299c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b299c-133">Example</span></span>
<span data-ttu-id="b299c-134">Este exemplo move um item especificado por {item-id} para a pasta **Documentos** no OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="b299c-134">This example moves an item specified by {item-id} into the **Documents** folder in the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-item-name",
    "parentReference" : {"path": "/drive/root:/Documents"}
}
```

##### <a name="response"></a><span data-ttu-id="b299c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b299c-135">Response</span></span>

<span data-ttu-id="b299c-136">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="b299c-136">The following example shows the formula bar</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0123456789abc",
    "name": "new-item-name",
    "folder": { "childCount": 3 },
  "parentReference": {
    "id": "507DE6D5-0201-496A-AA87-5E2563247982",
    "path": "/drive/root:/Documents"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Move item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
