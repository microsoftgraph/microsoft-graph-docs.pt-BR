# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="4bd5e-101">Atualizar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="4bd5e-101">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="4bd5e-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4bd5e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4bd5e-103">Atualizar as propriedades de um objeto [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="4bd5e-103">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4bd5e-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4bd5e-104">Prerequisites</span></span>
<span data-ttu-id="4bd5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4bd5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4bd5e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bd5e-107">Permission type</span></span>|<span data-ttu-id="4bd5e-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4bd5e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bd5e-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bd5e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4bd5e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bd5e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4bd5e-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bd5e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bd5e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bd5e-112">Not supported.</span></span>|
|<span data-ttu-id="4bd5e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bd5e-113">Application</span></span>|<span data-ttu-id="4bd5e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bd5e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bd5e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bd5e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="request-headers"></a><span data-ttu-id="4bd5e-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bd5e-116">Request headers</span></span>
|<span data-ttu-id="4bd5e-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4bd5e-117">Header</span></span>|<span data-ttu-id="4bd5e-118">Valor</span><span class="sxs-lookup"><span data-stu-id="4bd5e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bd5e-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bd5e-119">Authorization</span></span>|<span data-ttu-id="4bd5e-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bd5e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bd5e-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4bd5e-121">Accept</span></span>|<span data-ttu-id="4bd5e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4bd5e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bd5e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bd5e-123">Request body</span></span>
<span data-ttu-id="4bd5e-124">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="4bd5e-124">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="4bd5e-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="4bd5e-125">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="4bd5e-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bd5e-126">Property</span></span>|<span data-ttu-id="4bd5e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bd5e-127">Type</span></span>|<span data-ttu-id="4bd5e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bd5e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bd5e-129">displayName</span><span class="sxs-lookup"><span data-stu-id="4bd5e-129">displayName</span></span>|<span data-ttu-id="4bd5e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4bd5e-130">String</span></span>|<span data-ttu-id="4bd5e-131">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="4bd5e-131">The friendly name</span></span>|
|<span data-ttu-id="4bd5e-132">fileHash</span><span class="sxs-lookup"><span data-stu-id="4bd5e-132">fileHash</span></span>|<span data-ttu-id="4bd5e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4bd5e-133">String</span></span>|<span data-ttu-id="4bd5e-134">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="4bd5e-134">SHA256 hash of the file</span></span>|
|<span data-ttu-id="4bd5e-135">file</span><span class="sxs-lookup"><span data-stu-id="4bd5e-135">file</span></span>|<span data-ttu-id="4bd5e-136">Binária</span><span class="sxs-lookup"><span data-stu-id="4bd5e-136">Binary</span></span>|<span data-ttu-id="4bd5e-137">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="4bd5e-137">File as a byte array</span></span>|
|<span data-ttu-id="4bd5e-138">id</span><span class="sxs-lookup"><span data-stu-id="4bd5e-138">id</span></span>|<span data-ttu-id="4bd5e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4bd5e-139">String</span></span>|<span data-ttu-id="4bd5e-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4bd5e-140">Key of the entity.</span></span>|
|<span data-ttu-id="4bd5e-141">version</span><span class="sxs-lookup"><span data-stu-id="4bd5e-141">version</span></span>|<span data-ttu-id="4bd5e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4bd5e-142">String</span></span>|<span data-ttu-id="4bd5e-143">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="4bd5e-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="4bd5e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bd5e-144">Response</span></span>
<span data-ttu-id="4bd5e-145">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bd5e-145">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bd5e-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bd5e-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="4bd5e-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bd5e-147">Request</span></span>
<span data-ttu-id="4bd5e-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bd5e-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
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

### <a name="response"></a><span data-ttu-id="4bd5e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bd5e-149">Response</span></span>
<span data-ttu-id="4bd5e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bd5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



