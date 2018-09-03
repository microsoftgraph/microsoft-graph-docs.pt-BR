# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="e725c-101">Atualizar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e725c-101">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="e725c-102">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e725c-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e725c-103">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e725c-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e725c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e725c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e725c-105">Atualiza as propriedades de um objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e725c-105">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e725c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e725c-106">Prerequisites</span></span>
<span data-ttu-id="e725c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e725c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e725c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e725c-109">Permission type</span></span>|<span data-ttu-id="e725c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e725c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e725c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e725c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e725c-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e725c-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e725c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e725c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e725c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e725c-114">Not supported.</span></span>|
|<span data-ttu-id="e725c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e725c-115">Application</span></span>|<span data-ttu-id="e725c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e725c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e725c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e725c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="e725c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e725c-118">Request headers</span></span>
|<span data-ttu-id="e725c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e725c-119">Header</span></span>|<span data-ttu-id="e725c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e725c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e725c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e725c-121">Authorization</span></span>|<span data-ttu-id="e725c-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="e725c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e725c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e725c-123">Accept</span></span>|<span data-ttu-id="e725c-124">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="e725c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e725c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e725c-125">Request body</span></span>
<span data-ttu-id="e725c-126">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e725c-126">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="e725c-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e725c-127">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="e725c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e725c-128">Property</span></span>|<span data-ttu-id="e725c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e725c-129">Type</span></span>|<span data-ttu-id="e725c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e725c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e725c-131">id</span><span class="sxs-lookup"><span data-stu-id="e725c-131">id</span></span>|<span data-ttu-id="e725c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e725c-132">String</span></span>|<span data-ttu-id="e725c-133">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e725c-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e725c-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="e725c-134">eventDateTime</span></span>|<span data-ttu-id="e725c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e725c-135">DateTimeOffset</span></span>|<span data-ttu-id="e725c-136">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="e725c-136">Time when the event occurred .</span></span> <span data-ttu-id="e725c-137">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e725c-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e725c-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="e725c-138">correlationId</span></span>|<span data-ttu-id="e725c-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e725c-139">String</span></span>|<span data-ttu-id="e725c-140">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="e725c-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="e725c-141">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e725c-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e725c-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e725c-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="e725c-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e725c-143">String</span></span>|<span data-ttu-id="e725c-144">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="e725c-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="e725c-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="e725c-145">operatingSystem</span></span>|<span data-ttu-id="e725c-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e725c-146">String</span></span>|<span data-ttu-id="e725c-147">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="e725c-147">Operating System.</span></span>|
|<span data-ttu-id="e725c-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="e725c-148">osVersion</span></span>|<span data-ttu-id="e725c-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e725c-149">String</span></span>|<span data-ttu-id="e725c-150">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="e725c-150">OS Version.</span></span>|
|<span data-ttu-id="e725c-151">userId</span><span class="sxs-lookup"><span data-stu-id="e725c-151">userId</span></span>|<span data-ttu-id="e725c-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e725c-152">String</span></span>|<span data-ttu-id="e725c-153">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e725c-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="e725c-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="e725c-154">deviceId</span></span>|<span data-ttu-id="e725c-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e725c-155">String</span></span>|<span data-ttu-id="e725c-156">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e725c-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="e725c-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="e725c-157">enrollmentType</span></span>|[<span data-ttu-id="e725c-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="e725c-158">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="e725c-159">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="e725c-159">Type of the enrollment.</span></span> <span data-ttu-id="e725c-160">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="e725c-160">The possible values are `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, , or .</span></span>|
|<span data-ttu-id="e725c-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="e725c-161">failureCategory</span></span>|[<span data-ttu-id="e725c-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="e725c-162">deviceEnrollmentFailureReason values</span></span>](../resources/intune_troubleshooting_deviceenrollmentfailurereason.md)|<span data-ttu-id="e725c-163">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="e725c-163">Highlevel failure category.</span></span> <span data-ttu-id="e725c-164">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.</span><span class="sxs-lookup"><span data-stu-id="e725c-164">The possible values are `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, or .</span></span>|
|<span data-ttu-id="e725c-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="e725c-165">failureReason</span></span>|<span data-ttu-id="e725c-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e725c-166">String</span></span>|<span data-ttu-id="e725c-167">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="e725c-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="e725c-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="e725c-168">Response</span></span>
<span data-ttu-id="e725c-169">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e725c-169">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e725c-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e725c-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="e725c-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e725c-171">Request</span></span>
<span data-ttu-id="e725c-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e725c-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
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

### <a name="response"></a><span data-ttu-id="e725c-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="e725c-173">Response</span></span>
<span data-ttu-id="e725c-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e725c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



