# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="1a04e-101">Criar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="1a04e-101">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="1a04e-102">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1a04e-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a04e-103">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1a04e-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a04e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1a04e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a04e-105">Cria um novo objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="1a04e-105">Create a new [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a04e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1a04e-106">Prerequisites</span></span>
<span data-ttu-id="1a04e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1a04e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1a04e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a04e-109">Permission type</span></span>|<span data-ttu-id="1a04e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1a04e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a04e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a04e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1a04e-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a04e-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1a04e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a04e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a04e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a04e-114">Not supported.</span></span>|
|<span data-ttu-id="1a04e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a04e-115">Application</span></span>|<span data-ttu-id="1a04e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a04e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a04e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a04e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="1a04e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a04e-118">Request headers</span></span>
|<span data-ttu-id="1a04e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1a04e-119">Header</span></span>|<span data-ttu-id="1a04e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1a04e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a04e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a04e-121">Authorization</span></span>|<span data-ttu-id="1a04e-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="1a04e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a04e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1a04e-123">Accept</span></span>|<span data-ttu-id="1a04e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1a04e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a04e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a04e-125">Request body</span></span>
<span data-ttu-id="1a04e-126">No corpo da solicitação, forneça uma representação JSON do objeto enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="1a04e-126">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="1a04e-127">A tabela a seguir mostra as propriedades que são necessárias ao criar enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="1a04e-127">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="1a04e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a04e-128">Property</span></span>|<span data-ttu-id="1a04e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a04e-129">Type</span></span>|<span data-ttu-id="1a04e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a04e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a04e-131">id</span><span class="sxs-lookup"><span data-stu-id="1a04e-131">id</span></span>|<span data-ttu-id="1a04e-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a04e-132">String</span></span>|<span data-ttu-id="1a04e-133">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="1a04e-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="1a04e-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="1a04e-134">eventDateTime</span></span>|<span data-ttu-id="1a04e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a04e-135">DateTimeOffset</span></span>|<span data-ttu-id="1a04e-136">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="1a04e-136">Time when the event occurred .</span></span> <span data-ttu-id="1a04e-137">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="1a04e-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="1a04e-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="1a04e-138">correlationId</span></span>|<span data-ttu-id="1a04e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a04e-139">String</span></span>|<span data-ttu-id="1a04e-140">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="1a04e-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="1a04e-141">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="1a04e-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="1a04e-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1a04e-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="1a04e-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a04e-143">String</span></span>|<span data-ttu-id="1a04e-144">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="1a04e-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="1a04e-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="1a04e-145">operatingSystem</span></span>|<span data-ttu-id="1a04e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a04e-146">String</span></span>|<span data-ttu-id="1a04e-147">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="1a04e-147">Operating System.</span></span>|
|<span data-ttu-id="1a04e-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="1a04e-148">osVersion</span></span>|<span data-ttu-id="1a04e-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a04e-149">String</span></span>|<span data-ttu-id="1a04e-150">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="1a04e-150">OS Version.</span></span>|
|<span data-ttu-id="1a04e-151">userId</span><span class="sxs-lookup"><span data-stu-id="1a04e-151">userId</span></span>|<span data-ttu-id="1a04e-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a04e-152">String</span></span>|<span data-ttu-id="1a04e-153">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1a04e-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="1a04e-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="1a04e-154">deviceId</span></span>|<span data-ttu-id="1a04e-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a04e-155">String</span></span>|<span data-ttu-id="1a04e-156">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1a04e-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="1a04e-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="1a04e-157">enrollmentType</span></span>|[<span data-ttu-id="1a04e-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="1a04e-158">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="1a04e-159">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="1a04e-159">Type of the enrollment.</span></span> <span data-ttu-id="1a04e-160">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="1a04e-160">The possible values are `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, , or .</span></span>|
|<span data-ttu-id="1a04e-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="1a04e-161">failureCategory</span></span>|[<span data-ttu-id="1a04e-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="1a04e-162">deviceEnrollmentFailureReason values</span></span>](../resources/intune_troubleshooting_deviceenrollmentfailurereason.md)|<span data-ttu-id="1a04e-163">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="1a04e-163">Highlevel failure category.</span></span> <span data-ttu-id="1a04e-164">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.</span><span class="sxs-lookup"><span data-stu-id="1a04e-164">The possible values are `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, or .</span></span>|
|<span data-ttu-id="1a04e-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="1a04e-165">failureReason</span></span>|<span data-ttu-id="1a04e-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a04e-166">String</span></span>|<span data-ttu-id="1a04e-167">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="1a04e-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="1a04e-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a04e-168">Response</span></span>
<span data-ttu-id="1a04e-169">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a04e-169">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a04e-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a04e-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="1a04e-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a04e-171">Request</span></span>
<span data-ttu-id="1a04e-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a04e-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 509

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
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

### <a name="response"></a><span data-ttu-id="1a04e-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a04e-173">Response</span></span>
<span data-ttu-id="1a04e-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a04e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



