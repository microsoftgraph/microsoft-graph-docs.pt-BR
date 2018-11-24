# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="a8e0f-101">Criar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a8e0f-101">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="a8e0f-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8e0f-103">Criar um novo objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="a8e0f-103">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8e0f-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8e0f-104">Prerequisites</span></span>
<span data-ttu-id="a8e0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a8e0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a8e0f-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8e0f-107">Permission type</span></span>|<span data-ttu-id="a8e0f-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a8e0f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8e0f-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8e0f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a8e0f-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8e0f-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a8e0f-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8e0f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8e0f-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-112">Not supported.</span></span>|
|<span data-ttu-id="a8e0f-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8e0f-113">Application</span></span>|<span data-ttu-id="a8e0f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8e0f-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8e0f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="a8e0f-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e0f-116">Request headers</span></span>
|<span data-ttu-id="a8e0f-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8e0f-117">Header</span></span>|<span data-ttu-id="a8e0f-118">Valor</span><span class="sxs-lookup"><span data-stu-id="a8e0f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8e0f-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8e0f-119">Authorization</span></span>|<span data-ttu-id="a8e0f-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8e0f-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8e0f-121">Accept</span></span>|<span data-ttu-id="a8e0f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a8e0f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8e0f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e0f-123">Request body</span></span>
<span data-ttu-id="a8e0f-124">No corpo da solicitação, forneça uma representação JSON do objeto importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-124">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="a8e0f-125">A tabela a seguir mostra as propriedades que são necessárias ao criar importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-125">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="a8e0f-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8e0f-126">Property</span></span>|<span data-ttu-id="a8e0f-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8e0f-127">Type</span></span>|<span data-ttu-id="a8e0f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8e0f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8e0f-129">id</span><span class="sxs-lookup"><span data-stu-id="a8e0f-129">id</span></span>|<span data-ttu-id="a8e0f-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8e0f-130">String</span></span>|<span data-ttu-id="a8e0f-131">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-131">The GUID for the object</span></span>|
|<span data-ttu-id="a8e0f-132">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="a8e0f-132">orderIdentifier</span></span>|<span data-ttu-id="a8e0f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8e0f-133">String</span></span>|<span data-ttu-id="a8e0f-134">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-134">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a8e0f-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="a8e0f-135">serialNumber</span></span>|<span data-ttu-id="a8e0f-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8e0f-136">String</span></span>|<span data-ttu-id="a8e0f-137">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-137">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a8e0f-138">productKey</span><span class="sxs-lookup"><span data-stu-id="a8e0f-138">productKey</span></span>|<span data-ttu-id="a8e0f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8e0f-139">String</span></span>|<span data-ttu-id="a8e0f-140">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-140">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a8e0f-141">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="a8e0f-141">hardwareIdentifier</span></span>|<span data-ttu-id="a8e0f-142">Binária</span><span class="sxs-lookup"><span data-stu-id="a8e0f-142">Binary</span></span>|<span data-ttu-id="a8e0f-143">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-143">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a8e0f-144">state</span><span class="sxs-lookup"><span data-stu-id="a8e0f-144">state</span></span>|[<span data-ttu-id="a8e0f-145">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="a8e0f-145">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="a8e0f-146">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-146">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="a8e0f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8e0f-147">Response</span></span>
<span data-ttu-id="a8e0f-148">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-148">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8e0f-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8e0f-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8e0f-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e0f-150">Request</span></span>
<span data-ttu-id="a8e0f-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 541

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```

### <a name="response"></a><span data-ttu-id="a8e0f-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8e0f-152">Response</span></span>
<span data-ttu-id="a8e0f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8e0f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 590

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```



