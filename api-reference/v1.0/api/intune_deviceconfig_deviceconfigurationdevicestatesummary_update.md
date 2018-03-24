# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="3cb20-101">Atualizar deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="3cb20-101">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="3cb20-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3cb20-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cb20-103">Atualizar as propriedades de um objeto [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3cb20-103">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3cb20-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3cb20-104">Prerequisites</span></span>
<span data-ttu-id="3cb20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3cb20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3cb20-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cb20-107">Permission type</span></span>|<span data-ttu-id="3cb20-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3cb20-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cb20-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cb20-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3cb20-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cb20-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3cb20-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cb20-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cb20-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cb20-112">Not supported.</span></span>|
|<span data-ttu-id="3cb20-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cb20-113">Application</span></span>|<span data-ttu-id="3cb20-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cb20-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cb20-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cb20-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="3cb20-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cb20-116">Request headers</span></span>
|<span data-ttu-id="3cb20-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3cb20-117">Header</span></span>|<span data-ttu-id="3cb20-118">Valor</span><span class="sxs-lookup"><span data-stu-id="3cb20-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cb20-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cb20-119">Authorization</span></span>|<span data-ttu-id="3cb20-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cb20-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3cb20-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3cb20-121">Accept</span></span>|<span data-ttu-id="3cb20-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3cb20-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cb20-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cb20-123">Request body</span></span>
<span data-ttu-id="3cb20-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3cb20-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="3cb20-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3cb20-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="3cb20-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cb20-126">Property</span></span>|<span data-ttu-id="3cb20-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cb20-127">Type</span></span>|<span data-ttu-id="3cb20-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cb20-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cb20-129">id</span><span class="sxs-lookup"><span data-stu-id="3cb20-129">id</span></span>|<span data-ttu-id="3cb20-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3cb20-130">String</span></span>|<span data-ttu-id="3cb20-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3cb20-131">Key of the setting.</span></span>|
|<span data-ttu-id="3cb20-132">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3cb20-132">unknownDeviceCount</span></span>|<span data-ttu-id="3cb20-133">Int32</span><span class="sxs-lookup"><span data-stu-id="3cb20-133">Int32</span></span>|<span data-ttu-id="3cb20-134">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="3cb20-134">Number of unknown devices</span></span>|
|<span data-ttu-id="3cb20-135">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3cb20-135">notApplicableDeviceCount</span></span>|<span data-ttu-id="3cb20-136">Int32</span><span class="sxs-lookup"><span data-stu-id="3cb20-136">Int32</span></span>|<span data-ttu-id="3cb20-137">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="3cb20-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="3cb20-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3cb20-138">compliantDeviceCount</span></span>|<span data-ttu-id="3cb20-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3cb20-139">Int32</span></span>|<span data-ttu-id="3cb20-140">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="3cb20-140">Number of compliant devices</span></span>|
|<span data-ttu-id="3cb20-141">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3cb20-141">remediatedDeviceCount</span></span>|<span data-ttu-id="3cb20-142">Int32</span><span class="sxs-lookup"><span data-stu-id="3cb20-142">Int32</span></span>|<span data-ttu-id="3cb20-143">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="3cb20-143">Number of remediated devices</span></span>|
|<span data-ttu-id="3cb20-144">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3cb20-144">nonCompliantDeviceCount</span></span>|<span data-ttu-id="3cb20-145">Int32</span><span class="sxs-lookup"><span data-stu-id="3cb20-145">Int32</span></span>|<span data-ttu-id="3cb20-146">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="3cb20-146">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="3cb20-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3cb20-147">errorDeviceCount</span></span>|<span data-ttu-id="3cb20-148">Int32</span><span class="sxs-lookup"><span data-stu-id="3cb20-148">Int32</span></span>|<span data-ttu-id="3cb20-149">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="3cb20-149">Number of error devices</span></span>|
|<span data-ttu-id="3cb20-150">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3cb20-150">conflictDeviceCount</span></span>|<span data-ttu-id="3cb20-151">Int32</span><span class="sxs-lookup"><span data-stu-id="3cb20-151">Int32</span></span>|<span data-ttu-id="3cb20-152">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="3cb20-152">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="3cb20-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cb20-153">Response</span></span>
<span data-ttu-id="3cb20-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cb20-154">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cb20-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cb20-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="3cb20-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cb20-156">Request</span></span>
<span data-ttu-id="3cb20-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cb20-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 214

{
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="3cb20-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cb20-158">Response</span></span>
<span data-ttu-id="3cb20-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3cb20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



