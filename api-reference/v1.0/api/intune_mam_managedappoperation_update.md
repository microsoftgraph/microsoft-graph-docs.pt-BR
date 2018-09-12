# <a name="update-managedappoperation"></a><span data-ttu-id="20be9-101">Atualizar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="20be9-101">Update managedAppOperation</span></span>

> <span data-ttu-id="20be9-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="20be9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20be9-103">Atualizar as propriedades de um objeto [managedAppOperation](../resources/intune_mam_managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="20be9-103">Update the properties of a [managedAppOperation](../resources/intune_mam_managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20be9-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20be9-104">Prerequisites</span></span>
<span data-ttu-id="20be9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="20be9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="20be9-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20be9-107">Permission type</span></span>|<span data-ttu-id="20be9-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="20be9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20be9-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20be9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="20be9-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20be9-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="20be9-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20be9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20be9-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20be9-112">Not supported.</span></span>|
|<span data-ttu-id="20be9-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20be9-113">Application</span></span>|<span data-ttu-id="20be9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20be9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20be9-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20be9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="20be9-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20be9-116">Request headers</span></span>
|<span data-ttu-id="20be9-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20be9-117">Header</span></span>|<span data-ttu-id="20be9-118">Valor</span><span class="sxs-lookup"><span data-stu-id="20be9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20be9-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="20be9-119">Authorization</span></span>|<span data-ttu-id="20be9-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="20be9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20be9-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="20be9-121">Accept</span></span>|<span data-ttu-id="20be9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="20be9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20be9-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20be9-123">Request body</span></span>
<span data-ttu-id="20be9-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppOperation](../resources/intune_mam_managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="20be9-124">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune_mam_managedappoperation.md) object.</span></span>

<span data-ttu-id="20be9-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppOperation](../resources/intune_mam_managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="20be9-125">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune_mam_managedappoperation.md).</span></span>

|<span data-ttu-id="20be9-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20be9-126">Property</span></span>|<span data-ttu-id="20be9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="20be9-127">Type</span></span>|<span data-ttu-id="20be9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="20be9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20be9-129">displayName</span><span class="sxs-lookup"><span data-stu-id="20be9-129">displayName</span></span>|<span data-ttu-id="20be9-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20be9-130">String</span></span>|<span data-ttu-id="20be9-131">O nome da operação.</span><span class="sxs-lookup"><span data-stu-id="20be9-131">The operation name.</span></span>|
|<span data-ttu-id="20be9-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20be9-132">lastModifiedDateTime</span></span>|<span data-ttu-id="20be9-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20be9-133">DateTimeOffset</span></span>|<span data-ttu-id="20be9-134">Última vez em que a operação de aplicativo foi modificada.</span><span class="sxs-lookup"><span data-stu-id="20be9-134">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="20be9-135">state</span><span class="sxs-lookup"><span data-stu-id="20be9-135">state</span></span>|<span data-ttu-id="20be9-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20be9-136">String</span></span>|<span data-ttu-id="20be9-137">O estado atual da operação</span><span class="sxs-lookup"><span data-stu-id="20be9-137">The current state of the operation</span></span>|
|<span data-ttu-id="20be9-138">id</span><span class="sxs-lookup"><span data-stu-id="20be9-138">id</span></span>|<span data-ttu-id="20be9-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20be9-139">String</span></span>|<span data-ttu-id="20be9-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="20be9-140">Key of the entity.</span></span>|
|<span data-ttu-id="20be9-141">version</span><span class="sxs-lookup"><span data-stu-id="20be9-141">version</span></span>|<span data-ttu-id="20be9-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20be9-142">String</span></span>|<span data-ttu-id="20be9-143">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="20be9-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="20be9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="20be9-144">Response</span></span>
<span data-ttu-id="20be9-145">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppOperation](../resources/intune_mam_managedappoperation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20be9-145">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune_mam_managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20be9-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20be9-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="20be9-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20be9-147">Request</span></span>
<span data-ttu-id="20be9-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20be9-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 165

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="20be9-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="20be9-149">Response</span></span>
<span data-ttu-id="20be9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20be9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
  "version": "Version value"
}
```








