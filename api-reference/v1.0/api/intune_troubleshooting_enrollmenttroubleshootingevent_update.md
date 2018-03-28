# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="fbf8e-101">Atualizar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="fbf8e-101">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="fbf8e-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbf8e-103">Atualiza as propriedades de um objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="fbf8e-103">Update the properties of a [calendar](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fbf8e-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbf8e-104">Prerequisites</span></span>
<span data-ttu-id="fbf8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fbf8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fbf8e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbf8e-107">Permission type</span></span>|<span data-ttu-id="fbf8e-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbf8e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbf8e-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbf8e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fbf8e-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbf8e-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fbf8e-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbf8e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbf8e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-112">Not supported.</span></span>|
|<span data-ttu-id="fbf8e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbf8e-113">Application</span></span>|<span data-ttu-id="fbf8e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbf8e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbf8e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="fbf8e-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbf8e-116">Request headers</span></span>
|<span data-ttu-id="fbf8e-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbf8e-117">Header</span></span>|<span data-ttu-id="fbf8e-118">Valor</span><span class="sxs-lookup"><span data-stu-id="fbf8e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbf8e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbf8e-119">Authorization</span></span>|<span data-ttu-id="fbf8e-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fbf8e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fbf8e-121">Accept</span></span>|<span data-ttu-id="fbf8e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fbf8e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbf8e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbf8e-123">Request body</span></span>
<span data-ttu-id="fbf8e-124">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="fbf8e-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="fbf8e-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="fbf8e-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="fbf8e-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbf8e-126">Property</span></span>|<span data-ttu-id="fbf8e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbf8e-127">Type</span></span>|<span data-ttu-id="fbf8e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbf8e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbf8e-129">id</span><span class="sxs-lookup"><span data-stu-id="fbf8e-129">id</span></span>|<span data-ttu-id="fbf8e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf8e-130">String</span></span>|<span data-ttu-id="fbf8e-131">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="fbf8e-131">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="fbf8e-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="fbf8e-132">eventDateTime</span></span>|<span data-ttu-id="fbf8e-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbf8e-133">DateTimeOffset</span></span>|<span data-ttu-id="fbf8e-134">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-134">Time when the event occurred .</span></span> <span data-ttu-id="fbf8e-135">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="fbf8e-135">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="fbf8e-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="fbf8e-136">correlationId</span></span>|<span data-ttu-id="fbf8e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf8e-137">String</span></span>|<span data-ttu-id="fbf8e-138">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-138">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="fbf8e-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="fbf8e-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="fbf8e-140">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="fbf8e-140">managedDeviceIdentifier</span></span>|<span data-ttu-id="fbf8e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf8e-141">String</span></span>|<span data-ttu-id="fbf8e-142">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-142">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="fbf8e-143">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="fbf8e-143">operatingSystem</span></span>|<span data-ttu-id="fbf8e-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf8e-144">String</span></span>|<span data-ttu-id="fbf8e-145">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-145">Operating system</span></span>|
|<span data-ttu-id="fbf8e-146">osVersion</span><span class="sxs-lookup"><span data-stu-id="fbf8e-146">osVersion</span></span>|<span data-ttu-id="fbf8e-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf8e-147">String</span></span>|<span data-ttu-id="fbf8e-148">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-148">OS Version.</span></span>|
|<span data-ttu-id="fbf8e-149">userId</span><span class="sxs-lookup"><span data-stu-id="fbf8e-149">userId</span></span>|<span data-ttu-id="fbf8e-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf8e-150">String</span></span>|<span data-ttu-id="fbf8e-151">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-151">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="fbf8e-152">deviceId</span><span class="sxs-lookup"><span data-stu-id="fbf8e-152">deviceId</span></span>|<span data-ttu-id="fbf8e-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf8e-153">String</span></span>|<span data-ttu-id="fbf8e-154">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-154">Azure AD device identifier.</span></span>|
|<span data-ttu-id="fbf8e-155">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="fbf8e-155">enrollmentType</span></span>|<span data-ttu-id="fbf8e-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf8e-156">String</span></span>|<span data-ttu-id="fbf8e-157">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-157">Type of the enrollment.</span></span> <span data-ttu-id="fbf8e-158">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-158">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="fbf8e-159">failureCategory</span><span class="sxs-lookup"><span data-stu-id="fbf8e-159">failureCategory</span></span>|<span data-ttu-id="fbf8e-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf8e-160">String</span></span>|<span data-ttu-id="fbf8e-161">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-161">Highlevel failure category.</span></span> <span data-ttu-id="fbf8e-162">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-162">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.</span></span>|
|<span data-ttu-id="fbf8e-163">failureReason</span><span class="sxs-lookup"><span data-stu-id="fbf8e-163">failureReason</span></span>|<span data-ttu-id="fbf8e-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf8e-164">String</span></span>|<span data-ttu-id="fbf8e-165">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-165">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="fbf8e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbf8e-166">Response</span></span>
<span data-ttu-id="fbf8e-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-167">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbf8e-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbf8e-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="fbf8e-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbf8e-169">Request</span></span>
<span data-ttu-id="fbf8e-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 440

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```

### <a name="response"></a><span data-ttu-id="fbf8e-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbf8e-171">Response</span></span>
<span data-ttu-id="fbf8e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbf8e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 558

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```



