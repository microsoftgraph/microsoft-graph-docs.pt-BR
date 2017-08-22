# <a name="create-device"></a><span data-ttu-id="5a823-101">Criar dispositivo</span><span class="sxs-lookup"><span data-stu-id="5a823-101">Create device</span></span>

<span data-ttu-id="5a823-102">Cria e registra um novo dispositivo na organização.</span><span class="sxs-lookup"><span data-stu-id="5a823-102">Create and register a new device in the organization.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a823-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5a823-103">Prerequisites</span></span>
<span data-ttu-id="5a823-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Device.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="5a823-104">One of the following **scopes** is required to execute this API: *Device.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="5a823-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a823-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="5a823-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a823-106">Request headers</span></span>
| <span data-ttu-id="5a823-107">Nome</span><span class="sxs-lookup"><span data-stu-id="5a823-107">Name</span></span>       | <span data-ttu-id="5a823-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a823-108">Type</span></span> | <span data-ttu-id="5a823-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a823-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5a823-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a823-110">Authorization</span></span>  | <span data-ttu-id="5a823-111">string</span><span class="sxs-lookup"><span data-stu-id="5a823-111">string</span></span>  | <span data-ttu-id="5a823-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a823-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5a823-114">Content-type</span><span class="sxs-lookup"><span data-stu-id="5a823-114">Content-type</span></span> | <span data-ttu-id="5a823-115">string</span><span class="sxs-lookup"><span data-stu-id="5a823-115">string</span></span> | <span data-ttu-id="5a823-116">application/json</span><span class="sxs-lookup"><span data-stu-id="5a823-116">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a823-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a823-117">Request body</span></span>
<span data-ttu-id="5a823-118">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="5a823-118">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5a823-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a823-119">Response</span></span>

<span data-ttu-id="5a823-120">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a823-120">If successful, this method returns `201, Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a823-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a823-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a823-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a823-122">Request</span></span>
<span data-ttu-id="5a823-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a823-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"Y3YxN2E1MWFlYw=="
    }
  ],
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```
<span data-ttu-id="5a823-124">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="5a823-124">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5a823-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a823-125">Response</span></span>
<span data-ttu-id="5a823-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a823-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"Y3YxN2E1MWFlYw=="
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
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
