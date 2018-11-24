# <a name="get-devicemanagement"></a><span data-ttu-id="cca3d-101">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="cca3d-101">Get deviceManagement</span></span>

> <span data-ttu-id="cca3d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cca3d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cca3d-103">Ler propriedades e relações do objeto [deviceManagement](../resources/intune_shared_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="cca3d-103">Read properties and relationships of the [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cca3d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cca3d-104">Prerequisites</span></span>
<span data-ttu-id="cca3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cca3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="cca3d-107">Permissão&nbsp;tipo&nbsp;(por&nbsp;fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="cca3d-107">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="cca3d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cca3d-108">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="cca3d-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cca3d-109">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="cca3d-110">&nbsp;&nbsp; Auditoria</span><span class="sxs-lookup"><span data-stu-id="cca3d-110">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="cca3d-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cca3d-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="cca3d-112">&nbsp;&nbsp; Termos da empresa</span><span class="sxs-lookup"><span data-stu-id="cca3d-112">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="cca3d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cca3d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="cca3d-114">&nbsp;&nbsp; Configuração de dispositivo</span><span class="sxs-lookup"><span data-stu-id="cca3d-114">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="cca3d-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cca3d-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="cca3d-116">&nbsp;&nbsp; Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="cca3d-116">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="cca3d-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cca3d-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="cca3d-118">&nbsp;&nbsp; Inscrição</span><span class="sxs-lookup"><span data-stu-id="cca3d-118">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="cca3d-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cca3d-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="cca3d-120">&nbsp;&nbsp; Notificação</span><span class="sxs-lookup"><span data-stu-id="cca3d-120">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="cca3d-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cca3d-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="cca3d-122">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="cca3d-122">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="cca3d-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cca3d-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="cca3d-124">&nbsp;&nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="cca3d-124">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="cca3d-125">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="cca3d-125">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="cca3d-126">&nbsp;&nbsp; Assistência remota</span><span class="sxs-lookup"><span data-stu-id="cca3d-126">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="cca3d-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cca3d-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="cca3d-128">&nbsp;&nbsp; Gerenciamento de despesas de telecomunicações</span><span class="sxs-lookup"><span data-stu-id="cca3d-128">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="cca3d-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cca3d-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="cca3d-130">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="cca3d-130">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="cca3d-131">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cca3d-131">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="cca3d-132">&nbsp;&nbsp; Proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="cca3d-132">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="cca3d-133">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cca3d-133">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="cca3d-134">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cca3d-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cca3d-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cca3d-135">Not supported.</span></span>|
| <span data-ttu-id="cca3d-136">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cca3d-136">Application</span></span> | <span data-ttu-id="cca3d-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cca3d-137">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="cca3d-138">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cca3d-138">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cca3d-139">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cca3d-139">Optional query parameters</span></span>
<span data-ttu-id="cca3d-140">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cca3d-140">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cca3d-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cca3d-141">Request headers</span></span>
|<span data-ttu-id="cca3d-142">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cca3d-142">Header</span></span>|<span data-ttu-id="cca3d-143">Valor</span><span class="sxs-lookup"><span data-stu-id="cca3d-143">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cca3d-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="cca3d-144">Authorization</span></span>|<span data-ttu-id="cca3d-145">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cca3d-145">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cca3d-146">Accept</span><span class="sxs-lookup"><span data-stu-id="cca3d-146">Accept</span></span>|<span data-ttu-id="cca3d-147">application/json</span><span class="sxs-lookup"><span data-stu-id="cca3d-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cca3d-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cca3d-148">Request body</span></span>
<span data-ttu-id="cca3d-149">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cca3d-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cca3d-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="cca3d-150">Response</span></span>
<span data-ttu-id="cca3d-151">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune_shared_devicemanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cca3d-151">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune_shared_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cca3d-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cca3d-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="cca3d-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cca3d-153">Request</span></span>
<span data-ttu-id="cca3d-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cca3d-154">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="cca3d-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="cca3d-155">Response</span></span>
<span data-ttu-id="cca3d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cca3d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
  }
}
```



