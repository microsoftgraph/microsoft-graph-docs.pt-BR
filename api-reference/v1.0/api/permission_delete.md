# <a name="delete-permission"></a><span data-ttu-id="05a9d-101">Excluir permissão</span><span class="sxs-lookup"><span data-stu-id="05a9d-101">Delete permission</span></span>

<span data-ttu-id="05a9d-102">Remova o acesso a um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="05a9d-102">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="05a9d-p101">Somente as permissões que não são herdadas podem ser excluídas. A propriedade **inheritedFrom** deve ser `null`.</span><span class="sxs-lookup"><span data-stu-id="05a9d-p101">Only permissions that are not inherited can be deleted. The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="05a9d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="05a9d-105">Permissions</span></span>
<span data-ttu-id="05a9d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="05a9d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="05a9d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05a9d-108">Permission type</span></span>      | <span data-ttu-id="05a9d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05a9d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05a9d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05a9d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="05a9d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05a9d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="05a9d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05a9d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05a9d-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05a9d-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="05a9d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05a9d-114">Application</span></span> | <span data-ttu-id="05a9d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05a9d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05a9d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05a9d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/root:/{path}:/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
```

## <a name="request-headers"></a><span data-ttu-id="05a9d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05a9d-117">Request headers</span></span>

| <span data-ttu-id="05a9d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="05a9d-118">Name</span></span>          | <span data-ttu-id="05a9d-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="05a9d-119">Type</span></span>   | <span data-ttu-id="05a9d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="05a9d-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="05a9d-121">if-match</span><span class="sxs-lookup"><span data-stu-id="05a9d-121">if-match</span></span>      | <span data-ttu-id="05a9d-122">string</span><span class="sxs-lookup"><span data-stu-id="05a9d-122">string</span></span> | <span data-ttu-id="05a9d-123">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="05a9d-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05a9d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05a9d-124">Request body</span></span>
<span data-ttu-id="05a9d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="05a9d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05a9d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="05a9d-126">Response</span></span>

<span data-ttu-id="05a9d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05a9d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05a9d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05a9d-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="05a9d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05a9d-130">Request</span></span>

<span data-ttu-id="05a9d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05a9d-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_permission"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/root/items/{item-id}/permissions/{perm-id}
```

##### <a name="response"></a><span data-ttu-id="05a9d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="05a9d-132">Response</span></span>

<span data-ttu-id="05a9d-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05a9d-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="05a9d-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="05a9d-134">Remarks</span></span>

* <span data-ttu-id="05a9d-135">[Drives](../resources/drive.md) com **driveType** `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="05a9d-135">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission"
}-->
