# <a name="list-devices"></a><span data-ttu-id="8a9b8-101">Listar dispositivos</span><span class="sxs-lookup"><span data-stu-id="8a9b8-101">List devices</span></span>

<span data-ttu-id="8a9b8-102">Recupera uma lista de objetos de dispositivos registrados na organização.</span><span class="sxs-lookup"><span data-stu-id="8a9b8-102">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a9b8-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a9b8-103">Prerequisites</span></span>
<span data-ttu-id="8a9b8-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Device.ReadWrite.All* ou *Directory.Read.All* ou *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="8a9b8-104">One of the following **scopes** is required to execute this API: *Device.ReadWrite.All* or *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="8a9b8-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a9b8-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8a9b8-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8a9b8-106">Optional query parameters</span></span>
<span data-ttu-id="8a9b8-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8a9b8-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8a9b8-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a9b8-108">Request headers</span></span>
| <span data-ttu-id="8a9b8-109">Nome</span><span class="sxs-lookup"><span data-stu-id="8a9b8-109">Name</span></span>       | <span data-ttu-id="8a9b8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a9b8-110">Type</span></span> | <span data-ttu-id="8a9b8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a9b8-111">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8a9b8-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a9b8-112">Authorization</span></span>  | <span data-ttu-id="8a9b8-113">string</span><span class="sxs-lookup"><span data-stu-id="8a9b8-113">string</span></span>  | <span data-ttu-id="8a9b8-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a9b8-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a9b8-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a9b8-116">Request body</span></span>
<span data-ttu-id="8a9b8-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a9b8-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a9b8-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a9b8-118">Response</span></span>

<span data-ttu-id="8a9b8-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a9b8-119">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8a9b8-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a9b8-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a9b8-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a9b8-121">Request</span></span>
<span data-ttu-id="8a9b8-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a9b8-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices
```

##### <a name="response"></a><span data-ttu-id="8a9b8-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a9b8-123">Response</span></span>
<span data-ttu-id="8a9b8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a9b8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":false,
      "alternativeSecurityIds":
      [
        {
          "type":2,
          "key":"Y3YxN2E1MWFlYw==",
          "identityProvider": null
        }
      ],
      "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
      "displayName":"Test device",
      "id": "id-value",
      "operatingSystem":"linux",
      "operatingSystemVersion":"1"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
