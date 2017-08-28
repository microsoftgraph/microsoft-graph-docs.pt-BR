# <a name="delete-a-driveitem"></a><span data-ttu-id="a79ca-101">Excluir um DriveItem</span><span class="sxs-lookup"><span data-stu-id="a79ca-101">Delete a DriveItem</span></span>

<span data-ttu-id="a79ca-p101">Excluir um [DriveItem](../resources/driveitem.md) usando sua ID ou seu caminho. Observe que a exclusão de itens usando esse método moverá os itens para a Lixeira, ao invés de excluir permanentemente o item.</span><span class="sxs-lookup"><span data-stu-id="a79ca-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="a79ca-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="a79ca-104">Permissions</span></span>
<span data-ttu-id="a79ca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a79ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a79ca-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a79ca-107">Permission type</span></span>      | <span data-ttu-id="a79ca-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a79ca-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="a79ca-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a79ca-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a79ca-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a79ca-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="a79ca-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a79ca-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a79ca-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a79ca-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="a79ca-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a79ca-113">Application</span></span> | <span data-ttu-id="a79ca-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a79ca-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a79ca-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a79ca-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
DELETE /me/drive/items/{item-id}
DELETE /me/drive/root:/{item-path}
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="a79ca-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a79ca-116">Request headers</span></span>

| <span data-ttu-id="a79ca-117">Nome</span><span class="sxs-lookup"><span data-stu-id="a79ca-117">Name</span></span>          | <span data-ttu-id="a79ca-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="a79ca-118">Type</span></span>   | <span data-ttu-id="a79ca-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a79ca-119">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a79ca-120">if-match</span><span class="sxs-lookup"><span data-stu-id="a79ca-120">if-match</span></span>      | <span data-ttu-id="a79ca-121">String</span><span class="sxs-lookup"><span data-stu-id="a79ca-121">String</span></span> | <span data-ttu-id="a79ca-122">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="a79ca-122">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a79ca-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a79ca-123">Request body</span></span>
<span data-ttu-id="a79ca-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a79ca-124">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="a79ca-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a79ca-125">Example</span></span>

<span data-ttu-id="a79ca-126">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a79ca-126">Here is an example of how to call this API.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-item"
}-->
```
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="a79ca-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a79ca-127">Response</span></span>

<span data-ttu-id="a79ca-128">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="a79ca-128">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete item"
}-->
