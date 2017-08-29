# <a name="update-permission"></a><span data-ttu-id="54d18-101">Atualizar permissão</span><span class="sxs-lookup"><span data-stu-id="54d18-101">Update permission</span></span>

<span data-ttu-id="54d18-102">Atualize as propriedades de uma permissão corrigindo do recurso.</span><span class="sxs-lookup"><span data-stu-id="54d18-102">Update the properties of a permission by patching the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="54d18-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="54d18-103">Permissions</span></span>

<span data-ttu-id="54d18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="54d18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="54d18-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54d18-106">Permission type</span></span>      | <span data-ttu-id="54d18-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54d18-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54d18-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54d18-108">Delegated (work or school account)</span></span> | <span data-ttu-id="54d18-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54d18-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="54d18-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54d18-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54d18-111">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54d18-111">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="54d18-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54d18-112">Application</span></span> | <span data-ttu-id="54d18-113">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54d18-113">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54d18-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54d18-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/root:/{path}:/permissions/{perm-id}
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="request-headers"></a><span data-ttu-id="54d18-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54d18-115">Request headers</span></span>

| <span data-ttu-id="54d18-116">Nome</span><span class="sxs-lookup"><span data-stu-id="54d18-116">Name</span></span>          | <span data-ttu-id="54d18-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="54d18-117">Type</span></span>   | <span data-ttu-id="54d18-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="54d18-118">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="54d18-119">if-match</span><span class="sxs-lookup"><span data-stu-id="54d18-119">if-match</span></span>      | <span data-ttu-id="54d18-120">string</span><span class="sxs-lookup"><span data-stu-id="54d18-120">string</span></span> | <span data-ttu-id="54d18-121">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="54d18-121">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54d18-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54d18-122">Request body</span></span>
<span data-ttu-id="54d18-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="54d18-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="54d18-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54d18-126">Property</span></span>     | <span data-ttu-id="54d18-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="54d18-127">Type</span></span>   | <span data-ttu-id="54d18-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="54d18-128">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="54d18-129">**roles**</span><span class="sxs-lookup"><span data-stu-id="54d18-129">**roles**</span></span>    | <span data-ttu-id="54d18-130">String</span><span class="sxs-lookup"><span data-stu-id="54d18-130">String</span></span> | <span data-ttu-id="54d18-131">Uma matriz de tipos de permissão.</span><span class="sxs-lookup"><span data-stu-id="54d18-131">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="54d18-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="54d18-132">Response</span></span>

<span data-ttu-id="54d18-133">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [permission](../resources/permission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54d18-133">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54d18-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54d18-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="54d18-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54d18-135">Request</span></span>

<span data-ttu-id="54d18-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54d18-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_permission"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
##### <a name="response"></a><span data-ttu-id="54d18-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="54d18-137">Response</span></span>

<span data-ttu-id="54d18-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54d18-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
