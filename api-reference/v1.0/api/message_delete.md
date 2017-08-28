# <a name="delete-message"></a><span data-ttu-id="fcf18-101">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="fcf18-101">Delete message</span></span>

<span data-ttu-id="fcf18-102">Exclua a mensagem.</span><span class="sxs-lookup"><span data-stu-id="fcf18-102">Delete message.</span></span>
## <a name="permissions"></a><span data-ttu-id="fcf18-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="fcf18-103">Permissions</span></span>
<span data-ttu-id="fcf18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fcf18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fcf18-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcf18-106">Permission type</span></span>      | <span data-ttu-id="fcf18-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fcf18-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="fcf18-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcf18-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fcf18-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcf18-109">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="fcf18-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcf18-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcf18-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcf18-111">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="fcf18-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcf18-112">Application</span></span> | <span data-ttu-id="fcf18-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcf18-113">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fcf18-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcf18-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fcf18-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf18-115">Request headers</span></span>
| <span data-ttu-id="fcf18-116">Nome</span><span class="sxs-lookup"><span data-stu-id="fcf18-116">Name</span></span>       | <span data-ttu-id="fcf18-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcf18-117">Type</span></span> | <span data-ttu-id="fcf18-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcf18-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fcf18-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcf18-119">Authorization</span></span>  | <span data-ttu-id="fcf18-120">string</span><span class="sxs-lookup"><span data-stu-id="fcf18-120">string</span></span>  | <span data-ttu-id="fcf18-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcf18-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcf18-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf18-123">Request body</span></span>
<span data-ttu-id="fcf18-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fcf18-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcf18-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcf18-125">Response</span></span>

<span data-ttu-id="fcf18-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fcf18-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcf18-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fcf18-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fcf18-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf18-129">Request</span></span>
<span data-ttu-id="fcf18-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcf18-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="fcf18-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcf18-131">Response</span></span>
<span data-ttu-id="fcf18-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fcf18-132">Here is an example of the response.</span></span> 
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
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->