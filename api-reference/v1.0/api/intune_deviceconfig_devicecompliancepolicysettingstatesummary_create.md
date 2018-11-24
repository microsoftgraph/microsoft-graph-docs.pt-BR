# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="16e95-101">Criar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="16e95-101">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="16e95-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="16e95-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16e95-103">Crie um novo objeto [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="16e95-103">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16e95-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16e95-104">Prerequisites</span></span>
<span data-ttu-id="16e95-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="16e95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="16e95-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16e95-107">Permission type</span></span>|<span data-ttu-id="16e95-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16e95-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16e95-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16e95-109">Delegated (work or school account)</span></span>|<span data-ttu-id="16e95-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16e95-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16e95-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16e95-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16e95-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16e95-112">Not supported.</span></span>|
|<span data-ttu-id="16e95-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16e95-113">Application</span></span>|<span data-ttu-id="16e95-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16e95-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16e95-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16e95-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="16e95-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16e95-116">Request headers</span></span>
|<span data-ttu-id="16e95-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16e95-117">Header</span></span>|<span data-ttu-id="16e95-118">Valor</span><span class="sxs-lookup"><span data-stu-id="16e95-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16e95-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="16e95-119">Authorization</span></span>|<span data-ttu-id="16e95-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16e95-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16e95-121">Accept</span><span class="sxs-lookup"><span data-stu-id="16e95-121">Accept</span></span>|<span data-ttu-id="16e95-122">application/json</span><span class="sxs-lookup"><span data-stu-id="16e95-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16e95-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16e95-123">Request body</span></span>
<span data-ttu-id="16e95-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="16e95-124">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="16e95-125">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="16e95-125">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="16e95-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16e95-126">Property</span></span>|<span data-ttu-id="16e95-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="16e95-127">Type</span></span>|<span data-ttu-id="16e95-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="16e95-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16e95-129">id</span><span class="sxs-lookup"><span data-stu-id="16e95-129">id</span></span>|<span data-ttu-id="16e95-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16e95-130">String</span></span>|<span data-ttu-id="16e95-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="16e95-131">Key of the entity.</span></span>|
|<span data-ttu-id="16e95-132">configuração</span><span class="sxs-lookup"><span data-stu-id="16e95-132">setting</span></span>|<span data-ttu-id="16e95-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16e95-133">String</span></span>|<span data-ttu-id="16e95-134">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="16e95-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="16e95-135">settingName</span><span class="sxs-lookup"><span data-stu-id="16e95-135">settingName</span></span>|<span data-ttu-id="16e95-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16e95-136">String</span></span>|<span data-ttu-id="16e95-137">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="16e95-137">Name of the setting.</span></span>|
|<span data-ttu-id="16e95-138">platformType</span><span class="sxs-lookup"><span data-stu-id="16e95-138">platformType</span></span>|[<span data-ttu-id="16e95-139">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="16e95-139">policyPlatformType</span></span>](../resources/intune_deviceconfig_policyplatformtype.md)|<span data-ttu-id="16e95-140">Plataforma de configuração.</span><span class="sxs-lookup"><span data-stu-id="16e95-140">Setting platform.</span></span> <span data-ttu-id="16e95-141">Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="16e95-141">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="16e95-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16e95-142">unknownDeviceCount</span></span>|<span data-ttu-id="16e95-143">Int32</span><span class="sxs-lookup"><span data-stu-id="16e95-143">Int32</span></span>|<span data-ttu-id="16e95-144">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="16e95-144">Number of unknown devices</span></span>|
|<span data-ttu-id="16e95-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16e95-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="16e95-146">Int32</span><span class="sxs-lookup"><span data-stu-id="16e95-146">Int32</span></span>|<span data-ttu-id="16e95-147">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="16e95-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="16e95-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16e95-148">compliantDeviceCount</span></span>|<span data-ttu-id="16e95-149">Int32</span><span class="sxs-lookup"><span data-stu-id="16e95-149">Int32</span></span>|<span data-ttu-id="16e95-150">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="16e95-150">Number of compliant devices</span></span>|
|<span data-ttu-id="16e95-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16e95-151">remediatedDeviceCount</span></span>|<span data-ttu-id="16e95-152">Int32</span><span class="sxs-lookup"><span data-stu-id="16e95-152">Int32</span></span>|<span data-ttu-id="16e95-153">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="16e95-153">Number of remediated devices</span></span>|
|<span data-ttu-id="16e95-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16e95-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="16e95-155">Int32</span><span class="sxs-lookup"><span data-stu-id="16e95-155">Int32</span></span>|<span data-ttu-id="16e95-156">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="16e95-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="16e95-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16e95-157">errorDeviceCount</span></span>|<span data-ttu-id="16e95-158">Int32</span><span class="sxs-lookup"><span data-stu-id="16e95-158">Int32</span></span>|<span data-ttu-id="16e95-159">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="16e95-159">Number of error devices</span></span>|
|<span data-ttu-id="16e95-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16e95-160">conflictDeviceCount</span></span>|<span data-ttu-id="16e95-161">Int32</span><span class="sxs-lookup"><span data-stu-id="16e95-161">Int32</span></span>|<span data-ttu-id="16e95-162">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="16e95-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="16e95-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="16e95-163">Response</span></span>
<span data-ttu-id="16e95-164">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16e95-164">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16e95-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16e95-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="16e95-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16e95-166">Request</span></span>
<span data-ttu-id="16e95-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16e95-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="16e95-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="16e95-168">Response</span></span>
<span data-ttu-id="16e95-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16e95-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



