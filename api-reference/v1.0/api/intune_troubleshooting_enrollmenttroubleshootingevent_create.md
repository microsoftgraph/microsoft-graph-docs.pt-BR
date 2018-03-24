# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="4f475-101">Criar enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="4f475-101">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="4f475-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4f475-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f475-103">Cria um novo objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="4f475-103">Create a new [plannerBucket](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f475-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f475-104">Prerequisites</span></span>
<span data-ttu-id="4f475-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f475-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4f475-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f475-107">Permission type</span></span>|<span data-ttu-id="4f475-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f475-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f475-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f475-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4f475-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f475-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4f475-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f475-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f475-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f475-112">Not supported.</span></span>|
|<span data-ttu-id="4f475-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f475-113">Application</span></span>|<span data-ttu-id="4f475-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f475-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f475-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f475-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="4f475-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f475-116">Request headers</span></span>
|<span data-ttu-id="4f475-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f475-117">Header</span></span>|<span data-ttu-id="4f475-118">Valor</span><span class="sxs-lookup"><span data-stu-id="4f475-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f475-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f475-119">Authorization</span></span>|<span data-ttu-id="4f475-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f475-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4f475-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f475-121">Accept</span></span>|<span data-ttu-id="4f475-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4f475-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f475-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f475-123">Request body</span></span>
<span data-ttu-id="4f475-124">No corpo da solicitação, forneça uma representação JSON do objeto enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="4f475-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="4f475-125">A tabela a seguir mostra as propriedades que são necessárias ao criar enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="4f475-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="4f475-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f475-126">Property</span></span>|<span data-ttu-id="4f475-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f475-127">Type</span></span>|<span data-ttu-id="4f475-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f475-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f475-129">id</span><span class="sxs-lookup"><span data-stu-id="4f475-129">id</span></span>|<span data-ttu-id="4f475-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f475-130">String</span></span>|<span data-ttu-id="4f475-131">UUID do objeto, herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="4f475-131">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="4f475-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="4f475-132">eventDateTime</span></span>|<span data-ttu-id="4f475-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f475-133">DateTimeOffset</span></span>|<span data-ttu-id="4f475-134">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="4f475-134">Time when the event occurred .</span></span> <span data-ttu-id="4f475-135">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="4f475-135">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="4f475-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="4f475-136">correlationId</span></span>|<span data-ttu-id="4f475-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f475-137">String</span></span>|<span data-ttu-id="4f475-138">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="4f475-138">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="4f475-139">Herdado de [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="4f475-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="4f475-140">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4f475-140">managedDeviceIdentifier</span></span>|<span data-ttu-id="4f475-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f475-141">String</span></span>|<span data-ttu-id="4f475-142">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="4f475-142">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="4f475-143">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="4f475-143">operatingSystem</span></span>|<span data-ttu-id="4f475-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f475-144">String</span></span>|<span data-ttu-id="4f475-145">Sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="4f475-145">Operating system</span></span>|
|<span data-ttu-id="4f475-146">osVersion</span><span class="sxs-lookup"><span data-stu-id="4f475-146">osVersion</span></span>|<span data-ttu-id="4f475-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f475-147">String</span></span>|<span data-ttu-id="4f475-148">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="4f475-148">OS Version.</span></span>|
|<span data-ttu-id="4f475-149">userId</span><span class="sxs-lookup"><span data-stu-id="4f475-149">userId</span></span>|<span data-ttu-id="4f475-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f475-150">String</span></span>|<span data-ttu-id="4f475-151">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4f475-151">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="4f475-152">deviceId</span><span class="sxs-lookup"><span data-stu-id="4f475-152">deviceId</span></span>|<span data-ttu-id="4f475-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f475-153">String</span></span>|<span data-ttu-id="4f475-154">Identificador do dispositivo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4f475-154">Azure AD device identifier.</span></span>|
|<span data-ttu-id="4f475-155">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="4f475-155">enrollmentType</span></span>|<span data-ttu-id="4f475-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f475-156">String</span></span>|<span data-ttu-id="4f475-157">Tipo do registro.</span><span class="sxs-lookup"><span data-stu-id="4f475-157">Type of the enrollment.</span></span> <span data-ttu-id="4f475-158">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="4f475-158">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="4f475-159">failureCategory</span><span class="sxs-lookup"><span data-stu-id="4f475-159">failureCategory</span></span>|<span data-ttu-id="4f475-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f475-160">String</span></span>|<span data-ttu-id="4f475-161">Categoria de falha de alto nível.</span><span class="sxs-lookup"><span data-stu-id="4f475-161">Highlevel failure category.</span></span> <span data-ttu-id="4f475-162">Os valores possíveis são: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.</span><span class="sxs-lookup"><span data-stu-id="4f475-162">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.</span></span>|
|<span data-ttu-id="4f475-163">failureReason</span><span class="sxs-lookup"><span data-stu-id="4f475-163">failureReason</span></span>|<span data-ttu-id="4f475-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f475-164">String</span></span>|<span data-ttu-id="4f475-165">Motivo detalhado da falha.</span><span class="sxs-lookup"><span data-stu-id="4f475-165">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="4f475-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f475-166">Response</span></span>
<span data-ttu-id="4f475-167">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f475-167">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f475-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f475-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f475-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f475-169">Request</span></span>
<span data-ttu-id="4f475-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f475-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="4f475-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f475-171">Response</span></span>
<span data-ttu-id="4f475-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f475-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



