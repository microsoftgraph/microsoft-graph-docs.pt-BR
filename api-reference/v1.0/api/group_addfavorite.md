# <a name="group-addfavorite"></a><span data-ttu-id="3046f-101">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="3046f-101">group: addFavorite</span></span>
<span data-ttu-id="3046f-p101">Adicionar o grupo à lista de grupos de favoritos do usuário atual. Com suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="3046f-p101">Add the group to the list of the current user's favorite groups. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="3046f-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="3046f-104">Permissions</span></span>
<span data-ttu-id="3046f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3046f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3046f-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3046f-107">Permission type</span></span>      | <span data-ttu-id="3046f-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3046f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3046f-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3046f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="3046f-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3046f-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3046f-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3046f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3046f-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3046f-112">Not supported.</span></span>    |
|<span data-ttu-id="3046f-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3046f-113">Application</span></span> | <span data-ttu-id="3046f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3046f-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3046f-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3046f-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="3046f-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3046f-116">Request headers</span></span>
| <span data-ttu-id="3046f-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3046f-117">Header</span></span>       | <span data-ttu-id="3046f-118">Valor</span><span class="sxs-lookup"><span data-stu-id="3046f-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3046f-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="3046f-119">Authorization</span></span>  | <span data-ttu-id="3046f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3046f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3046f-122">Preferir</span><span class="sxs-lookup"><span data-stu-id="3046f-122">Prefer</span></span> | <span data-ttu-id="3046f-123">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="3046f-123">return=minimal.</span></span> <span data-ttu-id="3046f-124">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3046f-124">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="3046f-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3046f-125">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3046f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3046f-126">Request body</span></span>
<span data-ttu-id="3046f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3046f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3046f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3046f-128">Response</span></span>
<span data-ttu-id="3046f-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3046f-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3046f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3046f-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3046f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3046f-132">Request</span></span>
<span data-ttu-id="3046f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3046f-133">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/addFavorite
```

#### <a name="response"></a><span data-ttu-id="3046f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3046f-134">Response</span></span>
<span data-ttu-id="3046f-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3046f-135">Here is an example of the response.</span></span>
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
