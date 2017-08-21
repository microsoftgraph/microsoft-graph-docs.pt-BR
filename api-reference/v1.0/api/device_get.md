# <a name="get-device"></a><span data-ttu-id="908e1-101">Obter dispositivo</span><span class="sxs-lookup"><span data-stu-id="908e1-101">Get device</span></span>

<span data-ttu-id="908e1-102">Obtém as propriedades e os relacionamentos de um objeto device.</span><span class="sxs-lookup"><span data-stu-id="908e1-102">Get the properties and relationships of a device object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="908e1-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="908e1-103">Prerequisites</span></span>
<span data-ttu-id="908e1-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Device.ReadWrite.All* ou *Directory.Read.All* ou *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="908e1-104">One of the following **scopes** is required to execute this API: *Device.ReadWrite.All* or *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="908e1-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="908e1-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="908e1-106">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="908e1-106">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="908e1-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="908e1-107">Optional query parameters</span></span>
<span data-ttu-id="908e1-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="908e1-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="908e1-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="908e1-109">Request headers</span></span>
| <span data-ttu-id="908e1-110">Nome</span><span class="sxs-lookup"><span data-stu-id="908e1-110">Name</span></span>       | <span data-ttu-id="908e1-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="908e1-111">Type</span></span> | <span data-ttu-id="908e1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="908e1-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="908e1-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="908e1-113">Authorization</span></span>  | <span data-ttu-id="908e1-114">string</span><span class="sxs-lookup"><span data-stu-id="908e1-114">string</span></span>  | <span data-ttu-id="908e1-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="908e1-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="908e1-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="908e1-117">Request body</span></span>
<span data-ttu-id="908e1-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="908e1-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="908e1-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="908e1-119">Response</span></span>

<span data-ttu-id="908e1-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="908e1-120">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="908e1-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="908e1-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="908e1-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="908e1-122">Request</span></span>
<span data-ttu-id="908e1-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="908e1-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="908e1-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="908e1-124">Response</span></span>
<span data-ttu-id="908e1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="908e1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type": 2,
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
