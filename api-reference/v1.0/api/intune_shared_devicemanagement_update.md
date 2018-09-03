# <a name="update-devicemanagement"></a><span data-ttu-id="4738d-101">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4738d-101">Update deviceManagement</span></span>

> <span data-ttu-id="4738d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4738d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4738d-103">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune_shared_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="4738d-103">Update the properties of a [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4738d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4738d-104">Prerequisites</span></span>
<span data-ttu-id="4738d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4738d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="4738d-107">Permissão&nbsp;tipo&nbsp;(por&nbsp;fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="4738d-107">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="4738d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4738d-108">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="4738d-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4738d-109">Delegated (work or school account)</span></span> |
| <span data-ttu-id="4738d-110">&nbsp; &nbsp; Auditoria</span><span class="sxs-lookup"><span data-stu-id="4738d-110">&nbsp; &nbsp;Auditing</span></span> | <span data-ttu-id="4738d-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4738d-111">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="4738d-112">&nbsp; &nbsp; Termos de empresa</span><span class="sxs-lookup"><span data-stu-id="4738d-112">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="4738d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4738d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4738d-114">&nbsp; &nbsp; Inscrição corporativa</span><span class="sxs-lookup"><span data-stu-id="4738d-114">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="4738d-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4738d-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="4738d-116">&nbsp; &nbsp; Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="4738d-116">&nbsp; &nbsp;Device configuration</span></span> | <span data-ttu-id="4738d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4738d-117">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="4738d-118">&nbsp; &nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="4738d-118">&nbsp; &nbsp;Device management</span></span> | <span data-ttu-id="4738d-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4738d-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="4738d-120">&nbsp; &nbsp; Proteção de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="4738d-120">&nbsp; &nbsp;Endpoint Protection</span></span> | <span data-ttu-id="4738d-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4738d-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="4738d-122">&nbsp; &nbsp; Registro</span><span class="sxs-lookup"><span data-stu-id="4738d-122">&nbsp; &nbsp;Enrollment</span></span> | <span data-ttu-id="4738d-123">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4738d-123">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4738d-124">&nbsp; &nbsp; Notificação</span><span class="sxs-lookup"><span data-stu-id="4738d-124">&nbsp; &nbsp;Notification</span></span> | <span data-ttu-id="4738d-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4738d-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4738d-126">&nbsp; &nbsp; Nível de contratação</span><span class="sxs-lookup"><span data-stu-id="4738d-126">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="4738d-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4738d-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4738d-128">&nbsp; &nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="4738d-128">&nbsp; &nbsp;RBAC</span></span> | <span data-ttu-id="4738d-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4738d-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="4738d-130">&nbsp; &nbsp; Assistência remota</span><span class="sxs-lookup"><span data-stu-id="4738d-130">remote assistance,</span></span> | <span data-ttu-id="4738d-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4738d-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4738d-132">&nbsp; &nbsp; Gerenciamento de despesas de telecomunicações</span><span class="sxs-lookup"><span data-stu-id="4738d-132">&nbsp; &nbsp;Telecom expense management partner</span></span> | <span data-ttu-id="4738d-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4738d-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4738d-134">&nbsp; &nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="4738d-134">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="4738d-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4738d-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="4738d-136">&nbsp; &nbsp; Proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="4738d-136">Windows information protection</span></span> | <span data-ttu-id="4738d-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4738d-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="4738d-138">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4738d-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4738d-139">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4738d-139">Not supported.</span></span>|
| <span data-ttu-id="4738d-140">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4738d-140">Application</span></span> | <span data-ttu-id="4738d-141">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4738d-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4738d-142">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4738d-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="4738d-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4738d-143">Request headers</span></span>
|<span data-ttu-id="4738d-144">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4738d-144">Header</span></span>|<span data-ttu-id="4738d-145">Valor</span><span class="sxs-lookup"><span data-stu-id="4738d-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4738d-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="4738d-146">Authorization</span></span>|<span data-ttu-id="4738d-147">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="4738d-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4738d-148">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4738d-148">Accept</span></span>|<span data-ttu-id="4738d-149">application/json</span><span class="sxs-lookup"><span data-stu-id="4738d-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4738d-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4738d-150">Request body</span></span>
<span data-ttu-id="4738d-151">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune_shared_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="4738d-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>

<span data-ttu-id="4738d-152">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune_shared_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="4738d-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune_shared_devicemanagement.md).</span></span>

|<span data-ttu-id="4738d-153">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4738d-153">Property</span></span>|<span data-ttu-id="4738d-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="4738d-154">Type</span></span>|<span data-ttu-id="4738d-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="4738d-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4738d-156">id</span><span class="sxs-lookup"><span data-stu-id="4738d-156">id</span></span>|<span data-ttu-id="4738d-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4738d-157">String</span></span>|<span data-ttu-id="4738d-158">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="4738d-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="4738d-159">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4738d-159">**Device configuration**</span></span>|
|<span data-ttu-id="4738d-160">configurações</span><span class="sxs-lookup"><span data-stu-id="4738d-160">settings</span></span>|[<span data-ttu-id="4738d-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="4738d-161">deviceManagementSettings</span></span>](../resources/intune_deviceconfig_devicemanagementsettings.md)|<span data-ttu-id="4738d-162">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="4738d-162">Account level settings.</span></span>|
|<span data-ttu-id="4738d-163">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="4738d-163">**Device management**</span></span>|
|<span data-ttu-id="4738d-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="4738d-164">subscriptionState</span></span>|[<span data-ttu-id="4738d-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="4738d-165">deviceManagementSubscriptionState</span></span>](../resources/intune_devices_devicemanagementsubscriptionstate.md)|<span data-ttu-id="4738d-166">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="4738d-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="4738d-167">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="4738d-167">The possible values are `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`, , , , , or .</span></span>|
|<span data-ttu-id="4738d-168">**Nível de contratação**</span><span class="sxs-lookup"><span data-stu-id="4738d-168">**On-boarding**</span></span>|
|<span data-ttu-id="4738d-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="4738d-169">intuneBrand</span></span>|[<span data-ttu-id="4738d-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="4738d-170">intuneBrand</span></span>](../resources/intune_onboarding_intunebrand.md)|<span data-ttu-id="4738d-171">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="4738d-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="4738d-172">O suporte de propriedade de corpo de solicitação varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="4738d-172">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="4738d-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="4738d-173">Response</span></span>
<span data-ttu-id="4738d-174">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune_shared_devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4738d-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune_shared_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4738d-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4738d-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="4738d-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4738d-176">Request</span></span>
<span data-ttu-id="4738d-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4738d-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4738d-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="4738d-178">Response</span></span>

<span data-ttu-id="4738d-179">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4738d-179">Here is an example of the response.</span></span> <span data-ttu-id="4738d-180">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="4738d-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4738d-181">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="4738d-181">Returned properties vary according to workflow and context.</span></span>

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



