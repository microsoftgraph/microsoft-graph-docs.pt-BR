# <a name="list-owners"></a><span data-ttu-id="ddf69-101">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="ddf69-101">List owners</span></span>
<span data-ttu-id="ddf69-p101">Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="ddf69-p101">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ddf69-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddf69-104">Permissions</span></span>
<span data-ttu-id="ddf69-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ddf69-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ddf69-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddf69-107">Permission type</span></span>      | <span data-ttu-id="ddf69-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddf69-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddf69-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddf69-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ddf69-110">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddf69-110">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="ddf69-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddf69-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddf69-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddf69-112">Not supported.</span></span>    |
|<span data-ttu-id="ddf69-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddf69-113">Application</span></span> | <span data-ttu-id="ddf69-114">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddf69-114">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddf69-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddf69-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddf69-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ddf69-116">Optional query parameters</span></span>
<span data-ttu-id="ddf69-117">Este método dá suporte a [Parâmetros de consulta OData](../../../concepts/query_parameters.md) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf69-117">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddf69-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf69-118">Request headers</span></span>
| <span data-ttu-id="ddf69-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ddf69-119">Name</span></span>       | <span data-ttu-id="ddf69-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddf69-120">Type</span></span> | <span data-ttu-id="ddf69-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddf69-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ddf69-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddf69-122">Authorization</span></span>  | <span data-ttu-id="ddf69-123">string</span><span class="sxs-lookup"><span data-stu-id="ddf69-123">string</span></span>  | <span data-ttu-id="ddf69-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddf69-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddf69-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf69-126">Request body</span></span>
<span data-ttu-id="ddf69-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ddf69-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddf69-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf69-128">Response</span></span>
<span data-ttu-id="ddf69-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf69-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddf69-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddf69-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ddf69-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf69-131">Request</span></span>
<span data-ttu-id="ddf69-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddf69-132">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="ddf69-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf69-133">Response</span></span>
<span data-ttu-id="ddf69-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf69-134">Here is an example of the response.</span></span>
><span data-ttu-id="ddf69-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ddf69-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ddf69-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddf69-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
