# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="01995-101">Atualizar deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="01995-101">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="01995-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="01995-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01995-103">Atualizar as propriedades de um objeto [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="01995-103">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01995-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01995-104">Prerequisites</span></span>
<span data-ttu-id="01995-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="01995-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01995-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01995-107">Permission type</span></span>|<span data-ttu-id="01995-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01995-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01995-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01995-109">Delegated (work or school account)</span></span>|<span data-ttu-id="01995-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01995-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="01995-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01995-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01995-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01995-112">Not supported.</span></span>|
|<span data-ttu-id="01995-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01995-113">Application</span></span>|<span data-ttu-id="01995-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01995-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01995-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01995-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="01995-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01995-116">Request headers</span></span>
|<span data-ttu-id="01995-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01995-117">Header</span></span>|<span data-ttu-id="01995-118">Valor</span><span class="sxs-lookup"><span data-stu-id="01995-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01995-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="01995-119">Authorization</span></span>|<span data-ttu-id="01995-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01995-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01995-121">Accept</span><span class="sxs-lookup"><span data-stu-id="01995-121">Accept</span></span>|<span data-ttu-id="01995-122">application/json</span><span class="sxs-lookup"><span data-stu-id="01995-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01995-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01995-123">Request body</span></span>
<span data-ttu-id="01995-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="01995-124">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="01995-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="01995-125">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="01995-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01995-126">Property</span></span>|<span data-ttu-id="01995-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="01995-127">Type</span></span>|<span data-ttu-id="01995-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="01995-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01995-129">id</span><span class="sxs-lookup"><span data-stu-id="01995-129">id</span></span>|<span data-ttu-id="01995-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01995-130">String</span></span>|<span data-ttu-id="01995-131">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="01995-131">UUID for the object</span></span>|
|<span data-ttu-id="01995-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="01995-132">eventDateTime</span></span>|<span data-ttu-id="01995-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01995-133">DateTimeOffset</span></span>|<span data-ttu-id="01995-134">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="01995-134">Time when the event occurred .</span></span>|
|<span data-ttu-id="01995-135">correlationId</span><span class="sxs-lookup"><span data-stu-id="01995-135">correlationId</span></span>|<span data-ttu-id="01995-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01995-136">String</span></span>|<span data-ttu-id="01995-137">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="01995-137">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="01995-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="01995-138">Response</span></span>
<span data-ttu-id="01995-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01995-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01995-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01995-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="01995-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01995-141">Request</span></span>
<span data-ttu-id="01995-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01995-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 104

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="01995-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="01995-143">Response</span></span>
<span data-ttu-id="01995-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01995-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```



