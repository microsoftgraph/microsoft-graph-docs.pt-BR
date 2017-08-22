# <a name="list-owners"></a><span data-ttu-id="0476b-101">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="0476b-101">List owners</span></span>

<span data-ttu-id="0476b-p101">Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="0476b-p101">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="0476b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0476b-104">Prerequisites</span></span>
<span data-ttu-id="0476b-105">Os seguintes **escopos** são necessários para executar esta API: *Group.Read.All* e *User.ReadBasic.All* ou *User.Read.All* ou *User.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="0476b-105">The following **scopes** are required to execute this API: *Group.Read.All* and one of *User.ReadBasic.All* or *User.Read.All* or *User.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="0476b-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0476b-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0476b-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0476b-107">Optional query parameters</span></span>
<span data-ttu-id="0476b-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0476b-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0476b-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0476b-109">Request headers</span></span>
| <span data-ttu-id="0476b-110">Nome</span><span class="sxs-lookup"><span data-stu-id="0476b-110">Name</span></span>       | <span data-ttu-id="0476b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0476b-111">Type</span></span> | <span data-ttu-id="0476b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0476b-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0476b-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="0476b-113">Authorization</span></span>  | <span data-ttu-id="0476b-114">string</span><span class="sxs-lookup"><span data-stu-id="0476b-114">string</span></span>  | <span data-ttu-id="0476b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0476b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0476b-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0476b-117">Request body</span></span>
<span data-ttu-id="0476b-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0476b-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0476b-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="0476b-119">Response</span></span>

<span data-ttu-id="0476b-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0476b-120">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0476b-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0476b-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0476b-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0476b-122">Request</span></span>
<span data-ttu-id="0476b-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0476b-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
##### <a name="response"></a><span data-ttu-id="0476b-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="0476b-124">Response</span></span>
<span data-ttu-id="0476b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0476b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
