# <a name="delete-photo"></a><span data-ttu-id="4ea4c-101">Excluir foto</span><span class="sxs-lookup"><span data-stu-id="4ea4c-101">Delete photo</span></span>

<span data-ttu-id="4ea4c-102">Exclua uma foto.</span><span class="sxs-lookup"><span data-stu-id="4ea4c-102">Delete a photo.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ea4c-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ea4c-103">Prerequisites</span></span>
<span data-ttu-id="4ea4c-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="4ea4c-104">One of the following **scopes** is required to execute this API:</span></span>

  * <span data-ttu-id="4ea4c-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ea4c-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="4ea4c-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ea4c-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="4ea4c-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea4c-107">Request headers</span></span>
| <span data-ttu-id="4ea4c-108">Nome</span><span class="sxs-lookup"><span data-stu-id="4ea4c-108">Name</span></span>       | <span data-ttu-id="4ea4c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ea4c-109">Type</span></span> | <span data-ttu-id="4ea4c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ea4c-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4ea4c-111">if-match</span><span class="sxs-lookup"><span data-stu-id="4ea4c-111">if-match</span></span>  | <span data-ttu-id="4ea4c-112">string</span><span class="sxs-lookup"><span data-stu-id="4ea4c-112">string</span></span>  | <span data-ttu-id="4ea4c-113">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="4ea4c-113">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="4ea4c-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ea4c-114">Authorization</span></span>  | <span data-ttu-id="4ea4c-115">string</span><span class="sxs-lookup"><span data-stu-id="4ea4c-115">string</span></span>  | <span data-ttu-id="4ea4c-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ea4c-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4ea4c-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea4c-118">Request body</span></span>
<span data-ttu-id="4ea4c-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ea4c-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ea4c-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ea4c-120">Response</span></span>

<span data-ttu-id="4ea4c-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ea4c-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ea4c-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ea4c-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ea4c-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea4c-124">Request</span></span>
<span data-ttu-id="4ea4c-125">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ea4c-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="4ea4c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ea4c-126">Response</span></span>
<span data-ttu-id="4ea4c-127">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ea4c-127">Here is an example of the response.</span></span>
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
