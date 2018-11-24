# <a name="update-devicemanagement"></a><span data-ttu-id="cf302-101">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="cf302-101">Update deviceManagement</span></span>

> <span data-ttu-id="cf302-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cf302-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf302-103">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune_shared_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="cf302-103">Update the properties of a [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf302-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf302-104">Prerequisites</span></span>
<span data-ttu-id="cf302-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cf302-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="cf302-107">Permissão&nbsp;tipo&nbsp;(por&nbsp;fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="cf302-107">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="cf302-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf302-108">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="cf302-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf302-109">Delegated (work or school account)</span></span> |
| <span data-ttu-id="cf302-110">&nbsp;&nbsp; Auditoria</span><span class="sxs-lookup"><span data-stu-id="cf302-110">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="cf302-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf302-111">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="cf302-112">&nbsp;&nbsp; Termos da empresa</span><span class="sxs-lookup"><span data-stu-id="cf302-112">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="cf302-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf302-113">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cf302-114">&nbsp;&nbsp; Inscrição corporativa</span><span class="sxs-lookup"><span data-stu-id="cf302-114">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="cf302-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf302-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="cf302-116">&nbsp;&nbsp; Configuração de dispositivo</span><span class="sxs-lookup"><span data-stu-id="cf302-116">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="cf302-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf302-117">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="cf302-118">&nbsp;&nbsp; Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="cf302-118">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="cf302-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf302-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="cf302-120">&nbsp;&nbsp; Proteção de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="cf302-120">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="cf302-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf302-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="cf302-122">&nbsp;&nbsp; Notificação</span><span class="sxs-lookup"><span data-stu-id="cf302-122">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="cf302-123">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf302-123">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cf302-124">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="cf302-124">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="cf302-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf302-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cf302-126">&nbsp;&nbsp; Controle de acesso baseado em função</span><span class="sxs-lookup"><span data-stu-id="cf302-126">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="cf302-127">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf302-127">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="cf302-128">&nbsp;&nbsp; Assistência remota</span><span class="sxs-lookup"><span data-stu-id="cf302-128">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="cf302-129">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf302-129">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cf302-130">&nbsp;&nbsp; Gerenciamento de despesas de telecomunicações</span><span class="sxs-lookup"><span data-stu-id="cf302-130">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="cf302-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf302-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cf302-132">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="cf302-132">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="cf302-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf302-133">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="cf302-134">&nbsp;&nbsp; Proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="cf302-134">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="cf302-135">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf302-135">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="cf302-136">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf302-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf302-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf302-137">Not supported.</span></span>|
| <span data-ttu-id="cf302-138">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf302-138">Application</span></span> | <span data-ttu-id="cf302-139">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf302-139">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf302-140">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf302-140">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="cf302-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf302-141">Request headers</span></span>
|<span data-ttu-id="cf302-142">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf302-142">Header</span></span>|<span data-ttu-id="cf302-143">Valor</span><span class="sxs-lookup"><span data-stu-id="cf302-143">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf302-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf302-144">Authorization</span></span>|<span data-ttu-id="cf302-145">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf302-145">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf302-146">Accept</span><span class="sxs-lookup"><span data-stu-id="cf302-146">Accept</span></span>|<span data-ttu-id="cf302-147">application/json</span><span class="sxs-lookup"><span data-stu-id="cf302-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf302-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf302-148">Request body</span></span>
<span data-ttu-id="cf302-149">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune_shared_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="cf302-149">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>

<span data-ttu-id="cf302-150">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune_shared_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="cf302-150">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune_shared_devicemanagement.md).</span></span>

|<span data-ttu-id="cf302-151">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf302-151">Property</span></span>|<span data-ttu-id="cf302-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf302-152">Type</span></span>|<span data-ttu-id="cf302-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf302-153">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf302-154">id</span><span class="sxs-lookup"><span data-stu-id="cf302-154">id</span></span>|<span data-ttu-id="cf302-155">String</span><span class="sxs-lookup"><span data-stu-id="cf302-155">String</span></span>|<span data-ttu-id="cf302-156">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cf302-156">Unique Identifier for the device</span></span>|
|<span data-ttu-id="cf302-157">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="cf302-157">**Device configuration**</span></span>|
|<span data-ttu-id="cf302-158">configurações</span><span class="sxs-lookup"><span data-stu-id="cf302-158">settings</span></span>|[<span data-ttu-id="cf302-159">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="cf302-159">deviceManagementSettings</span></span>](../resources/intune_deviceconfig_devicemanagementsettings.md)|<span data-ttu-id="cf302-160">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="cf302-160">Account level settings.</span></span>|
|<span data-ttu-id="cf302-161">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="cf302-161">**Device management**</span></span>|
|<span data-ttu-id="cf302-162">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="cf302-162">subscriptionState</span></span>|[<span data-ttu-id="cf302-163">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="cf302-163">deviceManagementSubscriptionState</span></span>](../resources/intune_devices_devicemanagementsubscriptionstate.md)|<span data-ttu-id="cf302-164">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="cf302-164">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="cf302-165">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="cf302-165">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="cf302-166">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="cf302-166">**Onboarding**</span></span>|
|<span data-ttu-id="cf302-167">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="cf302-167">intuneBrand</span></span>|[<span data-ttu-id="cf302-168">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="cf302-168">intuneBrand</span></span>](../resources/intune_onboarding_intunebrand.md)|<span data-ttu-id="cf302-169">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="cf302-169">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="cf302-170">Suporte de propriedade de corpo de solicitação varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="cf302-170">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="cf302-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf302-171">Response</span></span>
<span data-ttu-id="cf302-172">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune_shared_devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf302-172">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune_shared_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf302-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf302-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf302-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf302-174">Request</span></span>
<span data-ttu-id="cf302-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf302-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
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
```

### <a name="response"></a><span data-ttu-id="cf302-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf302-176">Response</span></span>

<span data-ttu-id="cf302-177">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf302-177">Here is an example of the response.</span></span> <span data-ttu-id="cf302-178">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="cf302-178">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cf302-179">Propriedades retornadas variam de acordo com o fluxo de trabalho e contexto.</span><span class="sxs-lookup"><span data-stu-id="cf302-179">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
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
```



