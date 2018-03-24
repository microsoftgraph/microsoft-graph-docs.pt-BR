# <a name="update-manageddeviceoverview"></a><span data-ttu-id="56e70-101">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="56e70-101">Update managedDeviceOverview</span></span>

> <span data-ttu-id="56e70-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="56e70-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56e70-103">Atualizar as propriedades de um objeto [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="56e70-103">Update the properties of a [calendar](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56e70-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56e70-104">Prerequisites</span></span>
<span data-ttu-id="56e70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="56e70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="56e70-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56e70-107">Permission type</span></span>|<span data-ttu-id="56e70-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56e70-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56e70-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56e70-109">Delegated (work or school account)</span></span>|<span data-ttu-id="56e70-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56e70-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="56e70-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56e70-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56e70-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56e70-112">Not supported.</span></span>|
|<span data-ttu-id="56e70-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56e70-113">Application</span></span>|<span data-ttu-id="56e70-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56e70-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56e70-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56e70-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="56e70-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56e70-116">Request headers</span></span>
|<span data-ttu-id="56e70-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56e70-117">Header</span></span>|<span data-ttu-id="56e70-118">Valor</span><span class="sxs-lookup"><span data-stu-id="56e70-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56e70-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="56e70-119">Authorization</span></span>|<span data-ttu-id="56e70-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56e70-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="56e70-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="56e70-121">Accept</span></span>|<span data-ttu-id="56e70-122">application/json</span><span class="sxs-lookup"><span data-stu-id="56e70-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56e70-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56e70-123">Request body</span></span>
<span data-ttu-id="56e70-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="56e70-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="56e70-125">A tabela a seguir mostra as propriedades necessárias ao criar [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="56e70-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="56e70-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56e70-126">Property</span></span>|<span data-ttu-id="56e70-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="56e70-127">Type</span></span>|<span data-ttu-id="56e70-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="56e70-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56e70-129">id</span><span class="sxs-lookup"><span data-stu-id="56e70-129">id</span></span>|<span data-ttu-id="56e70-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56e70-130">String</span></span>|<span data-ttu-id="56e70-131">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="56e70-131">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="56e70-132">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56e70-132">enrolledDeviceCount</span></span>|<span data-ttu-id="56e70-133">Int32</span><span class="sxs-lookup"><span data-stu-id="56e70-133">Int32</span></span>|<span data-ttu-id="56e70-134">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="56e70-134">Total enrolled device count.</span></span> <span data-ttu-id="56e70-135">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="56e70-135">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="56e70-136">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="56e70-136">mdmEnrolledCount</span></span>|<span data-ttu-id="56e70-137">Int32</span><span class="sxs-lookup"><span data-stu-id="56e70-137">Int32</span></span>|<span data-ttu-id="56e70-138">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="56e70-138">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="56e70-139">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56e70-139">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="56e70-140">Int32</span><span class="sxs-lookup"><span data-stu-id="56e70-140">Int32</span></span>|<span data-ttu-id="56e70-141">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="56e70-141">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="56e70-142">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="56e70-142">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="56e70-143">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="56e70-143">deviceOperatingSystemSummary</span></span>](../resources/intune_devices_deviceoperatingsystemsummary.md)|<span data-ttu-id="56e70-144">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="56e70-144">Device operating system summary.</span></span>|
|<span data-ttu-id="56e70-145">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="56e70-145">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="56e70-146">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="56e70-146">deviceExchangeAccessStateSummary</span></span>](../resources/intune_devices_deviceexchangeaccessstatesummary.md)|<span data-ttu-id="56e70-147">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="56e70-147">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="56e70-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="56e70-148">Response</span></span>
<span data-ttu-id="56e70-149">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56e70-149">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_devices_manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56e70-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56e70-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="56e70-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56e70-151">Request</span></span>
<span data-ttu-id="56e70-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56e70-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 625

{
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  }
}
```

### <a name="response"></a><span data-ttu-id="56e70-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="56e70-153">Response</span></span>
<span data-ttu-id="56e70-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56e70-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 734

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "42a91653-1653-42a9-5316-a9425316a942",
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  }
}
```



