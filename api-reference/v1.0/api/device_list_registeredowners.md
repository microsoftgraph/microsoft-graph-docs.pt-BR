# <a name="list-registeredowners"></a><span data-ttu-id="a1299-101">Listar registeredOwners</span><span class="sxs-lookup"><span data-stu-id="a1299-101">List registeredOwners</span></span>

<span data-ttu-id="a1299-102">Recupera uma lista de usuários que são proprietários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1299-102">Retrieve a list of users that are registered owners of the device.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1299-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1299-103">Prerequisites</span></span>
<span data-ttu-id="a1299-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="a1299-104">One of the following **scopes** is required to execute this API:</span></span> 
- <span data-ttu-id="a1299-105">*Device.ReadWrite.All* e *User.ReadBasic.All*</span><span class="sxs-lookup"><span data-stu-id="a1299-105">*Device.ReadWrite.All* and *User.ReadBasic.All*</span></span>
- <span data-ttu-id="a1299-106">*Directory.Read.All*</span><span class="sxs-lookup"><span data-stu-id="a1299-106">*Directory.Read.All*</span></span>
- <span data-ttu-id="a1299-107">*Directory.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="a1299-107">*Directory.ReadWrite.All*</span></span> 
- <span data-ttu-id="a1299-108">*Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="a1299-108">*Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="a1299-109">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1299-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a1299-110">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a1299-110">Optional query parameters</span></span>
<span data-ttu-id="a1299-111">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a1299-111">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a1299-112">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1299-112">Request headers</span></span>
| <span data-ttu-id="a1299-113">Nome</span><span class="sxs-lookup"><span data-stu-id="a1299-113">Name</span></span>       | <span data-ttu-id="a1299-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1299-114">Type</span></span> | <span data-ttu-id="a1299-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1299-115">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a1299-116">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1299-116">Authorization</span></span>  | <span data-ttu-id="a1299-117">string</span><span class="sxs-lookup"><span data-stu-id="a1299-117">string</span></span>  | <span data-ttu-id="a1299-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1299-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1299-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1299-120">Request body</span></span>
<span data-ttu-id="a1299-121">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1299-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1299-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1299-122">Response</span></span>

<span data-ttu-id="a1299-123">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1299-123">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a1299-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1299-124">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1299-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1299-125">Request</span></span>
<span data-ttu-id="a1299-126">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1299-126">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="a1299-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1299-127">Response</span></span>
<span data-ttu-id="a1299-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1299-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->