# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="0fa33-101">Atualizar importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="0fa33-101">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="0fa33-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0fa33-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0fa33-103">Atualizar as propriedades de um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md).</span><span class="sxs-lookup"><span data-stu-id="0fa33-103">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0fa33-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0fa33-104">Prerequisites</span></span>
<span data-ttu-id="0fa33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0fa33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0fa33-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fa33-107">Permission type</span></span>|<span data-ttu-id="0fa33-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0fa33-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fa33-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fa33-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0fa33-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fa33-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0fa33-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fa33-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fa33-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fa33-112">Not supported.</span></span>|
|<span data-ttu-id="0fa33-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fa33-113">Application</span></span>|<span data-ttu-id="0fa33-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fa33-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fa33-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fa33-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="0fa33-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa33-116">Request headers</span></span>
|<span data-ttu-id="0fa33-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fa33-117">Header</span></span>|<span data-ttu-id="0fa33-118">Valor</span><span class="sxs-lookup"><span data-stu-id="0fa33-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fa33-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fa33-119">Authorization</span></span>|<span data-ttu-id="0fa33-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="0fa33-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fa33-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0fa33-121">Accept</span></span>|<span data-ttu-id="0fa33-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0fa33-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fa33-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa33-123">Request body</span></span>
<span data-ttu-id="0fa33-124">No corpo da solicitação, forneça uma representação JSON do objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="0fa33-124">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="0fa33-125">A tabela a seguir mostra as propriedades que são necessárias ao criar o [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md).</span><span class="sxs-lookup"><span data-stu-id="0fa33-125">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="0fa33-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0fa33-126">Property</span></span>|<span data-ttu-id="0fa33-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fa33-127">Type</span></span>|<span data-ttu-id="0fa33-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fa33-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fa33-129">id</span><span class="sxs-lookup"><span data-stu-id="0fa33-129">id</span></span>|<span data-ttu-id="0fa33-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fa33-130">String</span></span>|<span data-ttu-id="0fa33-131">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="0fa33-131">The GUID for the object</span></span>|
|<span data-ttu-id="0fa33-132">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="0fa33-132">createdDateTimeUtc</span></span>|<span data-ttu-id="0fa33-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fa33-133">DateTimeOffset</span></span>|<span data-ttu-id="0fa33-134">DateTime quando a entidade é criada.</span><span class="sxs-lookup"><span data-stu-id="0fa33-134">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="0fa33-135">status</span><span class="sxs-lookup"><span data-stu-id="0fa33-135">status</span></span>|[<span data-ttu-id="0fa33-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="0fa33-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="0fa33-137">Status de carregamento.</span><span class="sxs-lookup"><span data-stu-id="0fa33-137">Upload status.</span></span> <span data-ttu-id="0fa33-138">Os valores possíveis são: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="0fa33-138">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="0fa33-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fa33-139">Response</span></span>
<span data-ttu-id="0fa33-140">Se bem-sucedido, este método retorna uma `200 OK` resposta de código e um objeto atualizado [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fa33-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fa33-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fa33-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="0fa33-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa33-142">Request</span></span>
<span data-ttu-id="0fa33-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fa33-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 89

{
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="0fa33-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fa33-144">Response</span></span>
<span data-ttu-id="0fa33-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fa33-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```








