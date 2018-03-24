# <a name="create-managedappoperation"></a><span data-ttu-id="97862-101">Criar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="97862-101">Create managedAppOperation</span></span>

> <span data-ttu-id="97862-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="97862-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97862-103">Criar um novo objeto [managedAppOperation](../resources/intune_mam_managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="97862-103">Create a new [plannerBucket](../resources/intune_mam_managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97862-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97862-104">Prerequisites</span></span>
<span data-ttu-id="97862-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97862-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97862-107">Permission type</span></span>|<span data-ttu-id="97862-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97862-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97862-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97862-109">Delegated (work or school account)</span></span>|<span data-ttu-id="97862-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97862-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="97862-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97862-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97862-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97862-112">Not supported.</span></span>|
|<span data-ttu-id="97862-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97862-113">Application</span></span>|<span data-ttu-id="97862-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97862-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97862-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97862-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="97862-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97862-116">Request headers</span></span>
|<span data-ttu-id="97862-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97862-117">Header</span></span>|<span data-ttu-id="97862-118">Valor</span><span class="sxs-lookup"><span data-stu-id="97862-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97862-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="97862-119">Authorization</span></span>|<span data-ttu-id="97862-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97862-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="97862-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97862-121">Accept</span></span>|<span data-ttu-id="97862-122">application/json</span><span class="sxs-lookup"><span data-stu-id="97862-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97862-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97862-123">Request body</span></span>
<span data-ttu-id="97862-124">No corpo da solicitação, forneça uma representação JSON do objeto managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="97862-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="97862-125">A tabela a seguir mostra as propriedades que são necessárias ao criar managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="97862-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="97862-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97862-126">Property</span></span>|<span data-ttu-id="97862-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="97862-127">Type</span></span>|<span data-ttu-id="97862-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="97862-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97862-129">displayName</span><span class="sxs-lookup"><span data-stu-id="97862-129">displayName</span></span>|<span data-ttu-id="97862-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97862-130">String</span></span>|<span data-ttu-id="97862-131">O nome da operação.</span><span class="sxs-lookup"><span data-stu-id="97862-131">The operation name.</span></span>|
|<span data-ttu-id="97862-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97862-132">lastModifiedDateTime</span></span>|<span data-ttu-id="97862-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97862-133">DateTimeOffset</span></span>|<span data-ttu-id="97862-134">Última vez em que a operação de aplicativo foi modificada.</span><span class="sxs-lookup"><span data-stu-id="97862-134">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="97862-135">state</span><span class="sxs-lookup"><span data-stu-id="97862-135">state</span></span>|<span data-ttu-id="97862-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97862-136">String</span></span>|<span data-ttu-id="97862-137">O estado atual da operação</span><span class="sxs-lookup"><span data-stu-id="97862-137">The current state of the operation</span></span>|
|<span data-ttu-id="97862-138">id</span><span class="sxs-lookup"><span data-stu-id="97862-138">id</span></span>|<span data-ttu-id="97862-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97862-139">String</span></span>|<span data-ttu-id="97862-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="97862-140">Key of the setting.</span></span>|
|<span data-ttu-id="97862-141">version</span><span class="sxs-lookup"><span data-stu-id="97862-141">version</span></span>|<span data-ttu-id="97862-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97862-142">String</span></span>|<span data-ttu-id="97862-143">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="97862-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="97862-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="97862-144">Response</span></span>
<span data-ttu-id="97862-145">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedAppOperation](../resources/intune_mam_managedappoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97862-145">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_mam_managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97862-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97862-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="97862-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97862-147">Request</span></span>
<span data-ttu-id="97862-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97862-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 223

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="97862-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="97862-149">Response</span></span>
<span data-ttu-id="97862-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97862-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



