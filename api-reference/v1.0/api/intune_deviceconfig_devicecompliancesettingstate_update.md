# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="cbf3d-101">Atualizar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="cbf3d-101">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="cbf3d-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cbf3d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cbf3d-103">Atualizar as propriedades de um objeto [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) objeto.</span><span class="sxs-lookup"><span data-stu-id="cbf3d-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cbf3d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cbf3d-104">Prerequisites</span></span>
<span data-ttu-id="cbf3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cbf3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cbf3d-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbf3d-107">Permission type</span></span>|<span data-ttu-id="cbf3d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cbf3d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbf3d-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbf3d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cbf3d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbf3d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cbf3d-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbf3d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbf3d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbf3d-112">Not supported.</span></span>|
|<span data-ttu-id="cbf3d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbf3d-113">Application</span></span>|<span data-ttu-id="cbf3d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbf3d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbf3d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbf3d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="cbf3d-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbf3d-116">Request headers</span></span>
|<span data-ttu-id="cbf3d-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cbf3d-117">Header</span></span>|<span data-ttu-id="cbf3d-118">Valor</span><span class="sxs-lookup"><span data-stu-id="cbf3d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbf3d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbf3d-119">Authorization</span></span>|<span data-ttu-id="cbf3d-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbf3d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cbf3d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="cbf3d-121">Accept</span></span>|<span data-ttu-id="cbf3d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cbf3d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbf3d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbf3d-123">Request body</span></span>
<span data-ttu-id="cbf3d-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="cbf3d-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="cbf3d-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="cbf3d-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="cbf3d-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbf3d-126">Property</span></span>|<span data-ttu-id="cbf3d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbf3d-127">Type</span></span>|<span data-ttu-id="cbf3d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbf3d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbf3d-129">id</span><span class="sxs-lookup"><span data-stu-id="cbf3d-129">id</span></span>|<span data-ttu-id="cbf3d-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbf3d-130">String</span></span>|<span data-ttu-id="cbf3d-131">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="cbf3d-131">Key of the setting.</span></span>|
|<span data-ttu-id="cbf3d-132">configuração</span><span class="sxs-lookup"><span data-stu-id="cbf3d-132">Setting</span></span>|<span data-ttu-id="cbf3d-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbf3d-133">String</span></span>|<span data-ttu-id="cbf3d-134">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="cbf3d-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="cbf3d-135">settingName</span><span class="sxs-lookup"><span data-stu-id="cbf3d-135">settingName</span></span>|<span data-ttu-id="cbf3d-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbf3d-136">String</span></span>|<span data-ttu-id="cbf3d-137">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="cbf3d-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="cbf3d-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="cbf3d-138">deviceId</span></span>|<span data-ttu-id="cbf3d-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbf3d-139">String</span></span>|<span data-ttu-id="cbf3d-140">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="cbf3d-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="cbf3d-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="cbf3d-141">deviceName</span></span>|<span data-ttu-id="cbf3d-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbf3d-142">String</span></span>|<span data-ttu-id="cbf3d-143">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="cbf3d-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="cbf3d-144">userId</span><span class="sxs-lookup"><span data-stu-id="cbf3d-144">userId</span></span>|<span data-ttu-id="cbf3d-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbf3d-145">String</span></span>|<span data-ttu-id="cbf3d-146">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="cbf3d-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="cbf3d-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="cbf3d-147">userEmail</span></span>|<span data-ttu-id="cbf3d-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbf3d-148">String</span></span>|<span data-ttu-id="cbf3d-149">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="cbf3d-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="cbf3d-150">userName</span><span class="sxs-lookup"><span data-stu-id="cbf3d-150">UserName</span></span>|<span data-ttu-id="cbf3d-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbf3d-151">String</span></span>|<span data-ttu-id="cbf3d-152">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="cbf3d-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="cbf3d-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cbf3d-153">userPrincipalName</span></span>|<span data-ttu-id="cbf3d-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbf3d-154">String</span></span>|<span data-ttu-id="cbf3d-155">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="cbf3d-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="cbf3d-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="cbf3d-156">deviceModel</span></span>|<span data-ttu-id="cbf3d-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbf3d-157">String</span></span>|<span data-ttu-id="cbf3d-158">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="cbf3d-158">The device model that is being reported</span></span>|
|<span data-ttu-id="cbf3d-159">state</span><span class="sxs-lookup"><span data-stu-id="cbf3d-159">state</span></span>|<span data-ttu-id="cbf3d-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbf3d-160">String</span></span>|<span data-ttu-id="cbf3d-161">O estado de conformidade da configuração Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="cbf3d-161">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="cbf3d-162">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cbf3d-162">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="cbf3d-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbf3d-163">DateTimeOffset</span></span>|<span data-ttu-id="cbf3d-164">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="cbf3d-164">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="cbf3d-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbf3d-165">Response</span></span>
<span data-ttu-id="cbf3d-166">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbf3d-166">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbf3d-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbf3d-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="cbf3d-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbf3d-168">Request</span></span>
<span data-ttu-id="cbf3d-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbf3d-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
Content-type: application/json
Content-length: 450

{
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```

### <a name="response"></a><span data-ttu-id="cbf3d-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbf3d-170">Response</span></span>
<span data-ttu-id="cbf3d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbf3d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```



