# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="f7d24-101">Atualizar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="f7d24-101">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="f7d24-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f7d24-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7d24-103">Atualizar as propriedades de um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f7d24-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f7d24-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7d24-104">Prerequisites</span></span>
<span data-ttu-id="f7d24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f7d24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f7d24-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7d24-107">Permission type</span></span>|<span data-ttu-id="f7d24-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f7d24-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7d24-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7d24-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f7d24-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7d24-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f7d24-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7d24-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7d24-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7d24-112">Not supported.</span></span>|
|<span data-ttu-id="f7d24-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7d24-113">Application</span></span>|<span data-ttu-id="f7d24-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7d24-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7d24-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7d24-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="f7d24-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7d24-116">Request headers</span></span>
|<span data-ttu-id="f7d24-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7d24-117">Header</span></span>|<span data-ttu-id="f7d24-118">Valor</span><span class="sxs-lookup"><span data-stu-id="f7d24-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7d24-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7d24-119">Authorization</span></span>|<span data-ttu-id="f7d24-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7d24-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f7d24-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f7d24-121">Accept</span></span>|<span data-ttu-id="f7d24-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f7d24-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7d24-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7d24-123">Request body</span></span>
<span data-ttu-id="f7d24-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f7d24-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="f7d24-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f7d24-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="f7d24-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7d24-126">Property</span></span>|<span data-ttu-id="f7d24-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7d24-127">Type</span></span>|<span data-ttu-id="f7d24-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7d24-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7d24-129">configuração</span><span class="sxs-lookup"><span data-stu-id="f7d24-129">Setting</span></span>|<span data-ttu-id="f7d24-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7d24-130">String</span></span>|<span data-ttu-id="f7d24-131">O nome da classe de configuração e o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="f7d24-131">The setting class name and property name.</span></span>|
|<span data-ttu-id="f7d24-132">settingName</span><span class="sxs-lookup"><span data-stu-id="f7d24-132">settingName</span></span>|<span data-ttu-id="f7d24-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7d24-133">String</span></span>|<span data-ttu-id="f7d24-134">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="f7d24-134">Name of the setting.</span></span>|
|<span data-ttu-id="f7d24-135">platformType</span><span class="sxs-lookup"><span data-stu-id="f7d24-135">PlatformType</span></span>|<span data-ttu-id="f7d24-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7d24-136">String</span></span>|<span data-ttu-id="f7d24-137">Plataforma de configuração Os valores possíveis são: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span><span class="sxs-lookup"><span data-stu-id="f7d24-137">Setting platform Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="f7d24-138">id</span><span class="sxs-lookup"><span data-stu-id="f7d24-138">id</span></span>|<span data-ttu-id="f7d24-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7d24-139">String</span></span>|<span data-ttu-id="f7d24-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f7d24-140">Key of the setting.</span></span>|
|<span data-ttu-id="f7d24-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7d24-141">unknownDeviceCount</span></span>|<span data-ttu-id="f7d24-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f7d24-142">Int32</span></span>|<span data-ttu-id="f7d24-143">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="f7d24-143">Number of unknown devices</span></span>|
|<span data-ttu-id="f7d24-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7d24-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="f7d24-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f7d24-145">Int32</span></span>|<span data-ttu-id="f7d24-146">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="f7d24-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="f7d24-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7d24-147">compliantDeviceCount</span></span>|<span data-ttu-id="f7d24-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f7d24-148">Int32</span></span>|<span data-ttu-id="f7d24-149">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="f7d24-149">Number of compliant devices</span></span>|
|<span data-ttu-id="f7d24-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7d24-150">remediatedDeviceCount</span></span>|<span data-ttu-id="f7d24-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f7d24-151">Int32</span></span>|<span data-ttu-id="f7d24-152">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="f7d24-152">Number of remediated devices</span></span>|
|<span data-ttu-id="f7d24-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7d24-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f7d24-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f7d24-154">Int32</span></span>|<span data-ttu-id="f7d24-155">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="f7d24-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="f7d24-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7d24-156">errorDeviceCount</span></span>|<span data-ttu-id="f7d24-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f7d24-157">Int32</span></span>|<span data-ttu-id="f7d24-158">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="f7d24-158">Number of error devices</span></span>|
|<span data-ttu-id="f7d24-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f7d24-159">conflictDeviceCount</span></span>|<span data-ttu-id="f7d24-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f7d24-160">Int32</span></span>|<span data-ttu-id="f7d24-161">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="f7d24-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="f7d24-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7d24-162">Response</span></span>
<span data-ttu-id="f7d24-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7d24-163">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7d24-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7d24-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="f7d24-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7d24-165">Request</span></span>
<span data-ttu-id="f7d24-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7d24-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7d24-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7d24-167">Response</span></span>
<span data-ttu-id="f7d24-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7d24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



