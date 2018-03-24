# <a name="update-deviceinstallstate"></a><span data-ttu-id="86b3c-101">Atualizar deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="86b3c-101">Update deviceInstallState</span></span>

> <span data-ttu-id="86b3c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="86b3c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86b3c-103">Atualizar as propriedades de um objeto [deviceInstallState](../resources/intune_books_deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="86b3c-103">Update the properties of a [calendar](../resources/intune_books_deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86b3c-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86b3c-104">Prerequisites</span></span>
<span data-ttu-id="86b3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="86b3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="86b3c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86b3c-107">Permission type</span></span>|<span data-ttu-id="86b3c-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86b3c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86b3c-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86b3c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="86b3c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86b3c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="86b3c-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86b3c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86b3c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86b3c-112">Not supported.</span></span>|
|<span data-ttu-id="86b3c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86b3c-113">Application</span></span>|<span data-ttu-id="86b3c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86b3c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86b3c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86b3c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="86b3c-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86b3c-116">Request headers</span></span>
|<span data-ttu-id="86b3c-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86b3c-117">Header</span></span>|<span data-ttu-id="86b3c-118">Valor</span><span class="sxs-lookup"><span data-stu-id="86b3c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86b3c-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="86b3c-119">Authorization</span></span>|<span data-ttu-id="86b3c-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86b3c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="86b3c-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86b3c-121">Accept</span></span>|<span data-ttu-id="86b3c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="86b3c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86b3c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86b3c-123">Request body</span></span>
<span data-ttu-id="86b3c-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceInstallState](../resources/intune_books_deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="86b3c-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_books_deviceinstallstate.md) object.</span></span>

<span data-ttu-id="86b3c-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceInstallState](../resources/intune_books_deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="86b3c-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="86b3c-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86b3c-126">Property</span></span>|<span data-ttu-id="86b3c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="86b3c-127">Type</span></span>|<span data-ttu-id="86b3c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="86b3c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86b3c-129">id</span><span class="sxs-lookup"><span data-stu-id="86b3c-129">id</span></span>|<span data-ttu-id="86b3c-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86b3c-130">String</span></span>|<span data-ttu-id="86b3c-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="86b3c-131">Key of the setting.</span></span>|
|<span data-ttu-id="86b3c-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="86b3c-132">deviceName</span></span>|<span data-ttu-id="86b3c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86b3c-133">String</span></span>|<span data-ttu-id="86b3c-134">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="86b3c-134">Device name.</span></span>|
|<span data-ttu-id="86b3c-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="86b3c-135">deviceId</span></span>|<span data-ttu-id="86b3c-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86b3c-136">String</span></span>|<span data-ttu-id="86b3c-137">ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="86b3c-137">Device Id.</span></span>|
|<span data-ttu-id="86b3c-138">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="86b3c-138">lastSyncDateTime</span></span>|<span data-ttu-id="86b3c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86b3c-139">DateTimeOffset</span></span>|<span data-ttu-id="86b3c-140">Última sincronização de data e hora.</span><span class="sxs-lookup"><span data-stu-id="86b3c-140">Last sync date and time.</span></span>|
|<span data-ttu-id="86b3c-141">installState</span><span class="sxs-lookup"><span data-stu-id="86b3c-141">installState</span></span>|<span data-ttu-id="86b3c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86b3c-142">String</span></span>|<span data-ttu-id="86b3c-143">O estado de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="86b3c-143">The install state of the eBook.</span></span> <span data-ttu-id="86b3c-144">Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="86b3c-144">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="86b3c-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="86b3c-145">Error.code</span></span>|<span data-ttu-id="86b3c-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86b3c-146">String</span></span>|<span data-ttu-id="86b3c-147">O código de erro de falhas de instalação.</span><span class="sxs-lookup"><span data-stu-id="86b3c-147">The error code for install failures.</span></span>|
|<span data-ttu-id="86b3c-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="86b3c-148">osVersion</span></span>|<span data-ttu-id="86b3c-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86b3c-149">String</span></span>|<span data-ttu-id="86b3c-150">Versão do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="86b3c-150">OS Version.</span></span>|
|<span data-ttu-id="86b3c-151">osDescription</span><span class="sxs-lookup"><span data-stu-id="86b3c-151">osDescription</span></span>|<span data-ttu-id="86b3c-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86b3c-152">String</span></span>|<span data-ttu-id="86b3c-153">Descrição do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="86b3c-153">OS Description.</span></span>|
|<span data-ttu-id="86b3c-154">userName</span><span class="sxs-lookup"><span data-stu-id="86b3c-154">UserName</span></span>|<span data-ttu-id="86b3c-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86b3c-155">String</span></span>|<span data-ttu-id="86b3c-156">Nome de usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="86b3c-156">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="86b3c-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="86b3c-157">Response</span></span>
<span data-ttu-id="86b3c-158">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [deviceInstallState](../resources/intune_books_deviceinstallstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86b3c-158">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_books_deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86b3c-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86b3c-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="86b3c-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86b3c-160">Request</span></span>
<span data-ttu-id="86b3c-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86b3c-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
Content-type: application/json
Content-length: 317

{
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### <a name="response"></a><span data-ttu-id="86b3c-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="86b3c-162">Response</span></span>
<span data-ttu-id="86b3c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86b3c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```



