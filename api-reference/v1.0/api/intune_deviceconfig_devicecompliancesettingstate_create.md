# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="72aa4-101">Criar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="72aa4-101">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="72aa4-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="72aa4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72aa4-103">Criar um novo objeto [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="72aa4-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="72aa4-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72aa4-104">Prerequisites</span></span>
<span data-ttu-id="72aa4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="72aa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="72aa4-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72aa4-107">Permission type</span></span>|<span data-ttu-id="72aa4-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="72aa4-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72aa4-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72aa4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="72aa4-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72aa4-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72aa4-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72aa4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72aa4-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72aa4-112">Not supported.</span></span>|
|<span data-ttu-id="72aa4-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72aa4-113">Application</span></span>|<span data-ttu-id="72aa4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72aa4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72aa4-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72aa4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="72aa4-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72aa4-116">Request headers</span></span>
|<span data-ttu-id="72aa4-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72aa4-117">Header</span></span>|<span data-ttu-id="72aa4-118">Valor</span><span class="sxs-lookup"><span data-stu-id="72aa4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72aa4-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="72aa4-119">Authorization</span></span>|<span data-ttu-id="72aa4-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72aa4-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="72aa4-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="72aa4-121">Accept</span></span>|<span data-ttu-id="72aa4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="72aa4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72aa4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72aa4-123">Request body</span></span>
<span data-ttu-id="72aa4-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="72aa4-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="72aa4-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="72aa4-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="72aa4-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72aa4-126">Property</span></span>|<span data-ttu-id="72aa4-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="72aa4-127">Type</span></span>|<span data-ttu-id="72aa4-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="72aa4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72aa4-129">id</span><span class="sxs-lookup"><span data-stu-id="72aa4-129">id</span></span>|<span data-ttu-id="72aa4-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72aa4-130">String</span></span>|<span data-ttu-id="72aa4-131">Chave da entidade</span><span class="sxs-lookup"><span data-stu-id="72aa4-131">Key of the setting.</span></span>|
|<span data-ttu-id="72aa4-132">configuração</span><span class="sxs-lookup"><span data-stu-id="72aa4-132">Setting</span></span>|<span data-ttu-id="72aa4-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72aa4-133">String</span></span>|<span data-ttu-id="72aa4-134">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="72aa4-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="72aa4-135">settingName</span><span class="sxs-lookup"><span data-stu-id="72aa4-135">settingName</span></span>|<span data-ttu-id="72aa4-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72aa4-136">String</span></span>|<span data-ttu-id="72aa4-137">O Nome da configuração sendo relatada</span><span class="sxs-lookup"><span data-stu-id="72aa4-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="72aa4-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="72aa4-138">deviceId</span></span>|<span data-ttu-id="72aa4-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72aa4-139">String</span></span>|<span data-ttu-id="72aa4-140">A ID do dispositivo sendo relatada</span><span class="sxs-lookup"><span data-stu-id="72aa4-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="72aa4-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="72aa4-141">deviceName</span></span>|<span data-ttu-id="72aa4-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72aa4-142">String</span></span>|<span data-ttu-id="72aa4-143">O Nome do dispositivo sendo relatado</span><span class="sxs-lookup"><span data-stu-id="72aa4-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="72aa4-144">userId</span><span class="sxs-lookup"><span data-stu-id="72aa4-144">userId</span></span>|<span data-ttu-id="72aa4-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72aa4-145">String</span></span>|<span data-ttu-id="72aa4-146">A ID do usuário sendo relatada</span><span class="sxs-lookup"><span data-stu-id="72aa4-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="72aa4-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="72aa4-147">userEmail</span></span>|<span data-ttu-id="72aa4-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72aa4-148">String</span></span>|<span data-ttu-id="72aa4-149">O Endereço de email do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="72aa4-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="72aa4-150">userName</span><span class="sxs-lookup"><span data-stu-id="72aa4-150">UserName</span></span>|<span data-ttu-id="72aa4-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72aa4-151">String</span></span>|<span data-ttu-id="72aa4-152">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="72aa4-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="72aa4-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="72aa4-153">userPrincipalName</span></span>|<span data-ttu-id="72aa4-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72aa4-154">String</span></span>|<span data-ttu-id="72aa4-155">O PrincipalName do usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="72aa4-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="72aa4-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="72aa4-156">deviceModel</span></span>|<span data-ttu-id="72aa4-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72aa4-157">String</span></span>|<span data-ttu-id="72aa4-158">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="72aa4-158">The device model that is being reported</span></span>|
|<span data-ttu-id="72aa4-159">state</span><span class="sxs-lookup"><span data-stu-id="72aa4-159">state</span></span>|<span data-ttu-id="72aa4-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72aa4-160">String</span></span>|<span data-ttu-id="72aa4-161">O estado de conformidade da configuração Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="72aa4-161">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="72aa4-162">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="72aa4-162">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="72aa4-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72aa4-163">DateTimeOffset</span></span>|<span data-ttu-id="72aa4-164">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="72aa4-164">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="72aa4-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="72aa4-165">Response</span></span>
<span data-ttu-id="72aa4-166">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72aa4-166">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72aa4-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72aa4-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="72aa4-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72aa4-168">Request</span></span>
<span data-ttu-id="72aa4-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72aa4-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="72aa4-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="72aa4-170">Response</span></span>
<span data-ttu-id="72aa4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72aa4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



