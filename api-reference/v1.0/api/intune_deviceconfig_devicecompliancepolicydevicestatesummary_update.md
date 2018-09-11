# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="37a1c-101">Atualizar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="37a1c-101">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="37a1c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="37a1c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37a1c-103">Atualizar as propriedades de um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="37a1c-103">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="37a1c-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37a1c-104">Prerequisites</span></span>
<span data-ttu-id="37a1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="37a1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="37a1c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37a1c-107">Permission type</span></span>|<span data-ttu-id="37a1c-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37a1c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37a1c-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37a1c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="37a1c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37a1c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37a1c-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37a1c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37a1c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37a1c-112">Not supported.</span></span>|
|<span data-ttu-id="37a1c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37a1c-113">Application</span></span>|<span data-ttu-id="37a1c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37a1c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37a1c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37a1c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="37a1c-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37a1c-116">Request headers</span></span>
|<span data-ttu-id="37a1c-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37a1c-117">Header</span></span>|<span data-ttu-id="37a1c-118">Valor</span><span class="sxs-lookup"><span data-stu-id="37a1c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37a1c-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="37a1c-119">Authorization</span></span>|<span data-ttu-id="37a1c-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="37a1c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37a1c-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37a1c-121">Accept</span></span>|<span data-ttu-id="37a1c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="37a1c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37a1c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37a1c-123">Request body</span></span>
<span data-ttu-id="37a1c-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="37a1c-124">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="37a1c-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="37a1c-125">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="37a1c-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37a1c-126">Property</span></span>|<span data-ttu-id="37a1c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="37a1c-127">Type</span></span>|<span data-ttu-id="37a1c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="37a1c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37a1c-129">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="37a1c-129">inGracePeriodCount</span></span>|<span data-ttu-id="37a1c-130">Int32</span><span class="sxs-lookup"><span data-stu-id="37a1c-130">Int32</span></span>|<span data-ttu-id="37a1c-131">Quantidade de dispositivos que estão no período de cortesia</span><span class="sxs-lookup"><span data-stu-id="37a1c-131">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="37a1c-132">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="37a1c-132">configManagerCount</span></span>|<span data-ttu-id="37a1c-133">Int32</span><span class="sxs-lookup"><span data-stu-id="37a1c-133">Int32</span></span>|<span data-ttu-id="37a1c-134">Quantidade de dispositivos que estão em conformidade gerenciada pelo System Center Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="37a1c-134">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="37a1c-135">id</span><span class="sxs-lookup"><span data-stu-id="37a1c-135">id</span></span>|<span data-ttu-id="37a1c-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37a1c-136">String</span></span>|<span data-ttu-id="37a1c-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="37a1c-137">Key of the entity.</span></span>|
|<span data-ttu-id="37a1c-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37a1c-138">unknownDeviceCount</span></span>|<span data-ttu-id="37a1c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="37a1c-139">Int32</span></span>|<span data-ttu-id="37a1c-140">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="37a1c-140">Number of unknown devices</span></span>|
|<span data-ttu-id="37a1c-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37a1c-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="37a1c-142">Int32</span><span class="sxs-lookup"><span data-stu-id="37a1c-142">Int32</span></span>|<span data-ttu-id="37a1c-143">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="37a1c-143">Number of not applicable devices</span></span>|
|<span data-ttu-id="37a1c-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37a1c-144">compliantDeviceCount</span></span>|<span data-ttu-id="37a1c-145">Int32</span><span class="sxs-lookup"><span data-stu-id="37a1c-145">Int32</span></span>|<span data-ttu-id="37a1c-146">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="37a1c-146">Number of compliant devices</span></span>|
|<span data-ttu-id="37a1c-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37a1c-147">remediatedDeviceCount</span></span>|<span data-ttu-id="37a1c-148">Int32</span><span class="sxs-lookup"><span data-stu-id="37a1c-148">Int32</span></span>|<span data-ttu-id="37a1c-149">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="37a1c-149">Number of remediated devices</span></span>|
|<span data-ttu-id="37a1c-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37a1c-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="37a1c-151">Int32</span><span class="sxs-lookup"><span data-stu-id="37a1c-151">Int32</span></span>|<span data-ttu-id="37a1c-152">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="37a1c-152">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="37a1c-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37a1c-153">errorDeviceCount</span></span>|<span data-ttu-id="37a1c-154">Int32</span><span class="sxs-lookup"><span data-stu-id="37a1c-154">Int32</span></span>|<span data-ttu-id="37a1c-155">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="37a1c-155">Number of error devices</span></span>|
|<span data-ttu-id="37a1c-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37a1c-156">conflictDeviceCount</span></span>|<span data-ttu-id="37a1c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="37a1c-157">Int32</span></span>|<span data-ttu-id="37a1c-158">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="37a1c-158">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="37a1c-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a1c-159">Response</span></span>
<span data-ttu-id="37a1c-160">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37a1c-160">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37a1c-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37a1c-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="37a1c-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37a1c-162">Request</span></span>
<span data-ttu-id="37a1c-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37a1c-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 270

{
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="37a1c-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a1c-164">Response</span></span>
<span data-ttu-id="37a1c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37a1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```








