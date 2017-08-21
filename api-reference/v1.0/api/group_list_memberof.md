# <a name="list-memberof"></a><span data-ttu-id="92cca-101">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="92cca-101">List memberOf</span></span>

<span data-ttu-id="92cca-102">Obtenha grupos dos quais um grupo é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="92cca-102">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="92cca-p101">Essa operação não é transitiva. Ao contrário de obter Grupos do Office 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="92cca-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="92cca-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92cca-105">Prerequisites</span></span>
<span data-ttu-id="92cca-106">Um dos seguintes **escopos** é necessário para executar esta API: *Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="92cca-106">One of the following **scopes** is required to execute this API: *Group.Read.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="92cca-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92cca-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="92cca-108">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="92cca-108">Optional query parameters</span></span>
<span data-ttu-id="92cca-109">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="92cca-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="92cca-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92cca-110">Request headers</span></span>
| <span data-ttu-id="92cca-111">Nome</span><span class="sxs-lookup"><span data-stu-id="92cca-111">Name</span></span>       | <span data-ttu-id="92cca-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="92cca-112">Type</span></span> | <span data-ttu-id="92cca-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="92cca-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="92cca-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="92cca-114">Authorization</span></span>  | <span data-ttu-id="92cca-115">string</span><span class="sxs-lookup"><span data-stu-id="92cca-115">string</span></span>  | <span data-ttu-id="92cca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92cca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92cca-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92cca-118">Request body</span></span>
<span data-ttu-id="92cca-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92cca-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92cca-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="92cca-120">Response</span></span>

<span data-ttu-id="92cca-121">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92cca-121">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="92cca-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92cca-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92cca-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92cca-123">Request</span></span>
<span data-ttu-id="92cca-124">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92cca-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="92cca-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="92cca-125">Response</span></span>
<span data-ttu-id="92cca-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92cca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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