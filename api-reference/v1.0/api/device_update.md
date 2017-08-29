# <a name="update-device"></a><span data-ttu-id="e8e89-101">Atualizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="e8e89-101">Update device</span></span>

<span data-ttu-id="e8e89-102">Atualiza as propriedades de um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="e8e89-102">Update the properties of a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8e89-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8e89-103">Permissions</span></span>
<span data-ttu-id="e8e89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e8e89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="e8e89-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8e89-106">Permission type</span></span>      | <span data-ttu-id="e8e89-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8e89-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8e89-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8e89-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e8e89-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8e89-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e8e89-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8e89-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8e89-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8e89-111">Not supported.</span></span>    |
|<span data-ttu-id="e8e89-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8e89-112">Application</span></span> | <span data-ttu-id="e8e89-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8e89-113">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8e89-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8e89-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="e8e89-115">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="e8e89-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8e89-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e89-116">Request headers</span></span>
| <span data-ttu-id="e8e89-117">Nome</span><span class="sxs-lookup"><span data-stu-id="e8e89-117">Name</span></span>       | <span data-ttu-id="e8e89-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8e89-118">Type</span></span> | <span data-ttu-id="e8e89-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8e89-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e8e89-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8e89-120">Authorization</span></span>  | <span data-ttu-id="e8e89-121">string</span><span class="sxs-lookup"><span data-stu-id="e8e89-121">string</span></span>  | <span data-ttu-id="e8e89-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8e89-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8e89-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e89-124">Request body</span></span>
<span data-ttu-id="e8e89-125">No corpo da solicitação, forneça os valores para as propriedades [device](../resources/device.md)que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="e8e89-125">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span>

## <a name="response"></a><span data-ttu-id="e8e89-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8e89-126">Response</span></span>

<span data-ttu-id="e8e89-127">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e8e89-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e8e89-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8e89-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8e89-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e89-129">Request</span></span>
<span data-ttu-id="e8e89-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8e89-130">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e8e89-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8e89-131">Response</span></span>
<span data-ttu-id="e8e89-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8e89-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
