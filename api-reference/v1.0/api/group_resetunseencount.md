# <a name="group-resetunseencount"></a><span data-ttu-id="87ade-101">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="87ade-101">group: resetUnseenCount</span></span>

<span data-ttu-id="87ade-p101">Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita. Suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="87ade-p101">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for only Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87ade-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87ade-104">Prerequisites</span></span>
<span data-ttu-id="87ade-105">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="87ade-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span> 
## <a name="http-request"></a><span data-ttu-id="87ade-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87ade-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="87ade-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87ade-107">Request headers</span></span>
| <span data-ttu-id="87ade-108">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87ade-108">Header</span></span>       | <span data-ttu-id="87ade-109">Valor</span><span class="sxs-lookup"><span data-stu-id="87ade-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="87ade-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="87ade-110">Authorization</span></span>  | <span data-ttu-id="87ade-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87ade-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87ade-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87ade-113">Request body</span></span>
<span data-ttu-id="87ade-114">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87ade-114">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87ade-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="87ade-115">Response</span></span>

<span data-ttu-id="87ade-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87ade-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87ade-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87ade-118">Example</span></span>
<span data-ttu-id="87ade-119">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="87ade-119">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="87ade-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87ade-120">Request</span></span>
<span data-ttu-id="87ade-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87ade-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```

##### <a name="response"></a><span data-ttu-id="87ade-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="87ade-122">Response</span></span>
<span data-ttu-id="87ade-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87ade-123">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
