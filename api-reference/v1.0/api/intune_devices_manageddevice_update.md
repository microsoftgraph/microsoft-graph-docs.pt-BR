# <a name="update-manageddevice"></a><span data-ttu-id="7af22-101">Atualizar managedDevice</span><span class="sxs-lookup"><span data-stu-id="7af22-101">Update managedDevice</span></span>

> <span data-ttu-id="7af22-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7af22-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7af22-103">Atualizar as propriedades de um objeto [managedDevice](../resources/intune_devices_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="7af22-103">Update the properties of a [managedDevice](../resources/intune_devices_manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7af22-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7af22-104">Prerequisites</span></span>
<span data-ttu-id="7af22-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7af22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7af22-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7af22-107">Permission type</span></span>|<span data-ttu-id="7af22-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7af22-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7af22-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7af22-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7af22-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7af22-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7af22-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7af22-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7af22-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7af22-112">Not supported.</span></span>|
|<span data-ttu-id="7af22-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7af22-113">Application</span></span>|<span data-ttu-id="7af22-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7af22-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7af22-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7af22-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="7af22-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7af22-116">Request headers</span></span>
|<span data-ttu-id="7af22-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7af22-117">Header</span></span>|<span data-ttu-id="7af22-118">Valor</span><span class="sxs-lookup"><span data-stu-id="7af22-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7af22-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="7af22-119">Authorization</span></span>|<span data-ttu-id="7af22-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="7af22-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7af22-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7af22-121">Accept</span></span>|<span data-ttu-id="7af22-122">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="7af22-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7af22-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7af22-123">Request body</span></span>
<span data-ttu-id="7af22-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedDevice](../resources/intune_devices_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="7af22-124">In the request body, supply a JSON representation for the [managedDevice](../resources/intune_devices_manageddevice.md) object.</span></span>

<span data-ttu-id="7af22-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDevice](../resources/intune_devices_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="7af22-125">The following table shows the properties that are required when you create the [managedDevice](../resources/intune_devices_manageddevice.md).</span></span>

|<span data-ttu-id="7af22-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7af22-126">Property</span></span>|<span data-ttu-id="7af22-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7af22-127">Type</span></span>|<span data-ttu-id="7af22-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7af22-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7af22-129">id</span><span class="sxs-lookup"><span data-stu-id="7af22-129">id</span></span>|<span data-ttu-id="7af22-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-130">String</span></span>|<span data-ttu-id="7af22-131">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7af22-131">Unique Identifier for the device</span></span>|
|<span data-ttu-id="7af22-132">userId</span><span class="sxs-lookup"><span data-stu-id="7af22-132">userId</span></span>|<span data-ttu-id="7af22-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-133">String</span></span>|<span data-ttu-id="7af22-134">O identificador exclusivo do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="7af22-134">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="7af22-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="7af22-135">deviceName</span></span>|<span data-ttu-id="7af22-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-136">String</span></span>|<span data-ttu-id="7af22-137">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7af22-137">Name of the device</span></span>|
|<span data-ttu-id="7af22-138">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="7af22-138">managedDeviceOwnerType</span></span>|[<span data-ttu-id="7af22-139">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="7af22-139">managedDeviceOwnerType</span></span>](../resources/intune_devices_manageddeviceownertype.md)|<span data-ttu-id="7af22-p102">Propriedade do dispositivo. Pode ser 'empresa' ou 'pessoal'. Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="7af22-p102">Ownership of the device. Can be 'company' or 'personal'. The possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="7af22-143">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="7af22-143">deviceActionResults</span></span>|<span data-ttu-id="7af22-144">Coleção [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7af22-144">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) collection</span></span>|<span data-ttu-id="7af22-145">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="7af22-145">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="7af22-146">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="7af22-146">enrolledDateTime</span></span>|<span data-ttu-id="7af22-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7af22-147">DateTimeOffset</span></span>|<span data-ttu-id="7af22-148">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7af22-148">Enrollment time of the device.</span></span>|
|<span data-ttu-id="7af22-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7af22-149">lastSyncDateTime</span></span>|<span data-ttu-id="7af22-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7af22-150">DateTimeOffset</span></span>|<span data-ttu-id="7af22-151">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="7af22-151">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="7af22-152">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="7af22-152">operatingSystem</span></span>|<span data-ttu-id="7af22-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-153">String</span></span>|<span data-ttu-id="7af22-154">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7af22-154">Operating system of the device.</span></span> <span data-ttu-id="7af22-155">Windows, iOS, etc.</span><span class="sxs-lookup"><span data-stu-id="7af22-155">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="7af22-156">complianceState</span><span class="sxs-lookup"><span data-stu-id="7af22-156">complianceState</span></span>|[<span data-ttu-id="7af22-157">complianceState</span><span class="sxs-lookup"><span data-stu-id="7af22-157">complianceState</span></span>](../resources/intune_devices_compliancestate.md)|<span data-ttu-id="7af22-p104">Estado de conformidade do dispositivo. Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="7af22-p104">Compliance state of the device. The possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="7af22-160">jailBroken</span><span class="sxs-lookup"><span data-stu-id="7af22-160">jailBroken</span></span>|<span data-ttu-id="7af22-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-161">String</span></span>|<span data-ttu-id="7af22-162">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="7af22-162">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="7af22-163">managementAgent</span><span class="sxs-lookup"><span data-stu-id="7af22-163">managementAgent</span></span>|[<span data-ttu-id="7af22-164">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="7af22-164">managementAgentType</span></span>](../resources/intune_devices_managementagenttype.md)|<span data-ttu-id="7af22-p105">Canal de gerenciamento do dispositivo. Intune, EAS, etc. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="7af22-p105">Management channel of the device. Intune, EAS, etc. The possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="7af22-167">osVersion</span><span class="sxs-lookup"><span data-stu-id="7af22-167">osVersion</span></span>|<span data-ttu-id="7af22-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-168">String</span></span>|<span data-ttu-id="7af22-169">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7af22-169">Operating system version of the device.</span></span>|
|<span data-ttu-id="7af22-170">easActivated</span><span class="sxs-lookup"><span data-stu-id="7af22-170">easActivated</span></span>|<span data-ttu-id="7af22-171">Booleano</span><span class="sxs-lookup"><span data-stu-id="7af22-171">Boolean</span></span>|<span data-ttu-id="7af22-172">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="7af22-172">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="7af22-173">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="7af22-173">easDeviceId</span></span>|<span data-ttu-id="7af22-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-174">String</span></span>|<span data-ttu-id="7af22-175">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7af22-175">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="7af22-176">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="7af22-176">easActivationDateTime</span></span>|<span data-ttu-id="7af22-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7af22-177">DateTimeOffset</span></span>|<span data-ttu-id="7af22-178">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7af22-178">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="7af22-179">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="7af22-179">azureADRegistered</span></span>|<span data-ttu-id="7af22-180">Booleano</span><span class="sxs-lookup"><span data-stu-id="7af22-180">Boolean</span></span>|<span data-ttu-id="7af22-181">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7af22-181">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="7af22-182">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="7af22-182">deviceEnrollmentType</span></span>|[<span data-ttu-id="7af22-183">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="7af22-183">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="7af22-p106">Tipo de registro do dispositivo. Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="7af22-p106">Enrollment type of the device. The possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="7af22-186">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="7af22-186">activationLockBypassCode</span></span>|<span data-ttu-id="7af22-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-187">String</span></span>|<span data-ttu-id="7af22-188">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="7af22-188">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="7af22-189">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7af22-189">emailAddress</span></span>|<span data-ttu-id="7af22-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-190">String</span></span>|<span data-ttu-id="7af22-191">Email(s) do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="7af22-191">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="7af22-192">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="7af22-192">azureADDeviceId</span></span>|<span data-ttu-id="7af22-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-193">String</span></span>|<span data-ttu-id="7af22-194">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7af22-194">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="7af22-195">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7af22-195">Read only.</span></span>|
|<span data-ttu-id="7af22-196">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="7af22-196">deviceRegistrationState</span></span>|[<span data-ttu-id="7af22-197">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="7af22-197">deviceRegistrationState</span></span>](../resources/intune_devices_deviceregistrationstate.md)|<span data-ttu-id="7af22-p108">Estado do registro do dispositivo. Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="7af22-p108">Device registration state. The possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="7af22-200">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="7af22-200">deviceCategoryDisplayName</span></span>|<span data-ttu-id="7af22-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-201">String</span></span>|<span data-ttu-id="7af22-202">Nome de exibição da categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7af22-202">Device category display name</span></span>|
|<span data-ttu-id="7af22-203">isSupervised</span><span class="sxs-lookup"><span data-stu-id="7af22-203">isSupervised</span></span>|<span data-ttu-id="7af22-204">Booleano</span><span class="sxs-lookup"><span data-stu-id="7af22-204">Boolean</span></span>|<span data-ttu-id="7af22-205">Status supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7af22-205">Device supervised status</span></span>|
|<span data-ttu-id="7af22-206">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7af22-206">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="7af22-207">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7af22-207">DateTimeOffset</span></span>|<span data-ttu-id="7af22-208">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="7af22-208">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="7af22-209">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="7af22-209">exchangeAccessState</span></span>|[<span data-ttu-id="7af22-210">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="7af22-210">deviceManagementExchangeAccessState</span></span>](../resources/intune_devices_devicemanagementexchangeaccessstate.md)|<span data-ttu-id="7af22-p109">O estado de acesso do dispositivo no Exchange. Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="7af22-p109">The Access State of the device in Exchange. The possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="7af22-213">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="7af22-213">exchangeAccessStateReason</span></span>|[<span data-ttu-id="7af22-214">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="7af22-214">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune_devices_devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="7af22-p110">O motivo do estado de acesso do dispositivo no Exchange. Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="7af22-p110">The reason for the device's access state in Exchange. The possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="7af22-217">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="7af22-217">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="7af22-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-218">String</span></span>|<span data-ttu-id="7af22-219">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7af22-219">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="7af22-220">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="7af22-220">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="7af22-221">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-221">String</span></span>|<span data-ttu-id="7af22-222">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="7af22-222">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="7af22-223">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="7af22-223">isEncrypted</span></span>|<span data-ttu-id="7af22-224">Booleano</span><span class="sxs-lookup"><span data-stu-id="7af22-224">Boolean</span></span>|<span data-ttu-id="7af22-225">Status da criptografia de dispositivo</span><span class="sxs-lookup"><span data-stu-id="7af22-225">Device encryption status</span></span>|
|<span data-ttu-id="7af22-226">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7af22-226">userPrincipalName</span></span>|<span data-ttu-id="7af22-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-227">String</span></span>|<span data-ttu-id="7af22-228">Nome principal do usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7af22-228">Device user principal name</span></span>|
|<span data-ttu-id="7af22-229">modelo</span><span class="sxs-lookup"><span data-stu-id="7af22-229">model</span></span>|<span data-ttu-id="7af22-230">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-230">String</span></span>|<span data-ttu-id="7af22-231">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7af22-231">Model of the device</span></span>|
|<span data-ttu-id="7af22-232">fabricante</span><span class="sxs-lookup"><span data-stu-id="7af22-232">manufacturer</span></span>|<span data-ttu-id="7af22-233">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-233">String</span></span>|<span data-ttu-id="7af22-234">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7af22-234">Manufacturer of the device</span></span>|
|<span data-ttu-id="7af22-235">imei</span><span class="sxs-lookup"><span data-stu-id="7af22-235">imei</span></span>|<span data-ttu-id="7af22-236">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-236">String</span></span>|<span data-ttu-id="7af22-237">IMEI</span><span class="sxs-lookup"><span data-stu-id="7af22-237">IMEI</span></span>|
|<span data-ttu-id="7af22-238">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7af22-238">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="7af22-239">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7af22-239">DateTimeOffset</span></span>|<span data-ttu-id="7af22-240">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="7af22-240">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="7af22-241">serialNumber</span><span class="sxs-lookup"><span data-stu-id="7af22-241">serialNumber</span></span>|<span data-ttu-id="7af22-242">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-242">String</span></span>|<span data-ttu-id="7af22-243">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="7af22-243">SerialNumber</span></span>|
|<span data-ttu-id="7af22-244">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="7af22-244">phoneNumber</span></span>|<span data-ttu-id="7af22-245">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-245">String</span></span>|<span data-ttu-id="7af22-246">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7af22-246">Phone number of the device</span></span>|
|<span data-ttu-id="7af22-247">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="7af22-247">androidSecurityPatchLevel</span></span>|<span data-ttu-id="7af22-248">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-248">String</span></span>|<span data-ttu-id="7af22-249">Nível do patch de segurança Android</span><span class="sxs-lookup"><span data-stu-id="7af22-249">Android security patch level</span></span>|
|<span data-ttu-id="7af22-250">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7af22-250">userDisplayName</span></span>|<span data-ttu-id="7af22-251">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-251">String</span></span>|<span data-ttu-id="7af22-252">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="7af22-252">User display name</span></span>|
|<span data-ttu-id="7af22-253">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="7af22-253">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="7af22-254">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="7af22-254">configurationManagerClientEnabledFeatures</span></span>](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="7af22-255">Recursos habilitados pelo cliente do ConfigrMgr</span><span class="sxs-lookup"><span data-stu-id="7af22-255">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="7af22-256">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="7af22-256">wiFiMacAddress</span></span>|<span data-ttu-id="7af22-257">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-257">String</span></span>|<span data-ttu-id="7af22-258">MAC Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="7af22-258">Wi-Fi MAC</span></span>|
|<span data-ttu-id="7af22-259">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="7af22-259">deviceHealthAttestationState</span></span>|[<span data-ttu-id="7af22-260">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="7af22-260">deviceHealthAttestationState</span></span>](../resources/intune_devices_devicehealthattestationstate.md)|<span data-ttu-id="7af22-261">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7af22-261">The device health attestation state.</span></span>|
|<span data-ttu-id="7af22-262">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="7af22-262">subscriberCarrier</span></span>|<span data-ttu-id="7af22-263">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-263">String</span></span>|<span data-ttu-id="7af22-264">Operadora do assinante</span><span class="sxs-lookup"><span data-stu-id="7af22-264">Subscriber Carrier</span></span>|
|<span data-ttu-id="7af22-265">meid</span><span class="sxs-lookup"><span data-stu-id="7af22-265">meid</span></span>|<span data-ttu-id="7af22-266">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-266">String</span></span>|<span data-ttu-id="7af22-267">MEID</span><span class="sxs-lookup"><span data-stu-id="7af22-267">MEID</span></span>|
|<span data-ttu-id="7af22-268">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="7af22-268">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="7af22-269">Int64</span><span class="sxs-lookup"><span data-stu-id="7af22-269">Int64</span></span>|<span data-ttu-id="7af22-270">Total de armazenamento em bytes</span><span class="sxs-lookup"><span data-stu-id="7af22-270">Total Storage in Bytes</span></span>|
|<span data-ttu-id="7af22-271">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="7af22-271">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="7af22-272">Int64</span><span class="sxs-lookup"><span data-stu-id="7af22-272">Int64</span></span>|<span data-ttu-id="7af22-273">Armazenamento gratuito em bytes</span><span class="sxs-lookup"><span data-stu-id="7af22-273">Free Storage in Bytes</span></span>|
|<span data-ttu-id="7af22-274">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="7af22-274">managedDeviceName</span></span>|<span data-ttu-id="7af22-275">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7af22-275">String</span></span>|<span data-ttu-id="7af22-276">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7af22-276">Automatically generated name to identify a device.</span></span> <span data-ttu-id="7af22-277">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="7af22-277">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="7af22-278">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="7af22-278">partnerReportedThreatState</span></span>|[<span data-ttu-id="7af22-279">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="7af22-279">managedDevicePartnerReportedHealthState</span></span>](../resources/intune_devices_manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="7af22-p112">Indica o estado de ameaça de um dispositivo quando um parceiro do Mobile Threat Defense está em uso pela conta e pelo dispositivo. Somente leitura. Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="7af22-p112">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span>|



## <a name="response"></a><span data-ttu-id="7af22-283">Resposta</span><span class="sxs-lookup"><span data-stu-id="7af22-283">Response</span></span>
<span data-ttu-id="7af22-284">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune_devices_manageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7af22-284">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune_devices_manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7af22-285">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7af22-285">Example</span></span>
### <a name="request"></a><span data-ttu-id="7af22-286">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7af22-286">Request</span></span>
<span data-ttu-id="7af22-287">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7af22-287">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 4604

{
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated"
}
```

### <a name="response"></a><span data-ttu-id="7af22-288">Resposta</span><span class="sxs-lookup"><span data-stu-id="7af22-288">Response</span></span>
<span data-ttu-id="7af22-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7af22-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4705

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated"
}
```








