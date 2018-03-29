# <a name="create-manageddevice"></a><span data-ttu-id="7007c-101">Criar managedDevice</span><span class="sxs-lookup"><span data-stu-id="7007c-101">Create managedDevice</span></span>

> <span data-ttu-id="7007c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7007c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7007c-103">Criar um novo objeto [managedDevice](../resources/intune_devices_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="7007c-103">Create a new [plannerBucket](../resources/intune_devices_manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7007c-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7007c-104">Prerequisites</span></span>
<span data-ttu-id="7007c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7007c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7007c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7007c-107">Permission type</span></span>|<span data-ttu-id="7007c-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7007c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7007c-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7007c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7007c-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7007c-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7007c-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7007c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7007c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7007c-112">Not supported.</span></span>|
|<span data-ttu-id="7007c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7007c-113">Application</span></span>|<span data-ttu-id="7007c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7007c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7007c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7007c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="7007c-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7007c-116">Request headers</span></span>
|<span data-ttu-id="7007c-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7007c-117">Header</span></span>|<span data-ttu-id="7007c-118">Valor</span><span class="sxs-lookup"><span data-stu-id="7007c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7007c-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="7007c-119">Authorization</span></span>|<span data-ttu-id="7007c-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7007c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7007c-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7007c-121">Accept</span></span>|<span data-ttu-id="7007c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7007c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7007c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7007c-123">Request body</span></span>
<span data-ttu-id="7007c-124">No corpo da solicitação, forneça uma representação JSON do objeto managedDevice.</span><span class="sxs-lookup"><span data-stu-id="7007c-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="7007c-125">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDevice.</span><span class="sxs-lookup"><span data-stu-id="7007c-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="7007c-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7007c-126">Property</span></span>|<span data-ttu-id="7007c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7007c-127">Type</span></span>|<span data-ttu-id="7007c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7007c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7007c-129">id</span><span class="sxs-lookup"><span data-stu-id="7007c-129">id</span></span>|<span data-ttu-id="7007c-130">String</span><span class="sxs-lookup"><span data-stu-id="7007c-130">String</span></span>|<span data-ttu-id="7007c-131">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7007c-131">Unique Identifier for the device</span></span>|
|<span data-ttu-id="7007c-132">userId</span><span class="sxs-lookup"><span data-stu-id="7007c-132">userId</span></span>|<span data-ttu-id="7007c-133">String</span><span class="sxs-lookup"><span data-stu-id="7007c-133">String</span></span>|<span data-ttu-id="7007c-134">O identificador exclusivo do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="7007c-134">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="7007c-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="7007c-135">deviceName</span></span>|<span data-ttu-id="7007c-136">String</span><span class="sxs-lookup"><span data-stu-id="7007c-136">String</span></span>|<span data-ttu-id="7007c-137">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7007c-137">Name of the device</span></span>|
|<span data-ttu-id="7007c-138">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="7007c-138">deviceActionResults</span></span>|<span data-ttu-id="7007c-139">Coleção [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7007c-139">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) collection</span></span>|<span data-ttu-id="7007c-140">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="7007c-140">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="7007c-141">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="7007c-141">enrolledDateTime</span></span>|<span data-ttu-id="7007c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7007c-142">DateTimeOffset</span></span>|<span data-ttu-id="7007c-143">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7007c-143">Enrollment time of the device.</span></span>|
|<span data-ttu-id="7007c-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7007c-144">lastSyncDateTime</span></span>|<span data-ttu-id="7007c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7007c-145">DateTimeOffset</span></span>|<span data-ttu-id="7007c-146">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="7007c-146">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="7007c-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="7007c-147">operatingSystem</span></span>|<span data-ttu-id="7007c-148">String</span><span class="sxs-lookup"><span data-stu-id="7007c-148">String</span></span>|<span data-ttu-id="7007c-149">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7007c-149">Operating system of the device.</span></span> <span data-ttu-id="7007c-150">Windows, iOS, etc.</span><span class="sxs-lookup"><span data-stu-id="7007c-150">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="7007c-151">complianceState</span><span class="sxs-lookup"><span data-stu-id="7007c-151">complianceState</span></span>|<span data-ttu-id="7007c-152">String</span><span class="sxs-lookup"><span data-stu-id="7007c-152">String</span></span>|<span data-ttu-id="7007c-153">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7007c-153">Compliance state of the device.</span></span> <span data-ttu-id="7007c-154">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="7007c-154">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="7007c-155">jailBroken</span><span class="sxs-lookup"><span data-stu-id="7007c-155">jailBroken</span></span>|<span data-ttu-id="7007c-156">String</span><span class="sxs-lookup"><span data-stu-id="7007c-156">String</span></span>|<span data-ttu-id="7007c-157">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="7007c-157">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="7007c-158">managementAgent</span><span class="sxs-lookup"><span data-stu-id="7007c-158">managementAgent</span></span>|<span data-ttu-id="7007c-159">String</span><span class="sxs-lookup"><span data-stu-id="7007c-159">String</span></span>|<span data-ttu-id="7007c-160">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7007c-160">Management channel of the device.</span></span> <span data-ttu-id="7007c-161">Intune, EAS, etc. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="7007c-161">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="7007c-162">osVersion</span><span class="sxs-lookup"><span data-stu-id="7007c-162">osVersion</span></span>|<span data-ttu-id="7007c-163">String</span><span class="sxs-lookup"><span data-stu-id="7007c-163">String</span></span>|<span data-ttu-id="7007c-164">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7007c-164">Operating system version of the device.</span></span>|
|<span data-ttu-id="7007c-165">easActivated</span><span class="sxs-lookup"><span data-stu-id="7007c-165">easActivated</span></span>|<span data-ttu-id="7007c-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="7007c-166">Boolean</span></span>|<span data-ttu-id="7007c-167">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="7007c-167">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="7007c-168">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="7007c-168">easDeviceId</span></span>|<span data-ttu-id="7007c-169">String</span><span class="sxs-lookup"><span data-stu-id="7007c-169">String</span></span>|<span data-ttu-id="7007c-170">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7007c-170">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="7007c-171">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="7007c-171">easActivationDateTime</span></span>|<span data-ttu-id="7007c-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7007c-172">DateTimeOffset</span></span>|<span data-ttu-id="7007c-173">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7007c-173">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="7007c-174">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="7007c-174">azureADRegistered</span></span>|<span data-ttu-id="7007c-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="7007c-175">Boolean</span></span>|<span data-ttu-id="7007c-176">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7007c-176">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="7007c-177">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="7007c-177">deviceEnrollmentType</span></span>|<span data-ttu-id="7007c-178">String</span><span class="sxs-lookup"><span data-stu-id="7007c-178">String</span></span>|<span data-ttu-id="7007c-179">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7007c-179">Enrollment type of the device.</span></span> <span data-ttu-id="7007c-180">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="7007c-180">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="7007c-181">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="7007c-181">activationLockBypassCode</span></span>|<span data-ttu-id="7007c-182">String</span><span class="sxs-lookup"><span data-stu-id="7007c-182">String</span></span>|<span data-ttu-id="7007c-183">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="7007c-183">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="7007c-184">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7007c-184">emailAddress</span></span>|<span data-ttu-id="7007c-185">String</span><span class="sxs-lookup"><span data-stu-id="7007c-185">String</span></span>|<span data-ttu-id="7007c-186">Email(s) do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="7007c-186">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="7007c-187">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="7007c-187">azureADDeviceId</span></span>|<span data-ttu-id="7007c-188">String</span><span class="sxs-lookup"><span data-stu-id="7007c-188">String</span></span>|<span data-ttu-id="7007c-189">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7007c-189">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="7007c-190">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7007c-190">Read only.</span></span>|
|<span data-ttu-id="7007c-191">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="7007c-191">deviceRegistrationState</span></span>|<span data-ttu-id="7007c-192">String</span><span class="sxs-lookup"><span data-stu-id="7007c-192">String</span></span>|<span data-ttu-id="7007c-193">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7007c-193">Device registration state.</span></span> <span data-ttu-id="7007c-194">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="7007c-194">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`.</span></span>|
|<span data-ttu-id="7007c-195">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="7007c-195">deviceCategoryDisplayName</span></span>|<span data-ttu-id="7007c-196">String</span><span class="sxs-lookup"><span data-stu-id="7007c-196">String</span></span>|<span data-ttu-id="7007c-197">Nome de exibição da categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7007c-197">Device category display name</span></span>|
|<span data-ttu-id="7007c-198">isSupervised</span><span class="sxs-lookup"><span data-stu-id="7007c-198">isSupervised</span></span>|<span data-ttu-id="7007c-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="7007c-199">Boolean</span></span>|<span data-ttu-id="7007c-200">Status supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7007c-200">Device supervised status</span></span>|
|<span data-ttu-id="7007c-201">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7007c-201">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="7007c-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7007c-202">DateTimeOffset</span></span>|<span data-ttu-id="7007c-203">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="7007c-203">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="7007c-204">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="7007c-204">exchangeAccessState</span></span>|<span data-ttu-id="7007c-205">String</span><span class="sxs-lookup"><span data-stu-id="7007c-205">String</span></span>|<span data-ttu-id="7007c-206">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="7007c-206">The Access State of the device in Exchange.</span></span> <span data-ttu-id="7007c-207">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="7007c-207">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="7007c-208">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="7007c-208">exchangeAccessStateReason</span></span>|<span data-ttu-id="7007c-209">String</span><span class="sxs-lookup"><span data-stu-id="7007c-209">String</span></span>|<span data-ttu-id="7007c-210">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="7007c-210">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="7007c-211">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="7007c-211">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="7007c-212">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="7007c-212">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="7007c-213">String</span><span class="sxs-lookup"><span data-stu-id="7007c-213">String</span></span>|<span data-ttu-id="7007c-214">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7007c-214">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="7007c-215">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="7007c-215">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="7007c-216">String</span><span class="sxs-lookup"><span data-stu-id="7007c-216">String</span></span>|<span data-ttu-id="7007c-217">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="7007c-217">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="7007c-218">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="7007c-218">isEncrypted</span></span>|<span data-ttu-id="7007c-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="7007c-219">Boolean</span></span>|<span data-ttu-id="7007c-220">Status da criptografia de dispositivo</span><span class="sxs-lookup"><span data-stu-id="7007c-220">Device encryption status</span></span>|
|<span data-ttu-id="7007c-221">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7007c-221">userPrincipalName</span></span>|<span data-ttu-id="7007c-222">String</span><span class="sxs-lookup"><span data-stu-id="7007c-222">String</span></span>|<span data-ttu-id="7007c-223">Nome principal do usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7007c-223">Device user principal name</span></span>|
|<span data-ttu-id="7007c-224">modelo</span><span class="sxs-lookup"><span data-stu-id="7007c-224">model</span></span>|<span data-ttu-id="7007c-225">String</span><span class="sxs-lookup"><span data-stu-id="7007c-225">String</span></span>|<span data-ttu-id="7007c-226">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7007c-226">Model of the device</span></span>|
|<span data-ttu-id="7007c-227">fabricante</span><span class="sxs-lookup"><span data-stu-id="7007c-227">Camera manufacturer.</span></span>|<span data-ttu-id="7007c-228">String</span><span class="sxs-lookup"><span data-stu-id="7007c-228">String</span></span>|<span data-ttu-id="7007c-229">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7007c-229">Manufacturer of the device</span></span>|
|<span data-ttu-id="7007c-230">imei</span><span class="sxs-lookup"><span data-stu-id="7007c-230">imei</span></span>|<span data-ttu-id="7007c-231">String</span><span class="sxs-lookup"><span data-stu-id="7007c-231">String</span></span>|<span data-ttu-id="7007c-232">IMEI</span><span class="sxs-lookup"><span data-stu-id="7007c-232">IMEI</span></span>|
|<span data-ttu-id="7007c-233">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7007c-233">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="7007c-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7007c-234">DateTimeOffset</span></span>|<span data-ttu-id="7007c-235">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="7007c-235">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="7007c-236">serialNumber</span><span class="sxs-lookup"><span data-stu-id="7007c-236">serialNumber</span></span>|<span data-ttu-id="7007c-237">String</span><span class="sxs-lookup"><span data-stu-id="7007c-237">String</span></span>|<span data-ttu-id="7007c-238">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="7007c-238">SerialNumber</span></span>|
|<span data-ttu-id="7007c-239">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="7007c-239">PhoneNumber</span></span>|<span data-ttu-id="7007c-240">String</span><span class="sxs-lookup"><span data-stu-id="7007c-240">String</span></span>|<span data-ttu-id="7007c-241">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7007c-241">Phone number of the device</span></span>|
|<span data-ttu-id="7007c-242">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="7007c-242">androidSecurityPatchLevel</span></span>|<span data-ttu-id="7007c-243">String</span><span class="sxs-lookup"><span data-stu-id="7007c-243">String</span></span>|<span data-ttu-id="7007c-244">Nível do patch de segurança Android</span><span class="sxs-lookup"><span data-stu-id="7007c-244">Android security patch level</span></span>|
|<span data-ttu-id="7007c-245">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7007c-245">userDisplayName</span></span>|<span data-ttu-id="7007c-246">String</span><span class="sxs-lookup"><span data-stu-id="7007c-246">String</span></span>|<span data-ttu-id="7007c-247">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="7007c-247">user display name</span></span>|
|<span data-ttu-id="7007c-248">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="7007c-248">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="7007c-249">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="7007c-249">configurationManagerClientEnabledFeatures</span></span>](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="7007c-250">Recursos habilitados pelo cliente do ConfigrMgr</span><span class="sxs-lookup"><span data-stu-id="7007c-250">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="7007c-251">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="7007c-251">wiFiMacAddress</span></span>|<span data-ttu-id="7007c-252">String</span><span class="sxs-lookup"><span data-stu-id="7007c-252">String</span></span>|<span data-ttu-id="7007c-253">MAC Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="7007c-253">Wi-Fi MAC</span></span>|
|<span data-ttu-id="7007c-254">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="7007c-254">deviceHealthAttestationState</span></span>|[<span data-ttu-id="7007c-255">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="7007c-255">deviceHealthAttestationState</span></span>](../resources/intune_devices_devicehealthattestationstate.md)|<span data-ttu-id="7007c-256">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7007c-256">The device health attestation state.</span></span>|
|<span data-ttu-id="7007c-257">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="7007c-257">subscriberCarrier</span></span>|<span data-ttu-id="7007c-258">String</span><span class="sxs-lookup"><span data-stu-id="7007c-258">String</span></span>|<span data-ttu-id="7007c-259">Operadora do assinante</span><span class="sxs-lookup"><span data-stu-id="7007c-259">Subscriber Carrier</span></span>|
|<span data-ttu-id="7007c-260">meid</span><span class="sxs-lookup"><span data-stu-id="7007c-260">meid</span></span>|<span data-ttu-id="7007c-261">String</span><span class="sxs-lookup"><span data-stu-id="7007c-261">String</span></span>|<span data-ttu-id="7007c-262">MEID</span><span class="sxs-lookup"><span data-stu-id="7007c-262">MEID</span></span>|
|<span data-ttu-id="7007c-263">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="7007c-263">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="7007c-264">Int64</span><span class="sxs-lookup"><span data-stu-id="7007c-264">Int64</span></span>|<span data-ttu-id="7007c-265">Total de armazenamento em bytes</span><span class="sxs-lookup"><span data-stu-id="7007c-265">Total Storage in Bytes</span></span>|
|<span data-ttu-id="7007c-266">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="7007c-266">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="7007c-267">Int64</span><span class="sxs-lookup"><span data-stu-id="7007c-267">Int64</span></span>|<span data-ttu-id="7007c-268">Armazenamento gratuito em bytes</span><span class="sxs-lookup"><span data-stu-id="7007c-268">Free Storage in Bytes</span></span>|
|<span data-ttu-id="7007c-269">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="7007c-269">managedDeviceName</span></span>|<span data-ttu-id="7007c-270">String</span><span class="sxs-lookup"><span data-stu-id="7007c-270">String</span></span>|<span data-ttu-id="7007c-271">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7007c-271">Automatically generated name to identify a device.</span></span> <span data-ttu-id="7007c-272">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="7007c-272">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="7007c-273">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="7007c-273">partnerReportedThreatState</span></span>|<span data-ttu-id="7007c-274">String</span><span class="sxs-lookup"><span data-stu-id="7007c-274">String</span></span>|<span data-ttu-id="7007c-275">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra Ameaças Móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7007c-275">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="7007c-276">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7007c-276">Read only.</span></span> <span data-ttu-id="7007c-277">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="7007c-277">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`.</span></span>|



## <a name="response"></a><span data-ttu-id="7007c-278">Resposta</span><span class="sxs-lookup"><span data-stu-id="7007c-278">Response</span></span>
<span data-ttu-id="7007c-279">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedDevice](../resources/intune_devices_manageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7007c-279">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_devices_manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7007c-280">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7007c-280">Example</span></span>
### <a name="request"></a><span data-ttu-id="7007c-281">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7007c-281">Request</span></span>
<span data-ttu-id="7007c-282">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7007c-282">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 4616

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
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

### <a name="response"></a><span data-ttu-id="7007c-283">Resposta</span><span class="sxs-lookup"><span data-stu-id="7007c-283">Response</span></span>
<span data-ttu-id="7007c-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7007c-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4665

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
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



