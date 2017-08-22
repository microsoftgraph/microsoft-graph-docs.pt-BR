# <a name="list-memberof"></a><span data-ttu-id="e73c0-101">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="e73c0-101">List memberOf</span></span>

<span data-ttu-id="e73c0-102">Obtenha [grupos](../resources/group.md) e [funções de diretório](../resources/directoryrole.md) dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="e73c0-102">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="e73c0-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e73c0-103">Prerequisites</span></span>
<span data-ttu-id="e73c0-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="e73c0-104">One of the following **scopes** is required to execute this API: *Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="e73c0-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e73c0-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e73c0-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e73c0-106">Optional query parameters</span></span>
<span data-ttu-id="e73c0-p101">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta. $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="e73c0-p101">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response. $filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="e73c0-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e73c0-109">Request headers</span></span>
| <span data-ttu-id="e73c0-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e73c0-110">Header</span></span>       | <span data-ttu-id="e73c0-111">Valor</span><span class="sxs-lookup"><span data-stu-id="e73c0-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e73c0-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="e73c0-112">Authorization</span></span>  | <span data-ttu-id="e73c0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e73c0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e73c0-115">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e73c0-115">Accept</span></span>  | <span data-ttu-id="e73c0-116">application/json</span><span class="sxs-lookup"><span data-stu-id="e73c0-116">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e73c0-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e73c0-117">Request body</span></span>
<span data-ttu-id="e73c0-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e73c0-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e73c0-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="e73c0-119">Response</span></span>

<span data-ttu-id="e73c0-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e73c0-120">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e73c0-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e73c0-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e73c0-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e73c0-122">Request</span></span>
<span data-ttu-id="e73c0-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e73c0-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/memberOf
```
##### <a name="response"></a><span data-ttu-id="e73c0-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="e73c0-124">Response</span></span>
<span data-ttu-id="e73c0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e73c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
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
