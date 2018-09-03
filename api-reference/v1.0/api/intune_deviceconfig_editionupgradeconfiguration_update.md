# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="64354-101">Atualizar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="64354-101">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="64354-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="64354-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64354-103">Atualizar as propriedades de um objeto [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64354-103">Update the properties of a [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="64354-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64354-104">Prerequisites</span></span>
<span data-ttu-id="64354-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="64354-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="64354-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64354-107">Permission type</span></span>|<span data-ttu-id="64354-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64354-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64354-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64354-109">Delegated (work or school account)</span></span>|<span data-ttu-id="64354-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64354-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64354-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64354-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64354-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64354-112">Not supported.</span></span>|
|<span data-ttu-id="64354-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64354-113">Application</span></span>|<span data-ttu-id="64354-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64354-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64354-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64354-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="64354-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64354-116">Request headers</span></span>
|<span data-ttu-id="64354-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64354-117">Header</span></span>|<span data-ttu-id="64354-118">Valor</span><span class="sxs-lookup"><span data-stu-id="64354-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64354-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="64354-119">Authorization</span></span>|<span data-ttu-id="64354-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="64354-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64354-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64354-121">Accept</span></span>|<span data-ttu-id="64354-122">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="64354-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64354-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64354-123">Request body</span></span>
<span data-ttu-id="64354-124">No corpo da solicitação, forneça uma representação JSON do objeto [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64354-124">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="64354-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64354-125">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="64354-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64354-126">Property</span></span>|<span data-ttu-id="64354-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="64354-127">Type</span></span>|<span data-ttu-id="64354-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="64354-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64354-129">id</span><span class="sxs-lookup"><span data-stu-id="64354-129">id</span></span>|<span data-ttu-id="64354-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64354-130">String</span></span>|<span data-ttu-id="64354-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="64354-131">Key of the entity.</span></span> <span data-ttu-id="64354-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64354-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64354-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64354-133">lastModifiedDateTime</span></span>|<span data-ttu-id="64354-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64354-134">DateTimeOffset</span></span>|<span data-ttu-id="64354-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="64354-135">DateTime the object was last modified.</span></span> <span data-ttu-id="64354-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64354-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64354-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64354-137">createdDateTime</span></span>|<span data-ttu-id="64354-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64354-138">DateTimeOffset</span></span>|<span data-ttu-id="64354-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="64354-139">DateTime the object was created.</span></span> <span data-ttu-id="64354-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64354-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64354-141">description</span><span class="sxs-lookup"><span data-stu-id="64354-141">description</span></span>|<span data-ttu-id="64354-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64354-142">String</span></span>|<span data-ttu-id="64354-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64354-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="64354-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64354-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64354-145">displayName</span><span class="sxs-lookup"><span data-stu-id="64354-145">displayName</span></span>|<span data-ttu-id="64354-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64354-146">String</span></span>|<span data-ttu-id="64354-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64354-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="64354-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64354-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64354-149">version</span><span class="sxs-lookup"><span data-stu-id="64354-149">version</span></span>|<span data-ttu-id="64354-150">Int32</span><span class="sxs-lookup"><span data-stu-id="64354-150">Int32</span></span>|<span data-ttu-id="64354-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64354-151">Version of the device configuration.</span></span> <span data-ttu-id="64354-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64354-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64354-153">licenseType</span><span class="sxs-lookup"><span data-stu-id="64354-153">licenseType</span></span>|[<span data-ttu-id="64354-154">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="64354-154">editionUpgradeLicenseType</span></span>](../resources/intune_deviceconfig_editionupgradelicensetype.md)|<span data-ttu-id="64354-155">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="64354-155">Edition Upgrade License Type.</span></span> <span data-ttu-id="64354-156">Os valores possíveis são: `productKey`, `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="64354-156">The possible values are:</span></span>|
|<span data-ttu-id="64354-157">targetEdition</span><span class="sxs-lookup"><span data-stu-id="64354-157">targetEdition</span></span>|[<span data-ttu-id="64354-158">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="64354-158">windows10EditionType</span></span>](../resources/intune_deviceconfig_windows10editiontype.md)|<span data-ttu-id="64354-159">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="64354-159">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="64354-160">Os valores possíveis são: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="64354-160">The possible values are `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, or `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="64354-161">license</span><span class="sxs-lookup"><span data-stu-id="64354-161">license</span></span>|<span data-ttu-id="64354-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64354-162">String</span></span>|<span data-ttu-id="64354-163">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="64354-163">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="64354-164">productKey</span><span class="sxs-lookup"><span data-stu-id="64354-164">productKey</span></span>|<span data-ttu-id="64354-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64354-165">String</span></span>|<span data-ttu-id="64354-166">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="64354-166">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="64354-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="64354-167">Response</span></span>
<span data-ttu-id="64354-168">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64354-168">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64354-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64354-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="64354-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64354-170">Request</span></span>
<span data-ttu-id="64354-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64354-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 309

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```

### <a name="response"></a><span data-ttu-id="64354-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="64354-172">Response</span></span>
<span data-ttu-id="64354-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64354-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 483

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```



