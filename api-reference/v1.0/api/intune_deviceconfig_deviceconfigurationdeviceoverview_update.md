# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="241ef-101">Atualizar deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="241ef-101">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="241ef-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="241ef-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="241ef-103">Atualizar as propriedades de um objeto [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="241ef-103">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="241ef-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="241ef-104">Prerequisites</span></span>
<span data-ttu-id="241ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="241ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="241ef-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="241ef-107">Permission type</span></span>|<span data-ttu-id="241ef-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="241ef-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="241ef-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="241ef-109">Delegated (work or school account)</span></span>|<span data-ttu-id="241ef-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="241ef-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="241ef-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="241ef-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="241ef-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="241ef-112">Not supported.</span></span>|
|<span data-ttu-id="241ef-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="241ef-113">Application</span></span>|<span data-ttu-id="241ef-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="241ef-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="241ef-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="241ef-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="241ef-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="241ef-116">Request headers</span></span>
|<span data-ttu-id="241ef-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="241ef-117">Header</span></span>|<span data-ttu-id="241ef-118">Valor</span><span class="sxs-lookup"><span data-stu-id="241ef-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="241ef-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="241ef-119">Authorization</span></span>|<span data-ttu-id="241ef-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="241ef-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="241ef-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="241ef-121">Accept</span></span>|<span data-ttu-id="241ef-122">application/json</span><span class="sxs-lookup"><span data-stu-id="241ef-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="241ef-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="241ef-123">Request body</span></span>
<span data-ttu-id="241ef-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="241ef-124">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="241ef-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="241ef-125">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="241ef-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="241ef-126">Property</span></span>|<span data-ttu-id="241ef-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="241ef-127">Type</span></span>|<span data-ttu-id="241ef-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="241ef-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="241ef-129">id</span><span class="sxs-lookup"><span data-stu-id="241ef-129">id</span></span>|<span data-ttu-id="241ef-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="241ef-130">String</span></span>|<span data-ttu-id="241ef-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="241ef-131">Key of the entity.</span></span>|
|<span data-ttu-id="241ef-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="241ef-132">pendingCount</span></span>|<span data-ttu-id="241ef-133">Int32</span><span class="sxs-lookup"><span data-stu-id="241ef-133">Int32</span></span>|<span data-ttu-id="241ef-134">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="241ef-134">Number of pending devices</span></span>|
|<span data-ttu-id="241ef-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="241ef-135">notApplicableCount</span></span>|<span data-ttu-id="241ef-136">Int32</span><span class="sxs-lookup"><span data-stu-id="241ef-136">Int32</span></span>|<span data-ttu-id="241ef-137">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="241ef-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="241ef-138">successCount</span><span class="sxs-lookup"><span data-stu-id="241ef-138">successCount</span></span>|<span data-ttu-id="241ef-139">Int32</span><span class="sxs-lookup"><span data-stu-id="241ef-139">Int32</span></span>|<span data-ttu-id="241ef-140">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="241ef-140">Number of succeeded devices</span></span>|
|<span data-ttu-id="241ef-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="241ef-141">errorCount</span></span>|<span data-ttu-id="241ef-142">Int32</span><span class="sxs-lookup"><span data-stu-id="241ef-142">Int32</span></span>|<span data-ttu-id="241ef-143">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="241ef-143">Number of error devices</span></span>|
|<span data-ttu-id="241ef-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="241ef-144">failedCount</span></span>|<span data-ttu-id="241ef-145">Int32</span><span class="sxs-lookup"><span data-stu-id="241ef-145">Int32</span></span>|<span data-ttu-id="241ef-146">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="241ef-146">Number of failed devices</span></span>|
|<span data-ttu-id="241ef-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="241ef-147">lastUpdateDateTime</span></span>|<span data-ttu-id="241ef-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="241ef-148">DateTimeOffset</span></span>|<span data-ttu-id="241ef-149">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="241ef-149">Last update time</span></span>|
|<span data-ttu-id="241ef-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="241ef-150">configurationVersion</span></span>|<span data-ttu-id="241ef-151">Int32</span><span class="sxs-lookup"><span data-stu-id="241ef-151">Int32</span></span>|<span data-ttu-id="241ef-152">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="241ef-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="241ef-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="241ef-153">Response</span></span>
<span data-ttu-id="241ef-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="241ef-154">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="241ef-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="241ef-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="241ef-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="241ef-156">Request</span></span>
<span data-ttu-id="241ef-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="241ef-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 212

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="241ef-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="241ef-158">Response</span></span>
<span data-ttu-id="241ef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="241ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 333

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```








