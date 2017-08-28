# <a name="delete-photo"></a><span data-ttu-id="11c4f-101">Excluir foto</span><span class="sxs-lookup"><span data-stu-id="11c4f-101">Delete photo</span></span>

<span data-ttu-id="11c4f-102">Exclua uma foto.</span><span class="sxs-lookup"><span data-stu-id="11c4f-102">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="11c4f-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="11c4f-103">Permissions</span></span>
<span data-ttu-id="11c4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="11c4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="11c4f-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11c4f-106">Permission type</span></span>      | <span data-ttu-id="11c4f-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11c4f-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="11c4f-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11c4f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="11c4f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11c4f-109">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="11c4f-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11c4f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11c4f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11c4f-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="11c4f-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11c4f-112">Application</span></span> | <span data-ttu-id="11c4f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11c4f-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="11c4f-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11c4f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="11c4f-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11c4f-115">Request headers</span></span>
| <span data-ttu-id="11c4f-116">Nome</span><span class="sxs-lookup"><span data-stu-id="11c4f-116">Name</span></span>       | <span data-ttu-id="11c4f-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="11c4f-117">Type</span></span> | <span data-ttu-id="11c4f-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="11c4f-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="11c4f-119">if-match</span><span class="sxs-lookup"><span data-stu-id="11c4f-119">if-match</span></span>  | <span data-ttu-id="11c4f-120">string</span><span class="sxs-lookup"><span data-stu-id="11c4f-120">string</span></span>  | <span data-ttu-id="11c4f-121">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="11c4f-121">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="11c4f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="11c4f-122">Authorization</span></span>  | <span data-ttu-id="11c4f-123">string</span><span class="sxs-lookup"><span data-stu-id="11c4f-123">string</span></span>  | <span data-ttu-id="11c4f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11c4f-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="11c4f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11c4f-126">Request body</span></span>
<span data-ttu-id="11c4f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11c4f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11c4f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="11c4f-128">Response</span></span>

<span data-ttu-id="11c4f-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11c4f-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11c4f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11c4f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11c4f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11c4f-132">Request</span></span>
<span data-ttu-id="11c4f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11c4f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="11c4f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="11c4f-134">Response</span></span>
<span data-ttu-id="11c4f-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11c4f-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
