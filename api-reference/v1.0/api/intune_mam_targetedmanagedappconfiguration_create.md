# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="bd898-101">Criar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd898-101">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="bd898-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bd898-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd898-103">Cria um novo objeto [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd898-103">Create a new [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd898-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bd898-104">Prerequisites</span></span>
<span data-ttu-id="bd898-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bd898-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bd898-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd898-107">Permission type</span></span>|<span data-ttu-id="bd898-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bd898-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd898-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd898-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bd898-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd898-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bd898-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd898-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd898-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd898-112">Not supported.</span></span>|
|<span data-ttu-id="bd898-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd898-113">Application</span></span>|<span data-ttu-id="bd898-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd898-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd898-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd898-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bd898-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd898-116">Request headers</span></span>
|<span data-ttu-id="bd898-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd898-117">Header</span></span>|<span data-ttu-id="bd898-118">Valor</span><span class="sxs-lookup"><span data-stu-id="bd898-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd898-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd898-119">Authorization</span></span>|<span data-ttu-id="bd898-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd898-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd898-121">Accept</span><span class="sxs-lookup"><span data-stu-id="bd898-121">Accept</span></span>|<span data-ttu-id="bd898-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bd898-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd898-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd898-123">Request body</span></span>
<span data-ttu-id="bd898-124">No corpo da solicitação, forneça uma representação JSON do objeto targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bd898-124">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="bd898-125">A tabela a seguir mostra as propriedades obrigatórias ao criar targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bd898-125">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="bd898-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd898-126">Property</span></span>|<span data-ttu-id="bd898-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd898-127">Type</span></span>|<span data-ttu-id="bd898-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd898-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd898-129">displayName</span><span class="sxs-lookup"><span data-stu-id="bd898-129">displayName</span></span>|<span data-ttu-id="bd898-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd898-130">String</span></span>|<span data-ttu-id="bd898-131">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="bd898-131">Policy display name.</span></span> <span data-ttu-id="bd898-132">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bd898-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bd898-133">description</span><span class="sxs-lookup"><span data-stu-id="bd898-133">description</span></span>|<span data-ttu-id="bd898-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd898-134">String</span></span>|<span data-ttu-id="bd898-135">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="bd898-135">The policy's description.</span></span> <span data-ttu-id="bd898-136">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bd898-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bd898-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd898-137">createdDateTime</span></span>|<span data-ttu-id="bd898-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd898-138">DateTimeOffset</span></span>|<span data-ttu-id="bd898-139">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="bd898-139">The date and time the policy was created.</span></span> <span data-ttu-id="bd898-140">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bd898-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bd898-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd898-141">lastModifiedDateTime</span></span>|<span data-ttu-id="bd898-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd898-142">DateTimeOffset</span></span>|<span data-ttu-id="bd898-143">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="bd898-143">Last time the policy was modified.</span></span> <span data-ttu-id="bd898-144">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bd898-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bd898-145">id</span><span class="sxs-lookup"><span data-stu-id="bd898-145">id</span></span>|<span data-ttu-id="bd898-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd898-146">String</span></span>|<span data-ttu-id="bd898-147">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bd898-147">Key of the entity.</span></span> <span data-ttu-id="bd898-148">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bd898-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bd898-149">version</span><span class="sxs-lookup"><span data-stu-id="bd898-149">version</span></span>|<span data-ttu-id="bd898-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd898-150">String</span></span>|<span data-ttu-id="bd898-151">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="bd898-151">Version of the entity.</span></span> <span data-ttu-id="bd898-152">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bd898-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bd898-153">customSettings</span><span class="sxs-lookup"><span data-stu-id="bd898-153">customSettings</span></span>|<span data-ttu-id="bd898-154">Coleção [keyValuePair](../resources/intune_mam_keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="bd898-154">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="bd898-155">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd898-155">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)</span></span>|
|<span data-ttu-id="bd898-156">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="bd898-156">deployedAppCount</span></span>|<span data-ttu-id="bd898-157">Int32</span><span class="sxs-lookup"><span data-stu-id="bd898-157">Int32</span></span>|<span data-ttu-id="bd898-158">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="bd898-158">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="bd898-159">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bd898-159">isAssigned</span></span>|<span data-ttu-id="bd898-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="bd898-160">Boolean</span></span>|<span data-ttu-id="bd898-161">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="bd898-161">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="bd898-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd898-162">Response</span></span>
<span data-ttu-id="bd898-163">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd898-163">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd898-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd898-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="bd898-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd898-165">Request</span></span>
<span data-ttu-id="bd898-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd898-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 388

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="bd898-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd898-167">Response</span></span>
<span data-ttu-id="bd898-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd898-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```



