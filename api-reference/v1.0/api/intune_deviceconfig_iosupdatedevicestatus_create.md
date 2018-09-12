# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="65bff-101">Criar iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="65bff-101">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="65bff-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="65bff-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65bff-103">Criar um novo objeto [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="65bff-103">Create a new [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="65bff-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="65bff-104">Prerequisites</span></span>
<span data-ttu-id="65bff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="65bff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="65bff-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65bff-107">Permission type</span></span>|<span data-ttu-id="65bff-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="65bff-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65bff-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65bff-109">Delegated (work or school account)</span></span>|<span data-ttu-id="65bff-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65bff-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65bff-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65bff-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65bff-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65bff-112">Not supported.</span></span>|
|<span data-ttu-id="65bff-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65bff-113">Application</span></span>|<span data-ttu-id="65bff-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65bff-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65bff-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65bff-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="65bff-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65bff-116">Request headers</span></span>
|<span data-ttu-id="65bff-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65bff-117">Header</span></span>|<span data-ttu-id="65bff-118">Valor</span><span class="sxs-lookup"><span data-stu-id="65bff-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65bff-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="65bff-119">Authorization</span></span>|<span data-ttu-id="65bff-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="65bff-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65bff-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="65bff-121">Accept</span></span>|<span data-ttu-id="65bff-122">application/json</span><span class="sxs-lookup"><span data-stu-id="65bff-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65bff-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65bff-123">Request body</span></span>
<span data-ttu-id="65bff-124">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="65bff-124">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="65bff-125">A tabela a seguir mostra as propriedades que são necessárias ao criar iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="65bff-125">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="65bff-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65bff-126">Property</span></span>|<span data-ttu-id="65bff-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="65bff-127">Type</span></span>|<span data-ttu-id="65bff-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="65bff-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65bff-129">id</span><span class="sxs-lookup"><span data-stu-id="65bff-129">id</span></span>|<span data-ttu-id="65bff-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65bff-130">String</span></span>|<span data-ttu-id="65bff-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="65bff-131">Key of the entity.</span></span>|
|<span data-ttu-id="65bff-132">installStatus</span><span class="sxs-lookup"><span data-stu-id="65bff-132">installStatus</span></span>|[<span data-ttu-id="65bff-133">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="65bff-133">iosUpdatesInstallStatus</span></span>](../resources/intune_deviceconfig_iosupdatesinstallstatus.md)|<span data-ttu-id="65bff-p102">O status de instalação do relatório de política. Os valores possíveis são: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="65bff-p102">The installation status of the policy report. The possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="65bff-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="65bff-136">osVersion</span></span>|<span data-ttu-id="65bff-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65bff-137">String</span></span>|<span data-ttu-id="65bff-138">A versão do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="65bff-138">The device version that is being reported.</span></span>|
|<span data-ttu-id="65bff-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="65bff-139">deviceId</span></span>|<span data-ttu-id="65bff-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65bff-140">String</span></span>|<span data-ttu-id="65bff-141">A ID do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="65bff-141">The device id that is being reported.</span></span>|
|<span data-ttu-id="65bff-142">userId</span><span class="sxs-lookup"><span data-stu-id="65bff-142">userId</span></span>|<span data-ttu-id="65bff-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65bff-143">String</span></span>|<span data-ttu-id="65bff-144">A ID do usuário que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="65bff-144">The User id that is being reported.</span></span>|
|<span data-ttu-id="65bff-145">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="65bff-145">deviceDisplayName</span></span>|<span data-ttu-id="65bff-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65bff-146">String</span></span>|<span data-ttu-id="65bff-147">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="65bff-147">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="65bff-148">userName</span><span class="sxs-lookup"><span data-stu-id="65bff-148">userName</span></span>|<span data-ttu-id="65bff-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65bff-149">String</span></span>|<span data-ttu-id="65bff-150">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="65bff-150">The User Name that is being reported</span></span>|
|<span data-ttu-id="65bff-151">deviceModel</span><span class="sxs-lookup"><span data-stu-id="65bff-151">deviceModel</span></span>|<span data-ttu-id="65bff-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65bff-152">String</span></span>|<span data-ttu-id="65bff-153">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="65bff-153">The device model that is being reported</span></span>|
|<span data-ttu-id="65bff-154">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="65bff-154">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="65bff-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65bff-155">DateTimeOffset</span></span>|<span data-ttu-id="65bff-156">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="65bff-156">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="65bff-157">status</span><span class="sxs-lookup"><span data-stu-id="65bff-157">status</span></span>|[<span data-ttu-id="65bff-158">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="65bff-158">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="65bff-p103">Status de conformidade do relatório de política. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="65bff-p103">Compliance status of the policy report. The possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="65bff-161">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="65bff-161">lastReportedDateTime</span></span>|<span data-ttu-id="65bff-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65bff-162">DateTimeOffset</span></span>|<span data-ttu-id="65bff-163">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="65bff-163">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="65bff-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="65bff-164">userPrincipalName</span></span>|<span data-ttu-id="65bff-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65bff-165">String</span></span>|<span data-ttu-id="65bff-166">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="65bff-166">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="65bff-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="65bff-167">Response</span></span>
<span data-ttu-id="65bff-168">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65bff-168">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65bff-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65bff-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="65bff-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65bff-170">Request</span></span>
<span data-ttu-id="65bff-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65bff-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
Content-type: application/json
Content-length: 552

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="65bff-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="65bff-172">Response</span></span>
<span data-ttu-id="65bff-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65bff-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 601

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "63a79499-9499-63a7-9994-a7639994a763",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```








