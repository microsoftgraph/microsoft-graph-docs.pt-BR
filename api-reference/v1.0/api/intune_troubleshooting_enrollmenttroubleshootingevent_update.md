# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="df4a8-101">Atualizar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="df4a8-101">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="df4a8-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="df4a8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df4a8-103">Atualiza as propriedades de um objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="df4a8-103">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df4a8-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df4a8-104">Prerequisites</span></span>
<span data-ttu-id="df4a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="df4a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="df4a8-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df4a8-107">Permission type</span></span>|<span data-ttu-id="df4a8-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df4a8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df4a8-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df4a8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="df4a8-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df4a8-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="df4a8-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df4a8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df4a8-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df4a8-112">Not supported.</span></span>|
|<span data-ttu-id="df4a8-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df4a8-113">Application</span></span>|<span data-ttu-id="df4a8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df4a8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df4a8-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df4a8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="df4a8-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df4a8-116">Request headers</span></span>
|<span data-ttu-id="df4a8-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df4a8-117">Header</span></span>|<span data-ttu-id="df4a8-118">Valor</span><span class="sxs-lookup"><span data-stu-id="df4a8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df4a8-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="df4a8-119">Authorization</span></span>|<span data-ttu-id="df4a8-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df4a8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df4a8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="df4a8-121">Accept</span></span>|<span data-ttu-id="df4a8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="df4a8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df4a8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df4a8-123">Request body</span></span>
<span data-ttu-id="df4a8-124">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="df4a8-124">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="df4a8-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="df4a8-125">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="df4a8-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df4a8-126">Property</span></span>|<span data-ttu-id="df4a8-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="df4a8-127">Type</span></span>|<span data-ttu-id="df4a8-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="df4a8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df4a8-129">id</span><span class="sxs-lookup"><span data-stu-id="df4a8-129">id</span></span>|<span data-ttu-id="df4a8-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df4a8-130">String</span></span>|<span data-ttu-id="df4a8-131">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="df4a8-131">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="df4a8-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="df4a8-132">eventDateTime</span></span>|<span data-ttu-id="df4a8-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df4a8-133">DateTimeOffset</span></span>|<span data-ttu-id="df4a8-134">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="df4a8-134">Time when the event occurred .</span></span> <span data-ttu-id="df4a8-135">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="df4a8-135">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="df4a8-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="df4a8-136">correlationId</span></span>|<span data-ttu-id="df4a8-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df4a8-137">String</span></span>|<span data-ttu-id="df4a8-138">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="df4a8-138">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="df4a8-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="df4a8-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="df4a8-140">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="df4a8-140">managedDeviceIdentifier</span></span>|<span data-ttu-id="df4a8-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df4a8-141">String</span></span>|<span data-ttu-id="df4a8-142">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="df4a8-142">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="df4a8-143">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="df4a8-143">operatingSystem</span></span>|<span data-ttu-id="df4a8-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df4a8-144">String</span></span>|<span data-ttu-id="df4a8-145">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="df4a8-145">Operating System.</span></span>|
|<span data-ttu-id="df4a8-146">osVersion</span><span class="sxs-lookup"><span data-stu-id="df4a8-146">osVersion</span></span>|<span data-ttu-id="df4a8-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df4a8-147">String</span></span>|<span data-ttu-id="df4a8-148">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="df4a8-148">OS Version.</span></span>|
|<span data-ttu-id="df4a8-149">userId</span><span class="sxs-lookup"><span data-stu-id="df4a8-149">userId</span></span>|<span data-ttu-id="df4a8-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df4a8-150">String</span></span>|<span data-ttu-id="df4a8-151">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="df4a8-151">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="df4a8-152">deviceId</span><span class="sxs-lookup"><span data-stu-id="df4a8-152">deviceId</span></span>|<span data-ttu-id="df4a8-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df4a8-153">String</span></span>|<span data-ttu-id="df4a8-154">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="df4a8-154">Azure AD device identifier.</span></span>|
|<span data-ttu-id="df4a8-155">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="df4a8-155">enrollmentType</span></span>|[<span data-ttu-id="df4a8-156">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="df4a8-156">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="df4a8-157">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="df4a8-157">Type of the enrollment.</span></span> <span data-ttu-id="df4a8-158">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="df4a8-158">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="df4a8-159">failureCategory</span><span class="sxs-lookup"><span data-stu-id="df4a8-159">failureCategory</span></span>|[<span data-ttu-id="df4a8-160">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="df4a8-160">deviceEnrollmentFailureReason</span></span>](../resources/intune_troubleshooting_deviceenrollmentfailurereason.md)|<span data-ttu-id="df4a8-161">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="df4a8-161">Highlevel failure category.</span></span> <span data-ttu-id="df4a8-162">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="df4a8-162">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="df4a8-163">failureReason</span><span class="sxs-lookup"><span data-stu-id="df4a8-163">failureReason</span></span>|<span data-ttu-id="df4a8-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df4a8-164">String</span></span>|<span data-ttu-id="df4a8-165">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="df4a8-165">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="df4a8-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="df4a8-166">Response</span></span>
<span data-ttu-id="df4a8-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df4a8-167">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df4a8-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df4a8-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="df4a8-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df4a8-169">Request</span></span>
<span data-ttu-id="df4a8-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df4a8-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="df4a8-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="df4a8-171">Response</span></span>
<span data-ttu-id="df4a8-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df4a8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



