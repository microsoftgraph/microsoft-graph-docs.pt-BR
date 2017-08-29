# <a name="list-memberof"></a><span data-ttu-id="2e3ef-101">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="2e3ef-101">List memberOf</span></span>

<span data-ttu-id="2e3ef-102">Obtenha grupos dos quais um grupo é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="2e3ef-102">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="2e3ef-p101">Essa operação não é transitiva. Ao contrário de obter Grupos do Office 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="2e3ef-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2e3ef-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e3ef-105">Permissions</span></span>
<span data-ttu-id="2e3ef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e3ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2e3ef-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e3ef-108">Permission type</span></span>      | <span data-ttu-id="2e3ef-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e3ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e3ef-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e3ef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e3ef-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e3ef-111">Group.Read.All</span></span>    |
|<span data-ttu-id="2e3ef-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e3ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e3ef-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e3ef-113">Not supported.</span></span>    |
|<span data-ttu-id="2e3ef-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e3ef-114">Application</span></span> | <span data-ttu-id="2e3ef-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e3ef-115">Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e3ef-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e3ef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2e3ef-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2e3ef-117">Optional query parameters</span></span>
<span data-ttu-id="2e3ef-118">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2e3ef-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2e3ef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e3ef-119">Request headers</span></span>
| <span data-ttu-id="2e3ef-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2e3ef-120">Name</span></span>       | <span data-ttu-id="2e3ef-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e3ef-121">Type</span></span> | <span data-ttu-id="2e3ef-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e3ef-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2e3ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e3ef-123">Authorization</span></span>  | <span data-ttu-id="2e3ef-124">string</span><span class="sxs-lookup"><span data-stu-id="2e3ef-124">string</span></span>  | <span data-ttu-id="2e3ef-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e3ef-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e3ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e3ef-127">Request body</span></span>
<span data-ttu-id="2e3ef-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e3ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e3ef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e3ef-129">Response</span></span>

<span data-ttu-id="2e3ef-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e3ef-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e3ef-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e3ef-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e3ef-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e3ef-132">Request</span></span>
<span data-ttu-id="2e3ef-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e3ef-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="2e3ef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e3ef-134">Response</span></span>
<span data-ttu-id="2e3ef-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e3ef-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->