# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="bb9a5-101">Atualizar settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="bb9a5-101">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="bb9a5-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bb9a5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb9a5-103">Atualizar as propriedades de um objeto [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="bb9a5-103">Update the properties of a [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bb9a5-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb9a5-104">Prerequisites</span></span>
<span data-ttu-id="bb9a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb9a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bb9a5-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb9a5-107">Permission type</span></span>|<span data-ttu-id="bb9a5-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb9a5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb9a5-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb9a5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bb9a5-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb9a5-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb9a5-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb9a5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb9a5-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb9a5-112">Not supported.</span></span>|
|<span data-ttu-id="bb9a5-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb9a5-113">Application</span></span>|<span data-ttu-id="bb9a5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb9a5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb9a5-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb9a5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="bb9a5-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb9a5-116">Request headers</span></span>
|<span data-ttu-id="bb9a5-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb9a5-117">Header</span></span>|<span data-ttu-id="bb9a5-118">Valor</span><span class="sxs-lookup"><span data-stu-id="bb9a5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb9a5-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb9a5-119">Authorization</span></span>|<span data-ttu-id="bb9a5-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb9a5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb9a5-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb9a5-121">Accept</span></span>|<span data-ttu-id="bb9a5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bb9a5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb9a5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb9a5-123">Request body</span></span>
<span data-ttu-id="bb9a5-124">No corpo da solicitação, forneça uma representação JSON do objeto [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="bb9a5-124">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="bb9a5-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="bb9a5-125">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="bb9a5-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb9a5-126">Property</span></span>|<span data-ttu-id="bb9a5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb9a5-127">Type</span></span>|<span data-ttu-id="bb9a5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb9a5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb9a5-129">id</span><span class="sxs-lookup"><span data-stu-id="bb9a5-129">id</span></span>|<span data-ttu-id="bb9a5-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb9a5-130">String</span></span>|<span data-ttu-id="bb9a5-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bb9a5-131">Key of the entity.</span></span>|
|<span data-ttu-id="bb9a5-132">settingName</span><span class="sxs-lookup"><span data-stu-id="bb9a5-132">settingName</span></span>|<span data-ttu-id="bb9a5-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb9a5-133">String</span></span>|<span data-ttu-id="bb9a5-134">Nome da configuração</span><span class="sxs-lookup"><span data-stu-id="bb9a5-134">Name of the setting</span></span>|
|<span data-ttu-id="bb9a5-135">instancePath</span><span class="sxs-lookup"><span data-stu-id="bb9a5-135">instancePath</span></span>|<span data-ttu-id="bb9a5-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb9a5-136">String</span></span>|<span data-ttu-id="bb9a5-137">Nome de InstancePath para a configuração</span><span class="sxs-lookup"><span data-stu-id="bb9a5-137">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="bb9a5-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb9a5-138">unknownDeviceCount</span></span>|<span data-ttu-id="bb9a5-139">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9a5-139">Int32</span></span>|<span data-ttu-id="bb9a5-140">Contagem desconhecida de dispositivos para a configuração</span><span class="sxs-lookup"><span data-stu-id="bb9a5-140">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="bb9a5-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb9a5-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="bb9a5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9a5-142">Int32</span></span>|<span data-ttu-id="bb9a5-143">Contagem não aplicável ao dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="bb9a5-143">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="bb9a5-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb9a5-144">compliantDeviceCount</span></span>|<span data-ttu-id="bb9a5-145">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9a5-145">Int32</span></span>|<span data-ttu-id="bb9a5-146">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="bb9a5-146">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="bb9a5-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb9a5-147">remediatedDeviceCount</span></span>|<span data-ttu-id="bb9a5-148">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9a5-148">Int32</span></span>|<span data-ttu-id="bb9a5-149">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="bb9a5-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="bb9a5-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb9a5-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="bb9a5-151">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9a5-151">Int32</span></span>|<span data-ttu-id="bb9a5-152">Contagem de dispositivo sem conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="bb9a5-152">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="bb9a5-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb9a5-153">errorDeviceCount</span></span>|<span data-ttu-id="bb9a5-154">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9a5-154">Int32</span></span>|<span data-ttu-id="bb9a5-155">Contagem de erros de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="bb9a5-155">Device error count for the setting</span></span>|
|<span data-ttu-id="bb9a5-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb9a5-156">conflictDeviceCount</span></span>|<span data-ttu-id="bb9a5-157">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9a5-157">Int32</span></span>|<span data-ttu-id="bb9a5-158">Contagem de erro de conflito de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="bb9a5-158">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="bb9a5-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb9a5-159">Response</span></span>
<span data-ttu-id="bb9a5-160">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb9a5-160">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb9a5-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb9a5-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb9a5-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb9a5-162">Request</span></span>
<span data-ttu-id="bb9a5-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb9a5-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="bb9a5-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb9a5-164">Response</span></span>
<span data-ttu-id="bb9a5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb9a5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



