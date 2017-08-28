# <a name="list-members"></a><span data-ttu-id="6b23b-101">Listar membros</span><span class="sxs-lookup"><span data-stu-id="6b23b-101">List members</span></span>

<span data-ttu-id="6b23b-p101">Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos e outros grupos como membros. Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="6b23b-p101">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b23b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b23b-105">Permissions</span></span>
<span data-ttu-id="6b23b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b23b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6b23b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b23b-108">Permission type</span></span>      | <span data-ttu-id="6b23b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b23b-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="6b23b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b23b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6b23b-111">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6b23b-111">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   | 
|<span data-ttu-id="6b23b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b23b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b23b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b23b-113">Not supported.</span></span>    | 
|<span data-ttu-id="6b23b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b23b-114">Application</span></span> | <span data-ttu-id="6b23b-115">User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b23b-115">User.Read.All, Directory.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6b23b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b23b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6b23b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6b23b-117">Optional query parameters</span></span>
<span data-ttu-id="6b23b-118">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6b23b-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6b23b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b23b-119">Request headers</span></span>
| <span data-ttu-id="6b23b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6b23b-120">Name</span></span>       | <span data-ttu-id="6b23b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b23b-121">Type</span></span> | <span data-ttu-id="6b23b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b23b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6b23b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b23b-123">Authorization</span></span>  | <span data-ttu-id="6b23b-124">string</span><span class="sxs-lookup"><span data-stu-id="6b23b-124">string</span></span>  | <span data-ttu-id="6b23b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b23b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b23b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b23b-127">Request body</span></span>
<span data-ttu-id="6b23b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b23b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b23b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b23b-129">Response</span></span>

<span data-ttu-id="6b23b-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b23b-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b23b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b23b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b23b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b23b-132">Request</span></span>
<span data-ttu-id="6b23b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b23b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
##### <a name="response"></a><span data-ttu-id="6b23b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b23b-134">Response</span></span>
<span data-ttu-id="6b23b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b23b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->