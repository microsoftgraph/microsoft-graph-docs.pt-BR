# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="1c5c4-101">Atualizar deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="1c5c4-101">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="1c5c4-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1c5c4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c5c4-103">Atualizar as propriedades de um objeto [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1c5c4-103">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c5c4-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c5c4-104">Prerequisites</span></span>
<span data-ttu-id="1c5c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c5c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c5c4-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c5c4-107">Permission type</span></span>|<span data-ttu-id="1c5c4-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c5c4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c5c4-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c5c4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1c5c4-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c5c4-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c5c4-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c5c4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c5c4-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c5c4-112">Not supported.</span></span>|
|<span data-ttu-id="1c5c4-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c5c4-113">Application</span></span>|<span data-ttu-id="1c5c4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c5c4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c5c4-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c5c4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="1c5c4-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c5c4-116">Request headers</span></span>
|<span data-ttu-id="1c5c4-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c5c4-117">Header</span></span>|<span data-ttu-id="1c5c4-118">Valor</span><span class="sxs-lookup"><span data-stu-id="1c5c4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c5c4-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c5c4-119">Authorization</span></span>|<span data-ttu-id="1c5c4-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c5c4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c5c4-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c5c4-121">Accept</span></span>|<span data-ttu-id="1c5c4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1c5c4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c5c4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c5c4-123">Request body</span></span>
<span data-ttu-id="1c5c4-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1c5c4-124">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="1c5c4-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1c5c4-125">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="1c5c4-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c5c4-126">Property</span></span>|<span data-ttu-id="1c5c4-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c5c4-127">Type</span></span>|<span data-ttu-id="1c5c4-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c5c4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c5c4-129">id</span><span class="sxs-lookup"><span data-stu-id="1c5c4-129">id</span></span>|<span data-ttu-id="1c5c4-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c5c4-130">String</span></span>|<span data-ttu-id="1c5c4-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1c5c4-131">Key of the entity.</span></span>|
|<span data-ttu-id="1c5c4-132">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1c5c4-132">unknownDeviceCount</span></span>|<span data-ttu-id="1c5c4-133">Int32</span><span class="sxs-lookup"><span data-stu-id="1c5c4-133">Int32</span></span>|<span data-ttu-id="1c5c4-134">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="1c5c4-134">Number of unknown devices</span></span>|
|<span data-ttu-id="1c5c4-135">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1c5c4-135">notApplicableDeviceCount</span></span>|<span data-ttu-id="1c5c4-136">Int32</span><span class="sxs-lookup"><span data-stu-id="1c5c4-136">Int32</span></span>|<span data-ttu-id="1c5c4-137">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="1c5c4-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="1c5c4-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1c5c4-138">compliantDeviceCount</span></span>|<span data-ttu-id="1c5c4-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1c5c4-139">Int32</span></span>|<span data-ttu-id="1c5c4-140">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="1c5c4-140">Number of compliant devices</span></span>|
|<span data-ttu-id="1c5c4-141">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1c5c4-141">remediatedDeviceCount</span></span>|<span data-ttu-id="1c5c4-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1c5c4-142">Int32</span></span>|<span data-ttu-id="1c5c4-143">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="1c5c4-143">Number of remediated devices</span></span>|
|<span data-ttu-id="1c5c4-144">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1c5c4-144">nonCompliantDeviceCount</span></span>|<span data-ttu-id="1c5c4-145">Int32</span><span class="sxs-lookup"><span data-stu-id="1c5c4-145">Int32</span></span>|<span data-ttu-id="1c5c4-146">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="1c5c4-146">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="1c5c4-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1c5c4-147">errorDeviceCount</span></span>|<span data-ttu-id="1c5c4-148">Int32</span><span class="sxs-lookup"><span data-stu-id="1c5c4-148">Int32</span></span>|<span data-ttu-id="1c5c4-149">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="1c5c4-149">Number of error devices</span></span>|
|<span data-ttu-id="1c5c4-150">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1c5c4-150">conflictDeviceCount</span></span>|<span data-ttu-id="1c5c4-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1c5c4-151">Int32</span></span>|<span data-ttu-id="1c5c4-152">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="1c5c4-152">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="1c5c4-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c5c4-153">Response</span></span>
<span data-ttu-id="1c5c4-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c5c4-154">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c5c4-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c5c4-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c5c4-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c5c4-156">Request</span></span>
<span data-ttu-id="1c5c4-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c5c4-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="1c5c4-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c5c4-158">Response</span></span>
<span data-ttu-id="1c5c4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c5c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



