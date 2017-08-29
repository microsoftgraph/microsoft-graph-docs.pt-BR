# <a name="group-removefavorite"></a><span data-ttu-id="629e6-101">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="629e6-101">group: removeFavorite</span></span>
<span data-ttu-id="629e6-p101">Remova o grupo da lista de grupos favoritos do usuário atual. Com suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="629e6-p101">Remove the group from the list of the current user's favorite groups. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="629e6-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="629e6-104">Permissions</span></span>
<span data-ttu-id="629e6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="629e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="629e6-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="629e6-107">Permission type</span></span>      | <span data-ttu-id="629e6-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="629e6-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="629e6-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="629e6-109">Delegated (work or school account)</span></span> | <span data-ttu-id="629e6-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e6-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="629e6-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="629e6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="629e6-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629e6-112">Not supported.</span></span>    |
|<span data-ttu-id="629e6-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="629e6-113">Application</span></span> | <span data-ttu-id="629e6-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e6-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="629e6-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="629e6-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```
## <a name="request-headers"></a><span data-ttu-id="629e6-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="629e6-116">Request headers</span></span>
| <span data-ttu-id="629e6-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="629e6-117">Header</span></span>       | <span data-ttu-id="629e6-118">Valor</span><span class="sxs-lookup"><span data-stu-id="629e6-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="629e6-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="629e6-119">Authorization</span></span>  | <span data-ttu-id="629e6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="629e6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="629e6-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="629e6-122">Request body</span></span>
<span data-ttu-id="629e6-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="629e6-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="629e6-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="629e6-124">Response</span></span>

<span data-ttu-id="629e6-p104">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="629e6-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="629e6-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="629e6-127">Example</span></span>
<span data-ttu-id="629e6-128">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="629e6-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="629e6-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="629e6-129">Request</span></span>
<span data-ttu-id="629e6-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="629e6-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/removeFavorite
```

##### <a name="response"></a><span data-ttu-id="629e6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="629e6-131">Response</span></span>
<span data-ttu-id="629e6-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="629e6-132">Here is an example of the response.</span></span>
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
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->