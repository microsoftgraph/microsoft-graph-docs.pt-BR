# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="d70a2-101">Criar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="d70a2-101">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="d70a2-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d70a2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d70a2-103">Criar um novo objeto [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="d70a2-103">Create a new [plannerBucket](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d70a2-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d70a2-104">Prerequisites</span></span>
<span data-ttu-id="d70a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d70a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d70a2-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d70a2-107">Permission type</span></span>|<span data-ttu-id="d70a2-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d70a2-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d70a2-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d70a2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d70a2-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d70a2-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d70a2-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d70a2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d70a2-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d70a2-112">Not supported.</span></span>|
|<span data-ttu-id="d70a2-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d70a2-113">Application</span></span>|<span data-ttu-id="d70a2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d70a2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d70a2-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d70a2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="d70a2-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d70a2-116">Request headers</span></span>
|<span data-ttu-id="d70a2-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d70a2-117">Header</span></span>|<span data-ttu-id="d70a2-118">Valor</span><span class="sxs-lookup"><span data-stu-id="d70a2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d70a2-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="d70a2-119">Authorization</span></span>|<span data-ttu-id="d70a2-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d70a2-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d70a2-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d70a2-121">Accept</span></span>|<span data-ttu-id="d70a2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d70a2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d70a2-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d70a2-123">Request body</span></span>
<span data-ttu-id="d70a2-124">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="d70a2-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="d70a2-125">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="d70a2-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="d70a2-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d70a2-126">Property</span></span>|<span data-ttu-id="d70a2-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d70a2-127">Type</span></span>|<span data-ttu-id="d70a2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d70a2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d70a2-129">displayName</span><span class="sxs-lookup"><span data-stu-id="d70a2-129">displayName</span></span>|<span data-ttu-id="d70a2-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d70a2-130">String</span></span>|<span data-ttu-id="d70a2-131">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="d70a2-131">The friendly name of the picture provider.</span></span>|
|<span data-ttu-id="d70a2-132">fileHash</span><span class="sxs-lookup"><span data-stu-id="d70a2-132">fileHash</span></span>|<span data-ttu-id="d70a2-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d70a2-133">String</span></span>|<span data-ttu-id="d70a2-134">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="d70a2-134">SHA256 hash of the file</span></span>|
|<span data-ttu-id="d70a2-135">file</span><span class="sxs-lookup"><span data-stu-id="d70a2-135">file</span></span>|<span data-ttu-id="d70a2-136">Binária</span><span class="sxs-lookup"><span data-stu-id="d70a2-136">Binary</span></span>|<span data-ttu-id="d70a2-137">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="d70a2-137">File as a byte array</span></span>|
|<span data-ttu-id="d70a2-138">id</span><span class="sxs-lookup"><span data-stu-id="d70a2-138">id</span></span>|<span data-ttu-id="d70a2-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d70a2-139">String</span></span>|<span data-ttu-id="d70a2-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d70a2-140">Key of the setting.</span></span>|
|<span data-ttu-id="d70a2-141">version</span><span class="sxs-lookup"><span data-stu-id="d70a2-141">version</span></span>|<span data-ttu-id="d70a2-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d70a2-142">String</span></span>|<span data-ttu-id="d70a2-143">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="d70a2-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="d70a2-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d70a2-144">Response</span></span>
<span data-ttu-id="d70a2-145">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d70a2-145">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d70a2-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d70a2-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="d70a2-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d70a2-147">Request</span></span>
<span data-ttu-id="d70a2-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d70a2-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="d70a2-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d70a2-149">Response</span></span>
<span data-ttu-id="d70a2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d70a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
  "version": "Version value"
}
```



