# <a name="delete-a-user"></a><span data-ttu-id="68a21-101">Excluir um usuário</span><span class="sxs-lookup"><span data-stu-id="68a21-101">Delete a user</span></span>

<span data-ttu-id="68a21-102">Exclua um usuário.</span><span class="sxs-lookup"><span data-stu-id="68a21-102">Delete user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68a21-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="68a21-103">Prerequisites</span></span>
<span data-ttu-id="68a21-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="68a21-104">One of the following **scopes** is required to execute this API: *Directory.AccessAsUser.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="68a21-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68a21-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="68a21-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68a21-106">Request headers</span></span>
| <span data-ttu-id="68a21-107">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68a21-107">Header</span></span>       | <span data-ttu-id="68a21-108">Valor</span><span class="sxs-lookup"><span data-stu-id="68a21-108">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="68a21-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="68a21-109">Authorization</span></span>  | <span data-ttu-id="68a21-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68a21-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="68a21-112">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68a21-112">Request body</span></span>
<span data-ttu-id="68a21-113">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="68a21-113">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68a21-114">Resposta</span><span class="sxs-lookup"><span data-stu-id="68a21-114">Response</span></span>

<span data-ttu-id="68a21-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68a21-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68a21-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68a21-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68a21-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68a21-118">Request</span></span>
<span data-ttu-id="68a21-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68a21-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/mba9a3254-9f18-4209-aeb3-9e42a35b5be4
```
##### <a name="response"></a><span data-ttu-id="68a21-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="68a21-120">Response</span></span>
<span data-ttu-id="68a21-121">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68a21-121">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->