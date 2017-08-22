# <a name="delete-eventmessage"></a><span data-ttu-id="3552a-101">Excluir eventMessage</span><span class="sxs-lookup"><span data-stu-id="3552a-101">Delete eventMessage</span></span>

<span data-ttu-id="3552a-102">Exclui a eventMessage.</span><span class="sxs-lookup"><span data-stu-id="3552a-102">Delete eventMessage.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3552a-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3552a-103">Prerequisites</span></span>
<span data-ttu-id="3552a-104">Os seguintes **escopos** são necessários para executar esta API: _Mail.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="3552a-104">The following **scopes** are required to execute this API: _Mail.ReadWrite_</span></span> 
## <a name="http-request"></a><span data-ttu-id="3552a-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3552a-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3552a-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3552a-106">Request headers</span></span>
| <span data-ttu-id="3552a-107">Nome</span><span class="sxs-lookup"><span data-stu-id="3552a-107">Name</span></span>       | <span data-ttu-id="3552a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3552a-108">Type</span></span> | <span data-ttu-id="3552a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3552a-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3552a-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="3552a-110">Authorization</span></span>  | <span data-ttu-id="3552a-111">string</span><span class="sxs-lookup"><span data-stu-id="3552a-111">string</span></span>  | <span data-ttu-id="3552a-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3552a-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3552a-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3552a-114">Request body</span></span>
<span data-ttu-id="3552a-115">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3552a-115">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3552a-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="3552a-116">Response</span></span>

<span data-ttu-id="3552a-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3552a-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3552a-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3552a-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3552a-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3552a-120">Request</span></span>
<span data-ttu-id="3552a-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3552a-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="3552a-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="3552a-122">Response</span></span>
<span data-ttu-id="3552a-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3552a-123">Here is an example of the response.</span></span> 
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
  "description": "Delete eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->