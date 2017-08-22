# <a name="list-createdobjects"></a><span data-ttu-id="8dbfb-101">Listar createdObjects</span><span class="sxs-lookup"><span data-stu-id="8dbfb-101">List createdObjects</span></span>

<span data-ttu-id="8dbfb-102">Obtenha uma lista de objetos de diretório criados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="8dbfb-102">Get a list of directory objects that were created by the user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8dbfb-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8dbfb-103">Prerequisites</span></span>
<span data-ttu-id="8dbfb-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *User.Read; User.ReadWrite; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="8dbfb-104">One of the following **scopes** is required to execute this API: *User.Read; User.ReadWrite; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="8dbfb-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8dbfb-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8dbfb-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8dbfb-106">Optional query parameters</span></span>
<span data-ttu-id="8dbfb-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8dbfb-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8dbfb-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8dbfb-108">Request headers</span></span>
| <span data-ttu-id="8dbfb-109">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8dbfb-109">Header</span></span>       | <span data-ttu-id="8dbfb-110">Valor</span><span class="sxs-lookup"><span data-stu-id="8dbfb-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8dbfb-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="8dbfb-111">Authorization</span></span>  | <span data-ttu-id="8dbfb-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8dbfb-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8dbfb-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8dbfb-114">Content-Type</span></span>  | <span data-ttu-id="8dbfb-115">application/json</span><span class="sxs-lookup"><span data-stu-id="8dbfb-115">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8dbfb-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8dbfb-116">Request body</span></span>
<span data-ttu-id="8dbfb-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8dbfb-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dbfb-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dbfb-118">Response</span></span>

<span data-ttu-id="8dbfb-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8dbfb-119">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8dbfb-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8dbfb-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8dbfb-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8dbfb-121">Request</span></span>
<span data-ttu-id="8dbfb-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8dbfb-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/createdObjects
```
##### <a name="response"></a><span data-ttu-id="8dbfb-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dbfb-123">Response</span></span>
<span data-ttu-id="8dbfb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8dbfb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->