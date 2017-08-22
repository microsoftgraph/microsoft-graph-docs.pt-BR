# <a name="delete-page"></a><span data-ttu-id="acbcc-101">Excluir página</span><span class="sxs-lookup"><span data-stu-id="acbcc-101">Delete page</span></span>

<span data-ttu-id="acbcc-102">Exclua uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="acbcc-102">Delete a OneNote page.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="acbcc-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="acbcc-103">Prerequisites</span></span>
<span data-ttu-id="acbcc-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="acbcc-104">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="acbcc-105">Notes.ReadWrite ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acbcc-105">Notes.ReadWrite, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="acbcc-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="acbcc-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="acbcc-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="acbcc-107">Request headers</span></span>
| <span data-ttu-id="acbcc-108">Nome</span><span class="sxs-lookup"><span data-stu-id="acbcc-108">Name</span></span>       | <span data-ttu-id="acbcc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="acbcc-109">Type</span></span> | <span data-ttu-id="acbcc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="acbcc-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="acbcc-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="acbcc-111">Authorization</span></span>  | <span data-ttu-id="acbcc-112">string</span><span class="sxs-lookup"><span data-stu-id="acbcc-112">string</span></span>  | <span data-ttu-id="acbcc-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="acbcc-p101">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="acbcc-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="acbcc-115">Response</span></span>

<span data-ttu-id="acbcc-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="acbcc-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acbcc-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="acbcc-118">Example</span></span>
##### <a name="request"></a><span data-ttu-id="acbcc-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="acbcc-119">Request</span></span>
<span data-ttu-id="acbcc-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="acbcc-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="acbcc-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="acbcc-121">Response</span></span>
<span data-ttu-id="acbcc-122">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="acbcc-122">Here is an example of the response.</span></span>
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