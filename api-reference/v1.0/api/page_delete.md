# <a name="delete-page"></a><span data-ttu-id="dd532-101">Excluir página</span><span class="sxs-lookup"><span data-stu-id="dd532-101">Delete page</span></span>

<span data-ttu-id="dd532-102">Exclua uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="dd532-102">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd532-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd532-103">Permissions</span></span>
<span data-ttu-id="dd532-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dd532-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dd532-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd532-106">Permission type</span></span>      | <span data-ttu-id="dd532-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd532-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="dd532-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd532-108">Delegated (work or school account)</span></span> | <span data-ttu-id="dd532-109">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd532-109">Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="dd532-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd532-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd532-111">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd532-111">Notes.ReadWrite</span></span>    | 
|<span data-ttu-id="dd532-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd532-112">Application</span></span> | <span data-ttu-id="dd532-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd532-113">Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="dd532-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd532-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="dd532-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd532-115">Request headers</span></span>
| <span data-ttu-id="dd532-116">Nome</span><span class="sxs-lookup"><span data-stu-id="dd532-116">Name</span></span>       | <span data-ttu-id="dd532-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd532-117">Type</span></span> | <span data-ttu-id="dd532-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd532-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dd532-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd532-119">Authorization</span></span>  | <span data-ttu-id="dd532-120">string</span><span class="sxs-lookup"><span data-stu-id="dd532-120">string</span></span>  | <span data-ttu-id="dd532-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd532-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="dd532-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd532-123">Response</span></span>

<span data-ttu-id="dd532-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd532-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd532-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd532-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd532-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd532-127">Request</span></span>
<span data-ttu-id="dd532-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd532-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="dd532-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd532-129">Response</span></span>
<span data-ttu-id="dd532-130">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd532-130">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->