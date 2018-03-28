# <a name="create-devicecompliancepolicystate"></a><span data-ttu-id="68c81-101">Criar deviceCompliancePolicyState</span><span class="sxs-lookup"><span data-stu-id="68c81-101">Create deviceCompliancePolicyState</span></span>

> <span data-ttu-id="68c81-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="68c81-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68c81-103">Criar um novo objeto [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).</span><span class="sxs-lookup"><span data-stu-id="68c81-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecompliancepolicystate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68c81-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="68c81-104">Prerequisites</span></span>
<span data-ttu-id="68c81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="68c81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="68c81-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68c81-107">Permission type</span></span>|<span data-ttu-id="68c81-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="68c81-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68c81-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68c81-109">Delegated (work or school account)</span></span>|<span data-ttu-id="68c81-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68c81-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="68c81-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68c81-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68c81-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68c81-112">Not supported.</span></span>|
|<span data-ttu-id="68c81-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68c81-113">Application</span></span>|<span data-ttu-id="68c81-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68c81-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68c81-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68c81-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /managedDevices/{managedDevicesId}/deviceCompliancePolicyStates
```

## <a name="request-headers"></a><span data-ttu-id="68c81-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68c81-116">Request headers</span></span>
|<span data-ttu-id="68c81-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68c81-117">Header</span></span>|<span data-ttu-id="68c81-118">Valor</span><span class="sxs-lookup"><span data-stu-id="68c81-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68c81-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="68c81-119">Authorization</span></span>|<span data-ttu-id="68c81-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68c81-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="68c81-121">Accept</span><span class="sxs-lookup"><span data-stu-id="68c81-121">Accept</span></span>|<span data-ttu-id="68c81-122">application/json</span><span class="sxs-lookup"><span data-stu-id="68c81-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68c81-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68c81-123">Request body</span></span>
<span data-ttu-id="68c81-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicyState.</span><span class="sxs-lookup"><span data-stu-id="68c81-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="68c81-125">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceCompliancePolicyState.</span><span class="sxs-lookup"><span data-stu-id="68c81-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="68c81-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68c81-126">Property</span></span>|<span data-ttu-id="68c81-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="68c81-127">Type</span></span>|<span data-ttu-id="68c81-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="68c81-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68c81-129">id</span><span class="sxs-lookup"><span data-stu-id="68c81-129">id</span></span>|<span data-ttu-id="68c81-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68c81-130">String</span></span>|<span data-ttu-id="68c81-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="68c81-131">Key of the setting.</span></span>|
|<span data-ttu-id="68c81-132">settingStates</span><span class="sxs-lookup"><span data-stu-id="68c81-132">settingStates</span></span>|<span data-ttu-id="68c81-133">Coleção [deviceCompliancePolicySettingState](../resources/intune_deviceconfig_devicecompliancepolicysettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="68c81-133">[deviceCompliancePolicySettingState](../resources/intune_deviceconfig_devicecompliancepolicysettingstate.md) collection</span></span>|<span data-ttu-id="68c81-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="68c81-134">Not yet documented</span></span>|
|<span data-ttu-id="68c81-135">displayName</span><span class="sxs-lookup"><span data-stu-id="68c81-135">displayName</span></span>|<span data-ttu-id="68c81-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68c81-136">String</span></span>|<span data-ttu-id="68c81-137">O nome da política dessa policyBase</span><span class="sxs-lookup"><span data-stu-id="68c81-137">The name of the policy for this policyBase</span></span>|
|<span data-ttu-id="68c81-138">version</span><span class="sxs-lookup"><span data-stu-id="68c81-138">version</span></span>|<span data-ttu-id="68c81-139">Int32</span><span class="sxs-lookup"><span data-stu-id="68c81-139">Int32</span></span>|<span data-ttu-id="68c81-140">A versão da política.</span><span class="sxs-lookup"><span data-stu-id="68c81-140">The version of the message.</span></span>|
|<span data-ttu-id="68c81-141">platformType</span><span class="sxs-lookup"><span data-stu-id="68c81-141">PlatformType</span></span>|<span data-ttu-id="68c81-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68c81-142">String</span></span>|<span data-ttu-id="68c81-143">Tipo de plataforma ao qual a política se aplica Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span><span class="sxs-lookup"><span data-stu-id="68c81-143">Platform type that the policy applies to Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="68c81-144">state</span><span class="sxs-lookup"><span data-stu-id="68c81-144">state</span></span>|<span data-ttu-id="68c81-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68c81-145">String</span></span>|<span data-ttu-id="68c81-146">O estado de conformidade da política Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="68c81-146">The compliance state of the policy Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="68c81-147">settingCount</span><span class="sxs-lookup"><span data-stu-id="68c81-147">settingCount</span></span>|<span data-ttu-id="68c81-148">Int32</span><span class="sxs-lookup"><span data-stu-id="68c81-148">Int32</span></span>|<span data-ttu-id="68c81-149">Contagem de quantas configurações uma política contém</span><span class="sxs-lookup"><span data-stu-id="68c81-149">Count of how many setting a policy holds</span></span>|



## <a name="response"></a><span data-ttu-id="68c81-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="68c81-150">Response</span></span>
<span data-ttu-id="68c81-151">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68c81-151">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_devicecompliancepolicystate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68c81-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68c81-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="68c81-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68c81-153">Request</span></span>
<span data-ttu-id="68c81-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68c81-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/managedDevices/{managedDevicesId}/deviceCompliancePolicyStates
Content-type: application/json
Content-length: 973

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "iOS",
  "state": "notApplicable",
  "settingCount": 12
}
```

### <a name="response"></a><span data-ttu-id="68c81-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="68c81-155">Response</span></span>
<span data-ttu-id="68c81-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68c81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1022

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
  "id": "2999e387-e387-2999-87e3-992987e39929",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "iOS",
  "state": "notApplicable",
  "settingCount": 12
}
```



