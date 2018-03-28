# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="f283e-101">Criar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="f283e-101">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="f283e-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f283e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f283e-103">Crie um novo objeto [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f283e-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f283e-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f283e-104">Prerequisites</span></span>
<span data-ttu-id="f283e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f283e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f283e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f283e-107">Permission type</span></span>|<span data-ttu-id="f283e-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f283e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f283e-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f283e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f283e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f283e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f283e-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f283e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f283e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f283e-112">Not supported.</span></span>|
|<span data-ttu-id="f283e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f283e-113">Application</span></span>|<span data-ttu-id="f283e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f283e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f283e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f283e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="f283e-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f283e-116">Request headers</span></span>
|<span data-ttu-id="f283e-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f283e-117">Header</span></span>|<span data-ttu-id="f283e-118">Valor</span><span class="sxs-lookup"><span data-stu-id="f283e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f283e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f283e-119">Authorization</span></span>|<span data-ttu-id="f283e-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f283e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f283e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f283e-121">Accept</span></span>|<span data-ttu-id="f283e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f283e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f283e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f283e-123">Request body</span></span>
<span data-ttu-id="f283e-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="f283e-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="f283e-125">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="f283e-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="f283e-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f283e-126">Property</span></span>|<span data-ttu-id="f283e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f283e-127">Type</span></span>|<span data-ttu-id="f283e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f283e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f283e-129">configuração</span><span class="sxs-lookup"><span data-stu-id="f283e-129">Setting</span></span>|<span data-ttu-id="f283e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f283e-130">String</span></span>|<span data-ttu-id="f283e-131">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="f283e-131">The setting class name and property name.</span></span>|
|<span data-ttu-id="f283e-132">settingName</span><span class="sxs-lookup"><span data-stu-id="f283e-132">settingName</span></span>|<span data-ttu-id="f283e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f283e-133">String</span></span>|<span data-ttu-id="f283e-134">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="f283e-134">Name of the setting.</span></span>|
|<span data-ttu-id="f283e-135">platformType</span><span class="sxs-lookup"><span data-stu-id="f283e-135">PlatformType</span></span>|<span data-ttu-id="f283e-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f283e-136">String</span></span>|<span data-ttu-id="f283e-137">Plataforma de configuração Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span><span class="sxs-lookup"><span data-stu-id="f283e-137">Setting platform Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="f283e-138">id</span><span class="sxs-lookup"><span data-stu-id="f283e-138">id</span></span>|<span data-ttu-id="f283e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f283e-139">String</span></span>|<span data-ttu-id="f283e-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f283e-140">Key of the setting.</span></span>|
|<span data-ttu-id="f283e-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f283e-141">unknownDeviceCount</span></span>|<span data-ttu-id="f283e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f283e-142">Int32</span></span>|<span data-ttu-id="f283e-143">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="f283e-143">Number of unknown devices</span></span>|
|<span data-ttu-id="f283e-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f283e-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="f283e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f283e-145">Int32</span></span>|<span data-ttu-id="f283e-146">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="f283e-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="f283e-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f283e-147">compliantDeviceCount</span></span>|<span data-ttu-id="f283e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f283e-148">Int32</span></span>|<span data-ttu-id="f283e-149">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="f283e-149">Number of compliant devices</span></span>|
|<span data-ttu-id="f283e-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f283e-150">remediatedDeviceCount</span></span>|<span data-ttu-id="f283e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f283e-151">Int32</span></span>|<span data-ttu-id="f283e-152">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="f283e-152">Number of remediated devices</span></span>|
|<span data-ttu-id="f283e-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f283e-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f283e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f283e-154">Int32</span></span>|<span data-ttu-id="f283e-155">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="f283e-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="f283e-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f283e-156">errorDeviceCount</span></span>|<span data-ttu-id="f283e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f283e-157">Int32</span></span>|<span data-ttu-id="f283e-158">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="f283e-158">Number of error devices</span></span>|
|<span data-ttu-id="f283e-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f283e-159">conflictDeviceCount</span></span>|<span data-ttu-id="f283e-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f283e-160">Int32</span></span>|<span data-ttu-id="f283e-161">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="f283e-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="f283e-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="f283e-162">Response</span></span>
<span data-ttu-id="f283e-163">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f283e-163">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f283e-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f283e-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="f283e-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f283e-165">Request</span></span>
<span data-ttu-id="f283e-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f283e-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f283e-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="f283e-167">Response</span></span>
<span data-ttu-id="f283e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f283e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



