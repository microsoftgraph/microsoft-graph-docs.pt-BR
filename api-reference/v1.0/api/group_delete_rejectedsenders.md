# <a name="remove-rejectedsender"></a><span data-ttu-id="916de-101">Remover rejectedSender</span><span class="sxs-lookup"><span data-stu-id="916de-101">Remove rejectedSender</span></span>

<span data-ttu-id="916de-102">Remove um usuário ou grupo da lista rejectedSenders.</span><span class="sxs-lookup"><span data-stu-id="916de-102">Remove a user or group from the rejectedSenders list.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="916de-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="916de-103">Prerequisites</span></span>
<span data-ttu-id="916de-104">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="916de-104">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="916de-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="916de-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=<id>

```
## <a name="request-headers"></a><span data-ttu-id="916de-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="916de-106">Request headers</span></span>
| <span data-ttu-id="916de-107">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="916de-107">Header</span></span>       | <span data-ttu-id="916de-108">Valor</span><span class="sxs-lookup"><span data-stu-id="916de-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="916de-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="916de-109">Authorization</span></span>  | <span data-ttu-id="916de-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="916de-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="916de-112">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="916de-112">Request body</span></span>
<span data-ttu-id="916de-113">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="916de-113">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="916de-114">Resposta</span><span class="sxs-lookup"><span data-stu-id="916de-114">Response</span></span>

<span data-ttu-id="916de-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="916de-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="916de-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="916de-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="916de-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="916de-118">Request</span></span>
<span data-ttu-id="916de-119">Eis alguns exemplos da solicitação.</span><span class="sxs-lookup"><span data-stu-id="916de-119">Here are a couple of examples of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id="users/{id}"

DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id="groups/{id}"
```

##### <a name="response"></a><span data-ttu-id="916de-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="916de-120">Response</span></span>
<span data-ttu-id="916de-121">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="916de-121">Here is an example of the response.</span></span> 
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
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->