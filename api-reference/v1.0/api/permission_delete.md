# <a name="delete-permission"></a><span data-ttu-id="15381-101">Excluir permissão</span><span class="sxs-lookup"><span data-stu-id="15381-101">Delete permission</span></span>

<span data-ttu-id="15381-102">Remova o acesso a um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="15381-102">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="15381-p101">Somente as permissões que não são herdadas podem ser excluídas. A propriedade **inheritedFrom** deve ser `null`.</span><span class="sxs-lookup"><span data-stu-id="15381-p101">Only permissions that are not inherited can be deleted. The **inheritedFrom** property must be `null`.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15381-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15381-105">Prerequisites</span></span>
<span data-ttu-id="15381-106">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="15381-106">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="15381-107">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15381-107">Files.ReadWrite</span></span>
* <span data-ttu-id="15381-108">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15381-108">Files.ReadWrite.All</span></span>
* <span data-ttu-id="15381-109">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15381-109">Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="15381-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15381-110">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/root:/{path}:/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
```

## <a name="request-headers"></a><span data-ttu-id="15381-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15381-111">Request headers</span></span>

| <span data-ttu-id="15381-112">Nome</span><span class="sxs-lookup"><span data-stu-id="15381-112">Name</span></span>          | <span data-ttu-id="15381-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="15381-113">Type</span></span>   | <span data-ttu-id="15381-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="15381-114">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="15381-115">if-match</span><span class="sxs-lookup"><span data-stu-id="15381-115">if-match</span></span>      | <span data-ttu-id="15381-116">string</span><span class="sxs-lookup"><span data-stu-id="15381-116">string</span></span> | <span data-ttu-id="15381-117">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="15381-117">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15381-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15381-118">Request body</span></span>
<span data-ttu-id="15381-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15381-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15381-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="15381-120">Response</span></span>

<span data-ttu-id="15381-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15381-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15381-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15381-123">Example</span></span>

##### <a name="request"></a><span data-ttu-id="15381-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15381-124">Request</span></span>

<span data-ttu-id="15381-125">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15381-125">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_permission"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/root/items/{item-id}/permissions/{perm-id}
```

##### <a name="response"></a><span data-ttu-id="15381-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="15381-126">Response</span></span>

<span data-ttu-id="15381-127">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15381-127">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="15381-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="15381-128">Remarks</span></span>

* <span data-ttu-id="15381-129">[Drives](../resources/drive.md) com **driveType** `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="15381-129">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission"
}-->
