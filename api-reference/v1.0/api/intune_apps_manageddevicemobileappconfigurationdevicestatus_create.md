# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="93256-101">Criar managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="93256-101">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="93256-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="93256-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93256-103">Crie um novo objeto de [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="93256-103">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="93256-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="93256-104">Prerequisites</span></span>
<span data-ttu-id="93256-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="93256-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="93256-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93256-107">Permission type</span></span>|<span data-ttu-id="93256-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="93256-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93256-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93256-109">Delegated (work or school account)</span></span>|<span data-ttu-id="93256-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93256-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="93256-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93256-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93256-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93256-112">Not supported.</span></span>|
|<span data-ttu-id="93256-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93256-113">Application</span></span>|<span data-ttu-id="93256-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93256-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93256-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93256-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="93256-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93256-116">Request headers</span></span>
|<span data-ttu-id="93256-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93256-117">Header</span></span>|<span data-ttu-id="93256-118">Valor</span><span class="sxs-lookup"><span data-stu-id="93256-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93256-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="93256-119">Authorization</span></span>|<span data-ttu-id="93256-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93256-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93256-121">Accept</span><span class="sxs-lookup"><span data-stu-id="93256-121">Accept</span></span>|<span data-ttu-id="93256-122">application/json</span><span class="sxs-lookup"><span data-stu-id="93256-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93256-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93256-123">Request body</span></span>
<span data-ttu-id="93256-124">No corpo da solicitação, fornece uma representação JSON para o objeto managedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="93256-124">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="93256-125">A tabela a seguir mostra as propriedades que são necessárias quando você cria o managedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="93256-125">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="93256-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93256-126">Property</span></span>|<span data-ttu-id="93256-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="93256-127">Type</span></span>|<span data-ttu-id="93256-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="93256-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93256-129">id</span><span class="sxs-lookup"><span data-stu-id="93256-129">id</span></span>|<span data-ttu-id="93256-130">String</span><span class="sxs-lookup"><span data-stu-id="93256-130">String</span></span>|<span data-ttu-id="93256-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="93256-131">Key of the entity.</span></span>|
|<span data-ttu-id="93256-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="93256-132">deviceDisplayName</span></span>|<span data-ttu-id="93256-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93256-133">String</span></span>|<span data-ttu-id="93256-134">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="93256-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="93256-135">userName</span><span class="sxs-lookup"><span data-stu-id="93256-135">userName</span></span>|<span data-ttu-id="93256-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93256-136">String</span></span>|<span data-ttu-id="93256-137">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="93256-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="93256-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="93256-138">deviceModel</span></span>|<span data-ttu-id="93256-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93256-139">String</span></span>|<span data-ttu-id="93256-140">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="93256-140">The device model that is being reported</span></span>|
|<span data-ttu-id="93256-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="93256-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="93256-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93256-142">DateTimeOffset</span></span>|<span data-ttu-id="93256-143">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="93256-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="93256-144">status</span><span class="sxs-lookup"><span data-stu-id="93256-144">status</span></span>|[<span data-ttu-id="93256-145">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="93256-145">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="93256-146">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="93256-146">Compliance status of the policy report.</span></span> <span data-ttu-id="93256-147">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="93256-147">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="93256-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="93256-148">lastReportedDateTime</span></span>|<span data-ttu-id="93256-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93256-149">DateTimeOffset</span></span>|<span data-ttu-id="93256-150">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="93256-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="93256-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="93256-151">userPrincipalName</span></span>|<span data-ttu-id="93256-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93256-152">String</span></span>|<span data-ttu-id="93256-153">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="93256-153">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="93256-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="93256-154">Response</span></span>
<span data-ttu-id="93256-155">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93256-155">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93256-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93256-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="93256-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93256-157">Request</span></span>
<span data-ttu-id="93256-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93256-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="93256-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="93256-159">Response</span></span>
<span data-ttu-id="93256-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93256-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 494

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



