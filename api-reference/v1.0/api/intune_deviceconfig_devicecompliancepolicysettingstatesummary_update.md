# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="dd7f3-101">Atualizar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="dd7f3-101">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="dd7f3-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dd7f3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd7f3-103">Atualizar as propriedades de um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="dd7f3-103">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd7f3-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dd7f3-104">Prerequisites</span></span>
<span data-ttu-id="dd7f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dd7f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dd7f3-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd7f3-107">Permission type</span></span>|<span data-ttu-id="dd7f3-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dd7f3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd7f3-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd7f3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dd7f3-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd7f3-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd7f3-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd7f3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd7f3-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd7f3-112">Not supported.</span></span>|
|<span data-ttu-id="dd7f3-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd7f3-113">Application</span></span>|<span data-ttu-id="dd7f3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd7f3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd7f3-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd7f3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="dd7f3-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd7f3-116">Request headers</span></span>
|<span data-ttu-id="dd7f3-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd7f3-117">Header</span></span>|<span data-ttu-id="dd7f3-118">Valor</span><span class="sxs-lookup"><span data-stu-id="dd7f3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd7f3-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd7f3-119">Authorization</span></span>|<span data-ttu-id="dd7f3-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="dd7f3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd7f3-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dd7f3-121">Accept</span></span>|<span data-ttu-id="dd7f3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="dd7f3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd7f3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd7f3-123">Request body</span></span>
<span data-ttu-id="dd7f3-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="dd7f3-124">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="dd7f3-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="dd7f3-125">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="dd7f3-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd7f3-126">Property</span></span>|<span data-ttu-id="dd7f3-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd7f3-127">Type</span></span>|<span data-ttu-id="dd7f3-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd7f3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd7f3-129">id</span><span class="sxs-lookup"><span data-stu-id="dd7f3-129">id</span></span>|<span data-ttu-id="dd7f3-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd7f3-130">String</span></span>|<span data-ttu-id="dd7f3-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dd7f3-131">Key of the entity.</span></span>|
|<span data-ttu-id="dd7f3-132">configuração</span><span class="sxs-lookup"><span data-stu-id="dd7f3-132">setting</span></span>|<span data-ttu-id="dd7f3-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd7f3-133">String</span></span>|<span data-ttu-id="dd7f3-134">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="dd7f3-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="dd7f3-135">settingName</span><span class="sxs-lookup"><span data-stu-id="dd7f3-135">settingName</span></span>|<span data-ttu-id="dd7f3-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd7f3-136">String</span></span>|<span data-ttu-id="dd7f3-137">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="dd7f3-137">Name of the setting.</span></span>|
|<span data-ttu-id="dd7f3-138">platformType</span><span class="sxs-lookup"><span data-stu-id="dd7f3-138">platformType</span></span>|[<span data-ttu-id="dd7f3-139">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="dd7f3-139">policyPlatformType</span></span>](../resources/intune_deviceconfig_policyplatformtype.md)|<span data-ttu-id="dd7f3-140">Plataforma de configuração.</span><span class="sxs-lookup"><span data-stu-id="dd7f3-140">Setting platform.</span></span> <span data-ttu-id="dd7f3-141">Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="dd7f3-141">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="dd7f3-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd7f3-142">unknownDeviceCount</span></span>|<span data-ttu-id="dd7f3-143">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7f3-143">Int32</span></span>|<span data-ttu-id="dd7f3-144">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="dd7f3-144">Number of unknown devices</span></span>|
|<span data-ttu-id="dd7f3-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd7f3-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="dd7f3-146">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7f3-146">Int32</span></span>|<span data-ttu-id="dd7f3-147">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="dd7f3-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="dd7f3-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd7f3-148">compliantDeviceCount</span></span>|<span data-ttu-id="dd7f3-149">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7f3-149">Int32</span></span>|<span data-ttu-id="dd7f3-150">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="dd7f3-150">Number of compliant devices</span></span>|
|<span data-ttu-id="dd7f3-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd7f3-151">remediatedDeviceCount</span></span>|<span data-ttu-id="dd7f3-152">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7f3-152">Int32</span></span>|<span data-ttu-id="dd7f3-153">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="dd7f3-153">Number of remediated devices</span></span>|
|<span data-ttu-id="dd7f3-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd7f3-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="dd7f3-155">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7f3-155">Int32</span></span>|<span data-ttu-id="dd7f3-156">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="dd7f3-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="dd7f3-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd7f3-157">errorDeviceCount</span></span>|<span data-ttu-id="dd7f3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7f3-158">Int32</span></span>|<span data-ttu-id="dd7f3-159">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="dd7f3-159">Number of error devices</span></span>|
|<span data-ttu-id="dd7f3-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dd7f3-160">conflictDeviceCount</span></span>|<span data-ttu-id="dd7f3-161">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7f3-161">Int32</span></span>|<span data-ttu-id="dd7f3-162">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="dd7f3-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="dd7f3-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd7f3-163">Response</span></span>
<span data-ttu-id="dd7f3-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd7f3-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd7f3-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd7f3-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd7f3-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd7f3-166">Request</span></span>
<span data-ttu-id="dd7f3-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd7f3-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 311

{
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

### <a name="response"></a><span data-ttu-id="dd7f3-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd7f3-168">Response</span></span>
<span data-ttu-id="dd7f3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd7f3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








