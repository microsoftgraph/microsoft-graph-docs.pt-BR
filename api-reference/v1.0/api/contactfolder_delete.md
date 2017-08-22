# <a name="delete-contactfolder"></a><span data-ttu-id="86529-101">Excluir contactFolder</span><span class="sxs-lookup"><span data-stu-id="86529-101">Delete contactFolder</span></span>

<span data-ttu-id="86529-102">Exclui uma contactFolder que não a padrão.</span><span class="sxs-lookup"><span data-stu-id="86529-102">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86529-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86529-103">Prerequisites</span></span>
<span data-ttu-id="86529-104">Um dos seguintes **escopos** é necessário para executar esta API: *Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="86529-104">One of the following **scopes** is required to execute this API: *Contacts.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="86529-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86529-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="86529-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86529-106">Request headers</span></span>
| <span data-ttu-id="86529-107">Nome</span><span class="sxs-lookup"><span data-stu-id="86529-107">Name</span></span>       | <span data-ttu-id="86529-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="86529-108">Type</span></span> | <span data-ttu-id="86529-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="86529-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="86529-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="86529-110">Authorization</span></span>  | <span data-ttu-id="86529-111">string</span><span class="sxs-lookup"><span data-stu-id="86529-111">string</span></span>  | <span data-ttu-id="86529-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86529-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86529-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86529-114">Request body</span></span>
<span data-ttu-id="86529-115">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86529-115">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86529-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="86529-116">Response</span></span>

<span data-ttu-id="86529-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86529-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86529-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86529-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86529-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86529-120">Request</span></span>
<span data-ttu-id="86529-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86529-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="86529-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="86529-122">Response</span></span>
<span data-ttu-id="86529-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86529-123">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
