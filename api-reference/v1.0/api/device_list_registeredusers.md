# <a name="list-registeredusers"></a><span data-ttu-id="b773a-101">Listar registeredUsers</span><span class="sxs-lookup"><span data-stu-id="b773a-101">List registeredUsers</span></span>

<span data-ttu-id="b773a-102">Recupera uma lista de usuários que são usuários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b773a-102">Retrieve a list of users that are registered users of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="b773a-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b773a-103">Permissions</span></span>
<span data-ttu-id="b773a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b773a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="b773a-106">Device.ReadWrite.All e User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="b773a-106">Device.ReadWrite.All and User.ReadBasic.All</span></span>
- <span data-ttu-id="b773a-107">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b773a-107">Directory.Read.All</span></span>
- <span data-ttu-id="b773a-108">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b773a-108">Directory.ReadWrite.All</span></span> 
- <span data-ttu-id="b773a-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b773a-109">Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="b773a-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b773a-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b773a-111">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b773a-111">Optional query parameters</span></span>
<span data-ttu-id="b773a-112">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b773a-112">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b773a-113">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b773a-113">Request headers</span></span>
| <span data-ttu-id="b773a-114">Nome</span><span class="sxs-lookup"><span data-stu-id="b773a-114">Name</span></span>       | <span data-ttu-id="b773a-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="b773a-115">Type</span></span> | <span data-ttu-id="b773a-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="b773a-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b773a-117">Autorização</span><span class="sxs-lookup"><span data-stu-id="b773a-117">Authorization</span></span>  | <span data-ttu-id="b773a-118">string</span><span class="sxs-lookup"><span data-stu-id="b773a-118">string</span></span>  | <span data-ttu-id="b773a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b773a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b773a-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b773a-121">Request body</span></span>
<span data-ttu-id="b773a-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b773a-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b773a-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="b773a-123">Response</span></span>

<span data-ttu-id="b773a-124">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b773a-124">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b773a-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b773a-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b773a-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b773a-126">Request</span></span>
<span data-ttu-id="b773a-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b773a-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="b773a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b773a-128">Response</span></span>
<span data-ttu-id="b773a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b773a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->