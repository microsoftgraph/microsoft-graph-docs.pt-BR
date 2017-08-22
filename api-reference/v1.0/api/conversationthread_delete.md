# <a name="delete-conversationthread"></a><span data-ttu-id="0fe02-101">Excluir conversationThread</span><span class="sxs-lookup"><span data-stu-id="0fe02-101">Delete conversationThread</span></span>

<span data-ttu-id="0fe02-102">Exclui um conversationThread.</span><span class="sxs-lookup"><span data-stu-id="0fe02-102">Delete conversationThread.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0fe02-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0fe02-103">Prerequisites</span></span>
<span data-ttu-id="0fe02-104">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="0fe02-104">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
 
## <a name="http-request"></a><span data-ttu-id="0fe02-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fe02-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0fe02-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe02-106">Request headers</span></span>
| <span data-ttu-id="0fe02-107">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fe02-107">Header</span></span>       | <span data-ttu-id="0fe02-108">Valor</span><span class="sxs-lookup"><span data-stu-id="0fe02-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0fe02-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fe02-109">Authorization</span></span>  | <span data-ttu-id="0fe02-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fe02-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0fe02-112">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe02-112">Request body</span></span>
<span data-ttu-id="0fe02-113">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0fe02-113">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fe02-114">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fe02-114">Response</span></span>

<span data-ttu-id="0fe02-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fe02-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fe02-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fe02-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0fe02-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe02-118">Request</span></span>
<span data-ttu-id="0fe02-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fe02-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="0fe02-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fe02-120">Response</span></span>
<span data-ttu-id="0fe02-121">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fe02-121">Here is an example of the response.</span></span> 
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
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->