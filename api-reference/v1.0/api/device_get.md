# <a name="get-device"></a><span data-ttu-id="af0c0-101">Obter dispositivo</span><span class="sxs-lookup"><span data-stu-id="af0c0-101">Get device</span></span>

<span data-ttu-id="af0c0-102">Obtém as propriedades e os relacionamentos de um objeto device.</span><span class="sxs-lookup"><span data-stu-id="af0c0-102">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="af0c0-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="af0c0-103">Permissions</span></span>
<span data-ttu-id="af0c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="af0c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="af0c0-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af0c0-106">Permission type</span></span>      | <span data-ttu-id="af0c0-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af0c0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af0c0-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af0c0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="af0c0-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="af0c0-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="af0c0-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af0c0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af0c0-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af0c0-111">Not supported.</span></span>    |
|<span data-ttu-id="af0c0-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af0c0-112">Application</span></span> | <span data-ttu-id="af0c0-113">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af0c0-113">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af0c0-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af0c0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="af0c0-115">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="af0c0-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="af0c0-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="af0c0-116">Optional query parameters</span></span>
<span data-ttu-id="af0c0-117">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="af0c0-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af0c0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af0c0-118">Request headers</span></span>
| <span data-ttu-id="af0c0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="af0c0-119">Name</span></span>       | <span data-ttu-id="af0c0-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="af0c0-120">Type</span></span> | <span data-ttu-id="af0c0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="af0c0-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="af0c0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="af0c0-122">Authorization</span></span>  | <span data-ttu-id="af0c0-123">string</span><span class="sxs-lookup"><span data-stu-id="af0c0-123">string</span></span>  | <span data-ttu-id="af0c0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af0c0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af0c0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af0c0-126">Request body</span></span>
<span data-ttu-id="af0c0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af0c0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af0c0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="af0c0-128">Response</span></span>

<span data-ttu-id="af0c0-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af0c0-129">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="af0c0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af0c0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af0c0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af0c0-131">Request</span></span>
<span data-ttu-id="af0c0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af0c0-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="af0c0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="af0c0-133">Response</span></span>
<span data-ttu-id="af0c0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af0c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
