# <a name="create-mobileappcontentfile"></a><span data-ttu-id="cb46c-101">Criar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cb46c-101">Create mobileAppContentFile</span></span>

> <span data-ttu-id="cb46c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cb46c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb46c-103">Criar um novo objeto [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="cb46c-103">Create a new [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb46c-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cb46c-104">Prerequisites</span></span>
<span data-ttu-id="cb46c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cb46c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cb46c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb46c-107">Permission type</span></span>|<span data-ttu-id="cb46c-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cb46c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb46c-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb46c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cb46c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb46c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cb46c-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb46c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb46c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb46c-112">Not supported.</span></span>|
|<span data-ttu-id="cb46c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb46c-113">Application</span></span>|<span data-ttu-id="cb46c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb46c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb46c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb46c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="cb46c-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb46c-116">Request headers</span></span>
|<span data-ttu-id="cb46c-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb46c-117">Header</span></span>|<span data-ttu-id="cb46c-118">Valor</span><span class="sxs-lookup"><span data-stu-id="cb46c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb46c-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb46c-119">Authorization</span></span>|<span data-ttu-id="cb46c-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="cb46c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb46c-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cb46c-121">Accept</span></span>|<span data-ttu-id="cb46c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cb46c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb46c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb46c-123">Request body</span></span>
<span data-ttu-id="cb46c-124">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="cb46c-124">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="cb46c-125">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="cb46c-125">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="cb46c-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb46c-126">Property</span></span>|<span data-ttu-id="cb46c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb46c-127">Type</span></span>|<span data-ttu-id="cb46c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb46c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb46c-129">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="cb46c-129">azureStorageUri</span></span>|<span data-ttu-id="cb46c-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb46c-130">String</span></span>|<span data-ttu-id="cb46c-131">O URI de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="cb46c-131">The Azure Storage URI.</span></span>|
|<span data-ttu-id="cb46c-132">isCommitted</span><span class="sxs-lookup"><span data-stu-id="cb46c-132">isCommitted</span></span>|<span data-ttu-id="cb46c-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="cb46c-133">Boolean</span></span>|<span data-ttu-id="cb46c-134">Um valor que indica se o arquivo tem está confirmado.</span><span class="sxs-lookup"><span data-stu-id="cb46c-134">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="cb46c-135">id</span><span class="sxs-lookup"><span data-stu-id="cb46c-135">id</span></span>|<span data-ttu-id="cb46c-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb46c-136">String</span></span>|<span data-ttu-id="cb46c-137">A ID do arquivo.</span><span class="sxs-lookup"><span data-stu-id="cb46c-137">The File Id.</span></span>|
|<span data-ttu-id="cb46c-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb46c-138">createdDateTime</span></span>|<span data-ttu-id="cb46c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb46c-139">DateTimeOffset</span></span>|<span data-ttu-id="cb46c-140">A hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="cb46c-140">The time the file was created.</span></span>|
|<span data-ttu-id="cb46c-141">name</span><span class="sxs-lookup"><span data-stu-id="cb46c-141">name</span></span>|<span data-ttu-id="cb46c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb46c-142">String</span></span>|<span data-ttu-id="cb46c-143">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="cb46c-143">the file name.</span></span>|
|<span data-ttu-id="cb46c-144">size</span><span class="sxs-lookup"><span data-stu-id="cb46c-144">size</span></span>|<span data-ttu-id="cb46c-145">Int64</span><span class="sxs-lookup"><span data-stu-id="cb46c-145">Int64</span></span>|<span data-ttu-id="cb46c-146">O tamanho do arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="cb46c-146">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="cb46c-147">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="cb46c-147">sizeEncrypted</span></span>|<span data-ttu-id="cb46c-148">Int64</span><span class="sxs-lookup"><span data-stu-id="cb46c-148">Int64</span></span>|<span data-ttu-id="cb46c-149">O tamanho do arquivo após a criptografia.</span><span class="sxs-lookup"><span data-stu-id="cb46c-149">The size of the file after encryption.</span></span>|
|<span data-ttu-id="cb46c-150">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cb46c-150">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="cb46c-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb46c-151">DateTimeOffset</span></span>|<span data-ttu-id="cb46c-152">A hora de expiração do URI do armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="cb46c-152">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="cb46c-153">manifest</span><span class="sxs-lookup"><span data-stu-id="cb46c-153">manifest</span></span>|<span data-ttu-id="cb46c-154">Binária</span><span class="sxs-lookup"><span data-stu-id="cb46c-154">Binary</span></span>|<span data-ttu-id="cb46c-155">As informações do manifesto.</span><span class="sxs-lookup"><span data-stu-id="cb46c-155">The manifest information.</span></span>|
|<span data-ttu-id="cb46c-156">uploadState</span><span class="sxs-lookup"><span data-stu-id="cb46c-156">uploadState</span></span>|[<span data-ttu-id="cb46c-157">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="cb46c-157">mobileAppContentFileUploadState</span></span>](../resources/intune_apps_mobileappcontentfileuploadstate.md)|<span data-ttu-id="cb46c-158">O estado da solicitação de carregamento atual.</span><span class="sxs-lookup"><span data-stu-id="cb46c-158">The state of the current upload request.</span></span> <span data-ttu-id="cb46c-159">Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="cb46c-159">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="cb46c-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb46c-160">Response</span></span>
<span data-ttu-id="cb46c-161">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb46c-161">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb46c-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb46c-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="cb46c-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb46c-163">Request</span></span>
<span data-ttu-id="cb46c-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb46c-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```

### <a name="response"></a><span data-ttu-id="cb46c-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb46c-165">Response</span></span>
<span data-ttu-id="cb46c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb46c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 450

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```








