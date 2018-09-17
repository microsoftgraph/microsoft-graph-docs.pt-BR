# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="b98ab-101">Criar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b98ab-101">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="b98ab-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b98ab-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b98ab-103">Cria um novo objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="b98ab-103">Create a new [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b98ab-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b98ab-104">Prerequisites</span></span>
<span data-ttu-id="b98ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b98ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b98ab-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b98ab-107">Permission type</span></span>|<span data-ttu-id="b98ab-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b98ab-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b98ab-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b98ab-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b98ab-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b98ab-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b98ab-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b98ab-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b98ab-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b98ab-112">Not supported.</span></span>|
|<span data-ttu-id="b98ab-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b98ab-113">Application</span></span>|<span data-ttu-id="b98ab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b98ab-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b98ab-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b98ab-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="b98ab-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b98ab-116">Request headers</span></span>
|<span data-ttu-id="b98ab-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b98ab-117">Header</span></span>|<span data-ttu-id="b98ab-118">Valor</span><span class="sxs-lookup"><span data-stu-id="b98ab-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b98ab-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="b98ab-119">Authorization</span></span>|<span data-ttu-id="b98ab-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="b98ab-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b98ab-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b98ab-121">Accept</span></span>|<span data-ttu-id="b98ab-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b98ab-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b98ab-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b98ab-123">Request body</span></span>
<span data-ttu-id="b98ab-124">No corpo da solicitação, forneça uma representação JSON do objeto enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="b98ab-124">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="b98ab-125">A tabela a seguir mostra as propriedades que são necessárias ao criar enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="b98ab-125">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="b98ab-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b98ab-126">Property</span></span>|<span data-ttu-id="b98ab-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b98ab-127">Type</span></span>|<span data-ttu-id="b98ab-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b98ab-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b98ab-129">id</span><span class="sxs-lookup"><span data-stu-id="b98ab-129">id</span></span>|<span data-ttu-id="b98ab-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b98ab-130">String</span></span>|<span data-ttu-id="b98ab-131">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b98ab-131">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b98ab-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="b98ab-132">eventDateTime</span></span>|<span data-ttu-id="b98ab-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b98ab-133">DateTimeOffset</span></span>|<span data-ttu-id="b98ab-134">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="b98ab-134">Time when the event occurred .</span></span> <span data-ttu-id="b98ab-135">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b98ab-135">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b98ab-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="b98ab-136">correlationId</span></span>|<span data-ttu-id="b98ab-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b98ab-137">String</span></span>|<span data-ttu-id="b98ab-138">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="b98ab-138">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="b98ab-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b98ab-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b98ab-140">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b98ab-140">managedDeviceIdentifier</span></span>|<span data-ttu-id="b98ab-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b98ab-141">String</span></span>|<span data-ttu-id="b98ab-142">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="b98ab-142">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="b98ab-143">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b98ab-143">operatingSystem</span></span>|<span data-ttu-id="b98ab-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b98ab-144">String</span></span>|<span data-ttu-id="b98ab-145">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="b98ab-145">Operating System.</span></span>|
|<span data-ttu-id="b98ab-146">osVersion</span><span class="sxs-lookup"><span data-stu-id="b98ab-146">osVersion</span></span>|<span data-ttu-id="b98ab-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b98ab-147">String</span></span>|<span data-ttu-id="b98ab-148">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="b98ab-148">OS Version.</span></span>|
|<span data-ttu-id="b98ab-149">userId</span><span class="sxs-lookup"><span data-stu-id="b98ab-149">userId</span></span>|<span data-ttu-id="b98ab-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b98ab-150">String</span></span>|<span data-ttu-id="b98ab-151">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b98ab-151">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="b98ab-152">deviceId</span><span class="sxs-lookup"><span data-stu-id="b98ab-152">deviceId</span></span>|<span data-ttu-id="b98ab-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b98ab-153">String</span></span>|<span data-ttu-id="b98ab-154">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b98ab-154">Azure AD device identifier.</span></span>|
|<span data-ttu-id="b98ab-155">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="b98ab-155">enrollmentType</span></span>|[<span data-ttu-id="b98ab-156">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="b98ab-156">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="b98ab-157">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="b98ab-157">Type of the enrollment.</span></span> <span data-ttu-id="b98ab-158">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="b98ab-158">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="b98ab-159">failureCategory</span><span class="sxs-lookup"><span data-stu-id="b98ab-159">failureCategory</span></span>|[<span data-ttu-id="b98ab-160">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="b98ab-160">deviceEnrollmentFailureReason values</span></span>](../resources/intune_troubleshooting_deviceenrollmentfailurereason.md)|<span data-ttu-id="b98ab-161">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="b98ab-161">Highlevel failure category.</span></span> <span data-ttu-id="b98ab-162">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="b98ab-162">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="b98ab-163">failureReason</span><span class="sxs-lookup"><span data-stu-id="b98ab-163">failureReason</span></span>|<span data-ttu-id="b98ab-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b98ab-164">String</span></span>|<span data-ttu-id="b98ab-165">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="b98ab-165">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="b98ab-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="b98ab-166">Response</span></span>
<span data-ttu-id="b98ab-167">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b98ab-167">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b98ab-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b98ab-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="b98ab-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b98ab-169">Request</span></span>
<span data-ttu-id="b98ab-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b98ab-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="b98ab-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="b98ab-171">Response</span></span>
<span data-ttu-id="b98ab-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b98ab-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




