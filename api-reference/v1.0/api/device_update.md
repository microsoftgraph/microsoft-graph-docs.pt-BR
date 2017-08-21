# <a name="update-device"></a><span data-ttu-id="65478-101">Atualizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="65478-101">Update device</span></span>

<span data-ttu-id="65478-102">Atualiza as propriedades de um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="65478-102">Update the properties of a registered device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65478-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="65478-103">Prerequisites</span></span>
<span data-ttu-id="65478-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Device.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="65478-104">One of the following **scopes** is required to execute this API: *Device.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span> 

## <a name="http-request"></a><span data-ttu-id="65478-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65478-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="65478-106">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="65478-106">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65478-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65478-107">Request headers</span></span>
| <span data-ttu-id="65478-108">Nome</span><span class="sxs-lookup"><span data-stu-id="65478-108">Name</span></span>       | <span data-ttu-id="65478-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="65478-109">Type</span></span> | <span data-ttu-id="65478-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="65478-110">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="65478-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="65478-111">Authorization</span></span>  | <span data-ttu-id="65478-112">string</span><span class="sxs-lookup"><span data-stu-id="65478-112">string</span></span>  | <span data-ttu-id="65478-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65478-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65478-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65478-115">Request body</span></span>
<span data-ttu-id="65478-116">No corpo da solicitação, forneça os valores para as propriedades [device](../resources/device.md)que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="65478-116">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span>

## <a name="response"></a><span data-ttu-id="65478-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="65478-117">Response</span></span>

<span data-ttu-id="65478-118">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="65478-118">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="65478-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65478-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65478-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65478-120">Request</span></span>
<span data-ttu-id="65478-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65478-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json

{
  "accountEnabled": true
}
```
##### <a name="response"></a><span data-ttu-id="65478-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="65478-122">Response</span></span>
<span data-ttu-id="65478-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65478-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
