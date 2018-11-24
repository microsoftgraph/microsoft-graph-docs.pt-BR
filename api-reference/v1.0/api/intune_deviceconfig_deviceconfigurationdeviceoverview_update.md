# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="0bc84-101">Atualizar deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0bc84-101">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="0bc84-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0bc84-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bc84-103">Atualizar as propriedades de um objeto [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="0bc84-103">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0bc84-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0bc84-104">Prerequisites</span></span>
<span data-ttu-id="0bc84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0bc84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0bc84-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bc84-107">Permission type</span></span>|<span data-ttu-id="0bc84-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0bc84-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bc84-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bc84-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0bc84-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bc84-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0bc84-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bc84-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bc84-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bc84-112">Not supported.</span></span>|
|<span data-ttu-id="0bc84-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bc84-113">Application</span></span>|<span data-ttu-id="0bc84-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bc84-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bc84-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bc84-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="0bc84-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bc84-116">Request headers</span></span>
|<span data-ttu-id="0bc84-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0bc84-117">Header</span></span>|<span data-ttu-id="0bc84-118">Valor</span><span class="sxs-lookup"><span data-stu-id="0bc84-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bc84-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bc84-119">Authorization</span></span>|<span data-ttu-id="0bc84-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bc84-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bc84-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0bc84-121">Accept</span></span>|<span data-ttu-id="0bc84-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0bc84-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bc84-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bc84-123">Request body</span></span>
<span data-ttu-id="0bc84-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="0bc84-124">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="0bc84-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="0bc84-125">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="0bc84-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bc84-126">Property</span></span>|<span data-ttu-id="0bc84-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bc84-127">Type</span></span>|<span data-ttu-id="0bc84-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bc84-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bc84-129">id</span><span class="sxs-lookup"><span data-stu-id="0bc84-129">id</span></span>|<span data-ttu-id="0bc84-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bc84-130">String</span></span>|<span data-ttu-id="0bc84-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0bc84-131">Key of the entity.</span></span>|
|<span data-ttu-id="0bc84-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="0bc84-132">pendingCount</span></span>|<span data-ttu-id="0bc84-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0bc84-133">Int32</span></span>|<span data-ttu-id="0bc84-134">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="0bc84-134">Number of pending devices</span></span>|
|<span data-ttu-id="0bc84-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="0bc84-135">notApplicableCount</span></span>|<span data-ttu-id="0bc84-136">Int32</span><span class="sxs-lookup"><span data-stu-id="0bc84-136">Int32</span></span>|<span data-ttu-id="0bc84-137">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="0bc84-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="0bc84-138">successCount</span><span class="sxs-lookup"><span data-stu-id="0bc84-138">successCount</span></span>|<span data-ttu-id="0bc84-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0bc84-139">Int32</span></span>|<span data-ttu-id="0bc84-140">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="0bc84-140">Number of succeeded devices</span></span>|
|<span data-ttu-id="0bc84-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="0bc84-141">errorCount</span></span>|<span data-ttu-id="0bc84-142">Int32</span><span class="sxs-lookup"><span data-stu-id="0bc84-142">Int32</span></span>|<span data-ttu-id="0bc84-143">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="0bc84-143">Number of error devices</span></span>|
|<span data-ttu-id="0bc84-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="0bc84-144">failedCount</span></span>|<span data-ttu-id="0bc84-145">Int32</span><span class="sxs-lookup"><span data-stu-id="0bc84-145">Int32</span></span>|<span data-ttu-id="0bc84-146">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="0bc84-146">Number of failed devices</span></span>|
|<span data-ttu-id="0bc84-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0bc84-147">lastUpdateDateTime</span></span>|<span data-ttu-id="0bc84-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bc84-148">DateTimeOffset</span></span>|<span data-ttu-id="0bc84-149">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="0bc84-149">Last update time</span></span>|
|<span data-ttu-id="0bc84-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="0bc84-150">configurationVersion</span></span>|<span data-ttu-id="0bc84-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0bc84-151">Int32</span></span>|<span data-ttu-id="0bc84-152">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="0bc84-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="0bc84-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bc84-153">Response</span></span>
<span data-ttu-id="0bc84-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bc84-154">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bc84-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0bc84-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="0bc84-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bc84-156">Request</span></span>
<span data-ttu-id="0bc84-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bc84-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 284

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="0bc84-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bc84-158">Response</span></span>
<span data-ttu-id="0bc84-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0bc84-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



