# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="af8ea-101">Atualizar managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="af8ea-101">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="af8ea-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="af8ea-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af8ea-103">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="af8ea-103">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af8ea-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af8ea-104">Prerequisites</span></span>
<span data-ttu-id="af8ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="af8ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="af8ea-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af8ea-107">Permission type</span></span>|<span data-ttu-id="af8ea-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af8ea-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af8ea-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af8ea-109">Delegated (work or school account)</span></span>|<span data-ttu-id="af8ea-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af8ea-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="af8ea-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af8ea-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af8ea-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af8ea-112">Not supported.</span></span>|
|<span data-ttu-id="af8ea-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af8ea-113">Application</span></span>|<span data-ttu-id="af8ea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af8ea-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af8ea-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af8ea-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="af8ea-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af8ea-116">Request headers</span></span>
|<span data-ttu-id="af8ea-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af8ea-117">Header</span></span>|<span data-ttu-id="af8ea-118">Valor</span><span class="sxs-lookup"><span data-stu-id="af8ea-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af8ea-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="af8ea-119">Authorization</span></span>|<span data-ttu-id="af8ea-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="af8ea-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af8ea-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af8ea-121">Accept</span></span>|<span data-ttu-id="af8ea-122">application/json</span><span class="sxs-lookup"><span data-stu-id="af8ea-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af8ea-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af8ea-123">Request body</span></span>
<span data-ttu-id="af8ea-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="af8ea-124">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="af8ea-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="af8ea-125">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="af8ea-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af8ea-126">Property</span></span>|<span data-ttu-id="af8ea-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="af8ea-127">Type</span></span>|<span data-ttu-id="af8ea-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="af8ea-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af8ea-129">id</span><span class="sxs-lookup"><span data-stu-id="af8ea-129">id</span></span>|<span data-ttu-id="af8ea-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af8ea-130">String</span></span>|<span data-ttu-id="af8ea-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="af8ea-131">Key of the entity.</span></span>|
|<span data-ttu-id="af8ea-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="af8ea-132">pendingCount</span></span>|<span data-ttu-id="af8ea-133">Int32</span><span class="sxs-lookup"><span data-stu-id="af8ea-133">Int32</span></span>|<span data-ttu-id="af8ea-134">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="af8ea-134">Number of pending devices</span></span>|
|<span data-ttu-id="af8ea-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="af8ea-135">notApplicableCount</span></span>|<span data-ttu-id="af8ea-136">Int32</span><span class="sxs-lookup"><span data-stu-id="af8ea-136">Int32</span></span>|<span data-ttu-id="af8ea-137">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="af8ea-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="af8ea-138">successCount</span><span class="sxs-lookup"><span data-stu-id="af8ea-138">successCount</span></span>|<span data-ttu-id="af8ea-139">Int32</span><span class="sxs-lookup"><span data-stu-id="af8ea-139">Int32</span></span>|<span data-ttu-id="af8ea-140">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="af8ea-140">Number of succeeded devices</span></span>|
|<span data-ttu-id="af8ea-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="af8ea-141">errorCount</span></span>|<span data-ttu-id="af8ea-142">Int32</span><span class="sxs-lookup"><span data-stu-id="af8ea-142">Int32</span></span>|<span data-ttu-id="af8ea-143">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="af8ea-143">Number of error devices</span></span>|
|<span data-ttu-id="af8ea-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="af8ea-144">failedCount</span></span>|<span data-ttu-id="af8ea-145">Int32</span><span class="sxs-lookup"><span data-stu-id="af8ea-145">Int32</span></span>|<span data-ttu-id="af8ea-146">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="af8ea-146">Number of failed devices</span></span>|
|<span data-ttu-id="af8ea-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="af8ea-147">lastUpdateDateTime</span></span>|<span data-ttu-id="af8ea-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af8ea-148">DateTimeOffset</span></span>|<span data-ttu-id="af8ea-149">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="af8ea-149">Last update time</span></span>|
|<span data-ttu-id="af8ea-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="af8ea-150">configurationVersion</span></span>|<span data-ttu-id="af8ea-151">Int32</span><span class="sxs-lookup"><span data-stu-id="af8ea-151">Int32</span></span>|<span data-ttu-id="af8ea-152">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="af8ea-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="af8ea-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="af8ea-153">Response</span></span>
<span data-ttu-id="af8ea-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af8ea-154">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af8ea-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af8ea-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="af8ea-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af8ea-156">Request</span></span>
<span data-ttu-id="af8ea-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af8ea-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
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

### <a name="response"></a><span data-ttu-id="af8ea-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="af8ea-158">Response</span></span>
<span data-ttu-id="af8ea-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af8ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 348

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```








