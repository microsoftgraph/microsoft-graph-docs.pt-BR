# <a name="update-deviceconfigurationstate"></a><span data-ttu-id="57a39-101">Atualizar deviceConfigurationState</span><span class="sxs-lookup"><span data-stu-id="57a39-101">Update deviceConfigurationState</span></span>

> <span data-ttu-id="57a39-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="57a39-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57a39-103">Atualizar as propriedades de um objeto [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md).</span><span class="sxs-lookup"><span data-stu-id="57a39-103">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57a39-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57a39-104">Prerequisites</span></span>
<span data-ttu-id="57a39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="57a39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="57a39-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57a39-107">Permission type</span></span>|<span data-ttu-id="57a39-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57a39-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57a39-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57a39-109">Delegated (work or school account)</span></span>|<span data-ttu-id="57a39-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57a39-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57a39-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57a39-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57a39-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57a39-112">Not supported.</span></span>|
|<span data-ttu-id="57a39-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57a39-113">Application</span></span>|<span data-ttu-id="57a39-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57a39-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57a39-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57a39-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /managedDevices/{managedDevicesId}/deviceConfigurationStates/{deviceConfigurationStateId}
```

## <a name="request-headers"></a><span data-ttu-id="57a39-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57a39-116">Request headers</span></span>
|<span data-ttu-id="57a39-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57a39-117">Header</span></span>|<span data-ttu-id="57a39-118">Valor</span><span class="sxs-lookup"><span data-stu-id="57a39-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57a39-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="57a39-119">Authorization</span></span>|<span data-ttu-id="57a39-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57a39-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="57a39-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57a39-121">Accept</span></span>|<span data-ttu-id="57a39-122">application/json</span><span class="sxs-lookup"><span data-stu-id="57a39-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57a39-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57a39-123">Request body</span></span>
<span data-ttu-id="57a39-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md).</span><span class="sxs-lookup"><span data-stu-id="57a39-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_deviceconfigurationstate.md) object.</span></span>

<span data-ttu-id="57a39-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md).</span><span class="sxs-lookup"><span data-stu-id="57a39-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="57a39-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57a39-126">Property</span></span>|<span data-ttu-id="57a39-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="57a39-127">Type</span></span>|<span data-ttu-id="57a39-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="57a39-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57a39-129">id</span><span class="sxs-lookup"><span data-stu-id="57a39-129">id</span></span>|<span data-ttu-id="57a39-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a39-130">String</span></span>|<span data-ttu-id="57a39-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="57a39-131">Key of the setting.</span></span>|
|<span data-ttu-id="57a39-132">settingStates</span><span class="sxs-lookup"><span data-stu-id="57a39-132">settingStates</span></span>|<span data-ttu-id="57a39-133">Coleção [deviceConfigurationSettingState](../resources/intune_deviceconfig_deviceconfigurationsettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="57a39-133">[deviceConfigurationSettingState](../resources/intune_deviceconfig_deviceconfigurationsettingstate.md) collection</span></span>|<span data-ttu-id="57a39-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="57a39-134">Not yet documented</span></span>|
|<span data-ttu-id="57a39-135">displayName</span><span class="sxs-lookup"><span data-stu-id="57a39-135">displayName</span></span>|<span data-ttu-id="57a39-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a39-136">String</span></span>|<span data-ttu-id="57a39-137">O nome da política dessa policyBase</span><span class="sxs-lookup"><span data-stu-id="57a39-137">The name of the policy for this policyBase</span></span>|
|<span data-ttu-id="57a39-138">version</span><span class="sxs-lookup"><span data-stu-id="57a39-138">version</span></span>|<span data-ttu-id="57a39-139">Int32</span><span class="sxs-lookup"><span data-stu-id="57a39-139">Int32</span></span>|<span data-ttu-id="57a39-140">A versão da política</span><span class="sxs-lookup"><span data-stu-id="57a39-140">The version of the message.</span></span>|
|<span data-ttu-id="57a39-141">platformType</span><span class="sxs-lookup"><span data-stu-id="57a39-141">PlatformType</span></span>|<span data-ttu-id="57a39-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a39-142">String</span></span>|<span data-ttu-id="57a39-143">Tipo de plataforma ao qual a política se aplica Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span><span class="sxs-lookup"><span data-stu-id="57a39-143">Platform type that the policy applies to Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="57a39-144">state</span><span class="sxs-lookup"><span data-stu-id="57a39-144">state</span></span>|<span data-ttu-id="57a39-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a39-145">String</span></span>|<span data-ttu-id="57a39-146">O estado de conformidade da política Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="57a39-146">The compliance state of the policy Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="57a39-147">settingCount</span><span class="sxs-lookup"><span data-stu-id="57a39-147">settingCount</span></span>|<span data-ttu-id="57a39-148">Int32</span><span class="sxs-lookup"><span data-stu-id="57a39-148">Int32</span></span>|<span data-ttu-id="57a39-149">Contagem de quantas configurações uma política contém</span><span class="sxs-lookup"><span data-stu-id="57a39-149">Count of how many setting a policy holds</span></span>|



## <a name="response"></a><span data-ttu-id="57a39-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="57a39-150">Response</span></span>
<span data-ttu-id="57a39-151">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57a39-151">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_deviceconfigurationstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57a39-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57a39-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="57a39-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57a39-153">Request</span></span>
<span data-ttu-id="57a39-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57a39-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/managedDevices/{managedDevicesId}/deviceConfigurationStates/{deviceConfigurationStateId}
Content-type: application/json
Content-length: 904

{
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
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

### <a name="response"></a><span data-ttu-id="57a39-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="57a39-155">Response</span></span>
<span data-ttu-id="57a39-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57a39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1016

{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "id": "11692784-2784-1169-8427-691184276911",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
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



