# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="b2990-101">Criar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="b2990-101">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="b2990-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b2990-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2990-103">Criar um novo objeto [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="b2990-103">Create a new [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2990-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2990-104">Prerequisites</span></span>
<span data-ttu-id="b2990-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b2990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b2990-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2990-107">Permission type</span></span>|<span data-ttu-id="b2990-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2990-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2990-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2990-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b2990-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2990-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2990-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2990-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2990-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2990-112">Not supported.</span></span>|
|<span data-ttu-id="b2990-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2990-113">Application</span></span>|<span data-ttu-id="b2990-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2990-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2990-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2990-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="b2990-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2990-116">Request headers</span></span>
|<span data-ttu-id="b2990-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2990-117">Header</span></span>|<span data-ttu-id="b2990-118">Valor</span><span class="sxs-lookup"><span data-stu-id="b2990-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2990-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2990-119">Authorization</span></span>|<span data-ttu-id="b2990-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="b2990-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2990-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2990-121">Accept</span></span>|<span data-ttu-id="b2990-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b2990-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2990-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2990-123">Request body</span></span>
<span data-ttu-id="b2990-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="b2990-124">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="b2990-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="b2990-125">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="b2990-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2990-126">Property</span></span>|<span data-ttu-id="b2990-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2990-127">Type</span></span>|<span data-ttu-id="b2990-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2990-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2990-129">id</span><span class="sxs-lookup"><span data-stu-id="b2990-129">id</span></span>|<span data-ttu-id="b2990-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2990-130">String</span></span>|<span data-ttu-id="b2990-131">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="b2990-131">Key of the entity</span></span>|
|<span data-ttu-id="b2990-132">configuração</span><span class="sxs-lookup"><span data-stu-id="b2990-132">setting</span></span>|<span data-ttu-id="b2990-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2990-133">String</span></span>|<span data-ttu-id="b2990-134">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="b2990-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="b2990-135">settingName</span><span class="sxs-lookup"><span data-stu-id="b2990-135">settingName</span></span>|<span data-ttu-id="b2990-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2990-136">String</span></span>|<span data-ttu-id="b2990-137">O nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="b2990-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="b2990-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="b2990-138">deviceId</span></span>|<span data-ttu-id="b2990-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2990-139">String</span></span>|<span data-ttu-id="b2990-140">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="b2990-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="b2990-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="b2990-141">deviceName</span></span>|<span data-ttu-id="b2990-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2990-142">String</span></span>|<span data-ttu-id="b2990-143">O nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b2990-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="b2990-144">userId</span><span class="sxs-lookup"><span data-stu-id="b2990-144">userId</span></span>|<span data-ttu-id="b2990-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2990-145">String</span></span>|<span data-ttu-id="b2990-146">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="b2990-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="b2990-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="b2990-147">userEmail</span></span>|<span data-ttu-id="b2990-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2990-148">String</span></span>|<span data-ttu-id="b2990-149">O endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b2990-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="b2990-150">userName</span><span class="sxs-lookup"><span data-stu-id="b2990-150">userName</span></span>|<span data-ttu-id="b2990-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2990-151">String</span></span>|<span data-ttu-id="b2990-152">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b2990-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="b2990-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b2990-153">userPrincipalName</span></span>|<span data-ttu-id="b2990-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2990-154">String</span></span>|<span data-ttu-id="b2990-155">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b2990-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="b2990-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b2990-156">deviceModel</span></span>|<span data-ttu-id="b2990-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2990-157">String</span></span>|<span data-ttu-id="b2990-158">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b2990-158">The device model that is being reported</span></span>|
|<span data-ttu-id="b2990-159">state</span><span class="sxs-lookup"><span data-stu-id="b2990-159">state</span></span>|[<span data-ttu-id="b2990-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b2990-160">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="b2990-161">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="b2990-161">The compliance state of the setting Possible values are: , , , , , , .</span></span> <span data-ttu-id="b2990-162">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="b2990-162">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="b2990-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b2990-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b2990-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2990-164">DateTimeOffset</span></span>|<span data-ttu-id="b2990-165">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="b2990-165">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="b2990-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2990-166">Response</span></span>
<span data-ttu-id="b2990-167">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2990-167">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2990-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2990-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="b2990-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2990-169">Request</span></span>
<span data-ttu-id="b2990-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2990-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
Content-type: application/json
Content-length: 517

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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

### <a name="response"></a><span data-ttu-id="b2990-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2990-171">Response</span></span>
<span data-ttu-id="b2990-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2990-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



