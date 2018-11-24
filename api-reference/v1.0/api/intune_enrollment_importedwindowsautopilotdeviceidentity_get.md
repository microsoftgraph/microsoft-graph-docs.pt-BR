# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="20e8a-101">Obter importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="20e8a-101">Get importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="20e8a-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="20e8a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20e8a-103">Lê as propriedades e relações do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="20e8a-103">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20e8a-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20e8a-104">Prerequisites</span></span>
<span data-ttu-id="20e8a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="20e8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="20e8a-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20e8a-107">Permission type</span></span>|<span data-ttu-id="20e8a-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="20e8a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20e8a-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20e8a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="20e8a-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="20e8a-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="20e8a-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20e8a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20e8a-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20e8a-112">Not supported.</span></span>|
|<span data-ttu-id="20e8a-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20e8a-113">Application</span></span>|<span data-ttu-id="20e8a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20e8a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20e8a-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20e8a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20e8a-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="20e8a-116">Optional query parameters</span></span>
<span data-ttu-id="20e8a-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="20e8a-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="20e8a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20e8a-118">Request headers</span></span>
|<span data-ttu-id="20e8a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20e8a-119">Header</span></span>|<span data-ttu-id="20e8a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="20e8a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20e8a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="20e8a-121">Authorization</span></span>|<span data-ttu-id="20e8a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20e8a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20e8a-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="20e8a-123">Accept</span></span>|<span data-ttu-id="20e8a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="20e8a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20e8a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20e8a-125">Request body</span></span>
<span data-ttu-id="20e8a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20e8a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20e8a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="20e8a-127">Response</span></span>
<span data-ttu-id="20e8a-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20e8a-128">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20e8a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20e8a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="20e8a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20e8a-130">Request</span></span>
<span data-ttu-id="20e8a-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20e8a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="20e8a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="20e8a-132">Response</span></span>
<span data-ttu-id="20e8a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20e8a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 635

{
  "value": {
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
}
```



