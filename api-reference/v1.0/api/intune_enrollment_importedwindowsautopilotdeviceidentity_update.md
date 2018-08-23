# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="06862-101">Atualizar importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="06862-101">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="06862-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="06862-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06862-103">Atualizar as propriedades de um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="06862-103">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06862-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06862-104">Prerequisites</span></span>
<span data-ttu-id="06862-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="06862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="06862-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06862-107">Permission type</span></span>|<span data-ttu-id="06862-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06862-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06862-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06862-109">Delegated (work or school account)</span></span>|<span data-ttu-id="06862-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06862-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="06862-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06862-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06862-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06862-112">Not supported.</span></span>|
|<span data-ttu-id="06862-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06862-113">Application</span></span>|<span data-ttu-id="06862-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06862-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06862-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06862-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="06862-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06862-116">Request headers</span></span>
|<span data-ttu-id="06862-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06862-117">Header</span></span>|<span data-ttu-id="06862-118">Valor</span><span class="sxs-lookup"><span data-stu-id="06862-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06862-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="06862-119">Authorization</span></span>|<span data-ttu-id="06862-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="06862-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06862-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06862-121">Accept</span></span>|<span data-ttu-id="06862-122">application/json</span><span class="sxs-lookup"><span data-stu-id="06862-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06862-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06862-123">Request body</span></span>
<span data-ttu-id="06862-124">No corpo da solicitação, forneça uma representação JSON do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="06862-124">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="06862-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="06862-125">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="06862-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06862-126">Property</span></span>|<span data-ttu-id="06862-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="06862-127">Type</span></span>|<span data-ttu-id="06862-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="06862-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06862-129">id</span><span class="sxs-lookup"><span data-stu-id="06862-129">id</span></span>|<span data-ttu-id="06862-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06862-130">String</span></span>|<span data-ttu-id="06862-131">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="06862-131">The GUID for the object</span></span>|
|<span data-ttu-id="06862-132">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="06862-132">orderIdentifier</span></span>|<span data-ttu-id="06862-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06862-133">String</span></span>|<span data-ttu-id="06862-134">ID do pedido do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="06862-134">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="06862-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="06862-135">serialNumber</span></span>|<span data-ttu-id="06862-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06862-136">String</span></span>|<span data-ttu-id="06862-137">Número de série do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="06862-137">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="06862-138">productKey</span><span class="sxs-lookup"><span data-stu-id="06862-138">productKey</span></span>|<span data-ttu-id="06862-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06862-139">String</span></span>|<span data-ttu-id="06862-140">Chave do produto (Product Key) do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="06862-140">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="06862-141">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="06862-141">hardwareIdentifier</span></span>|<span data-ttu-id="06862-142">Binária</span><span class="sxs-lookup"><span data-stu-id="06862-142">Binary</span></span>|<span data-ttu-id="06862-143">Blob de hardware do dispositivo do Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="06862-143">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="06862-144">state</span><span class="sxs-lookup"><span data-stu-id="06862-144">state</span></span>|[<span data-ttu-id="06862-145">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="06862-145">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="06862-146">Estado atual do dispositivo importado.</span><span class="sxs-lookup"><span data-stu-id="06862-146">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="06862-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="06862-147">Response</span></span>
<span data-ttu-id="06862-148">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [plannerTask](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06862-148">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06862-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06862-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="06862-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06862-150">Request</span></span>
<span data-ttu-id="06862-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06862-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 464

{
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

### <a name="response"></a><span data-ttu-id="06862-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="06862-152">Response</span></span>
<span data-ttu-id="06862-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06862-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



