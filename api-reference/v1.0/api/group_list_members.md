# <a name="list-members"></a><span data-ttu-id="622ef-101">Listar membros</span><span class="sxs-lookup"><span data-stu-id="622ef-101">List members</span></span>

<span data-ttu-id="622ef-p101">Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos e outros grupos como membros. Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="622ef-p101">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="622ef-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="622ef-105">Prerequisites</span></span>
<span data-ttu-id="622ef-106">Um dos seguintes **escopos** é necessário para executar esta API: *Directory.Read.All*, *Directory.AccessAsUser.All*, *User.ReadBasic.All* ou *User.Read.All*</span><span class="sxs-lookup"><span data-stu-id="622ef-106">One of the following **scopes** is required to execute this API: *Directory.Read.All*, *Directory.AccessAsUser.All*, *User.ReadBasic.All*, or *User.Read.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="622ef-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="622ef-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="622ef-108">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="622ef-108">Optional query parameters</span></span>
<span data-ttu-id="622ef-109">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="622ef-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="622ef-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="622ef-110">Request headers</span></span>
| <span data-ttu-id="622ef-111">Nome</span><span class="sxs-lookup"><span data-stu-id="622ef-111">Name</span></span>       | <span data-ttu-id="622ef-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="622ef-112">Type</span></span> | <span data-ttu-id="622ef-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="622ef-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="622ef-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="622ef-114">Authorization</span></span>  | <span data-ttu-id="622ef-115">string</span><span class="sxs-lookup"><span data-stu-id="622ef-115">string</span></span>  | <span data-ttu-id="622ef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="622ef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="622ef-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="622ef-118">Request body</span></span>
<span data-ttu-id="622ef-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="622ef-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="622ef-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="622ef-120">Response</span></span>

<span data-ttu-id="622ef-121">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="622ef-121">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="622ef-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="622ef-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="622ef-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="622ef-123">Request</span></span>
<span data-ttu-id="622ef-124">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="622ef-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
##### <a name="response"></a><span data-ttu-id="622ef-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="622ef-125">Response</span></span>
<span data-ttu-id="622ef-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="622ef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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