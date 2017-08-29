# <a name="create-device"></a><span data-ttu-id="ffe23-101">Criar dispositivo</span><span class="sxs-lookup"><span data-stu-id="ffe23-101">Create device</span></span>

<span data-ttu-id="ffe23-102">Cria e registra um novo dispositivo na organização.</span><span class="sxs-lookup"><span data-stu-id="ffe23-102">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffe23-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="ffe23-103">Permissions</span></span>
<span data-ttu-id="ffe23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ffe23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="ffe23-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ffe23-106">Permission type</span></span>      | <span data-ttu-id="ffe23-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ffe23-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffe23-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ffe23-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ffe23-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ffe23-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ffe23-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ffe23-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffe23-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ffe23-111">Not supported.</span></span>    |
|<span data-ttu-id="ffe23-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ffe23-112">Application</span></span> | <span data-ttu-id="ffe23-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffe23-113">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffe23-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ffe23-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="ffe23-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ffe23-115">Request headers</span></span>
| <span data-ttu-id="ffe23-116">Nome</span><span class="sxs-lookup"><span data-stu-id="ffe23-116">Name</span></span>       | <span data-ttu-id="ffe23-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffe23-117">Type</span></span> | <span data-ttu-id="ffe23-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffe23-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ffe23-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ffe23-119">Authorization</span></span>  | <span data-ttu-id="ffe23-120">string</span><span class="sxs-lookup"><span data-stu-id="ffe23-120">string</span></span>  | <span data-ttu-id="ffe23-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ffe23-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ffe23-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="ffe23-123">Content-type</span></span> | <span data-ttu-id="ffe23-124">string</span><span class="sxs-lookup"><span data-stu-id="ffe23-124">string</span></span> | <span data-ttu-id="ffe23-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ffe23-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffe23-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ffe23-126">Request body</span></span>
<span data-ttu-id="ffe23-127">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="ffe23-127">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ffe23-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffe23-128">Response</span></span>

<span data-ttu-id="ffe23-129">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ffe23-129">If successful, this method returns `201, Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffe23-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ffe23-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ffe23-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ffe23-131">Request</span></span>
<span data-ttu-id="ffe23-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ffe23-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="ffe23-133">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="ffe23-133">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ffe23-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffe23-134">Response</span></span>
<span data-ttu-id="ffe23-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ffe23-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
