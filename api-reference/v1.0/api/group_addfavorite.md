# <a name="group-addfavorite"></a><span data-ttu-id="1c6cd-101">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="1c6cd-101">group: addFavorite</span></span>
<span data-ttu-id="1c6cd-p101">Adiciona o grupo à lista de grupos de favoritos do usuário atual. Suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="1c6cd-p101">Add the group to the list of the current user's favorite groups. Supported for only Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c6cd-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c6cd-104">Prerequisites</span></span>
<span data-ttu-id="1c6cd-105">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="1c6cd-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="1c6cd-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c6cd-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```
## <a name="request-headers"></a><span data-ttu-id="1c6cd-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c6cd-107">Request headers</span></span>
| <span data-ttu-id="1c6cd-108">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c6cd-108">Header</span></span>       | <span data-ttu-id="1c6cd-109">Valor</span><span class="sxs-lookup"><span data-stu-id="1c6cd-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1c6cd-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c6cd-110">Authorization</span></span>  | <span data-ttu-id="1c6cd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c6cd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c6cd-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c6cd-113">Request body</span></span>
<span data-ttu-id="1c6cd-114">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c6cd-114">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c6cd-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c6cd-115">Response</span></span>

<span data-ttu-id="1c6cd-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c6cd-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c6cd-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c6cd-118">Example</span></span>
<span data-ttu-id="1c6cd-119">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1c6cd-119">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1c6cd-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c6cd-120">Request</span></span>
<span data-ttu-id="1c6cd-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c6cd-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/addFavorite
```

##### <a name="response"></a><span data-ttu-id="1c6cd-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c6cd-122">Response</span></span>
<span data-ttu-id="1c6cd-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c6cd-123">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->