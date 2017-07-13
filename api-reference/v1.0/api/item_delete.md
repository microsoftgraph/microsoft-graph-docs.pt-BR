<span data-ttu-id="32b83-p101">Excluir um [DriveItem](../resources/driveitem.md) usando sua ID ou seu caminho. Observe que a exclusão de itens usando esse método moverá os itens para a Lixeira, ao invés de excluir permanentemente o item.</span><span class="sxs-lookup"><span data-stu-id="32b83-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

Excluir um [DriveItem](../resources/driveitem.md) usando sua ID ou seu caminho. Observe que a exclusão de itens usando esse método moverá os itens para a Lixeira, ao invés de excluir permanentemente o item.

## <span data-ttu-id="32b83-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32b83-104">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="32b83-105">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="32b83-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="32b83-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32b83-106">Files.ReadWrite</span></span>
* <span data-ttu-id="32b83-107">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32b83-107">Files.ReadWrite.All</span></span>
* <span data-ttu-id="32b83-108">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32b83-108">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="32b83-109">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32b83-109">HTTP request</span></span>
<a id="http-request" class="xliff"></a>

<!-- { "blockType": "ignored" } -->
```
DELETE /me/drive/items/{item-id}
DELETE /me/drive/root:/{item-path}
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
```

## <span data-ttu-id="32b83-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32b83-110">Request headers</span></span>
<a id="request-headers" class="xliff"></a>

| <span data-ttu-id="32b83-111">Nome</span><span class="sxs-lookup"><span data-stu-id="32b83-111">Name</span></span>          | <span data-ttu-id="32b83-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="32b83-112">Type</span></span>   | <span data-ttu-id="32b83-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="32b83-113">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="32b83-114">if-match</span><span class="sxs-lookup"><span data-stu-id="32b83-114">if-match</span></span>      | <span data-ttu-id="32b83-115">String</span><span class="sxs-lookup"><span data-stu-id="32b83-115">String</span></span> | <span data-ttu-id="32b83-116">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="32b83-116">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <span data-ttu-id="32b83-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32b83-117">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="32b83-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32b83-118">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="32b83-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32b83-119">Example</span></span>
<a id="example" class="xliff"></a>

<span data-ttu-id="32b83-120">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="32b83-120">Here is an example of how to call this API.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-item"
}-->
```
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
```

## <span data-ttu-id="32b83-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="32b83-121">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="32b83-122">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="32b83-122">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
