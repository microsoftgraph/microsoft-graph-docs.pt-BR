# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="98e4e-101">Criar editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="98e4e-101">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="98e4e-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="98e4e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98e4e-103">Cria um novo objeto [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="98e4e-103">Create a new [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="98e4e-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98e4e-104">Prerequisites</span></span>
<span data-ttu-id="98e4e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="98e4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="98e4e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98e4e-107">Permission type</span></span>|<span data-ttu-id="98e4e-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98e4e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98e4e-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98e4e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="98e4e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98e4e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98e4e-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98e4e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98e4e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98e4e-112">Not supported.</span></span>|
|<span data-ttu-id="98e4e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98e4e-113">Application</span></span>|<span data-ttu-id="98e4e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98e4e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98e4e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98e4e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="98e4e-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98e4e-116">Request headers</span></span>
|<span data-ttu-id="98e4e-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98e4e-117">Header</span></span>|<span data-ttu-id="98e4e-118">Valor</span><span class="sxs-lookup"><span data-stu-id="98e4e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98e4e-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="98e4e-119">Authorization</span></span>|<span data-ttu-id="98e4e-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98e4e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98e4e-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="98e4e-121">Accept</span></span>|<span data-ttu-id="98e4e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="98e4e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98e4e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98e4e-123">Request body</span></span>
<span data-ttu-id="98e4e-124">No corpo da solicitação, forneça uma representação JSON do objeto editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="98e4e-124">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="98e4e-125">A tabela a seguir mostra as propriedades que são necessárias ao criar editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="98e4e-125">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="98e4e-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98e4e-126">Property</span></span>|<span data-ttu-id="98e4e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="98e4e-127">Type</span></span>|<span data-ttu-id="98e4e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="98e4e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98e4e-129">id</span><span class="sxs-lookup"><span data-stu-id="98e4e-129">id</span></span>|<span data-ttu-id="98e4e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98e4e-130">String</span></span>|<span data-ttu-id="98e4e-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="98e4e-131">Key of the entity.</span></span> <span data-ttu-id="98e4e-132">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98e4e-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98e4e-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="98e4e-133">lastModifiedDateTime</span></span>|<span data-ttu-id="98e4e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98e4e-134">DateTimeOffset</span></span>|<span data-ttu-id="98e4e-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="98e4e-135">DateTime the object was last modified.</span></span> <span data-ttu-id="98e4e-136">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98e4e-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98e4e-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="98e4e-137">createdDateTime</span></span>|<span data-ttu-id="98e4e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98e4e-138">DateTimeOffset</span></span>|<span data-ttu-id="98e4e-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="98e4e-139">DateTime the object was created.</span></span> <span data-ttu-id="98e4e-140">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98e4e-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98e4e-141">descrição</span><span class="sxs-lookup"><span data-stu-id="98e4e-141">description</span></span>|<span data-ttu-id="98e4e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98e4e-142">String</span></span>|<span data-ttu-id="98e4e-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e4e-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="98e4e-144">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98e4e-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98e4e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="98e4e-145">displayName</span></span>|<span data-ttu-id="98e4e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98e4e-146">String</span></span>|<span data-ttu-id="98e4e-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e4e-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="98e4e-148">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98e4e-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98e4e-149">version</span><span class="sxs-lookup"><span data-stu-id="98e4e-149">version</span></span>|<span data-ttu-id="98e4e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="98e4e-150">Int32</span></span>|<span data-ttu-id="98e4e-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e4e-151">Version of the device configuration.</span></span> <span data-ttu-id="98e4e-152">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98e4e-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98e4e-153">licenseType</span><span class="sxs-lookup"><span data-stu-id="98e4e-153">licenseType</span></span>|[<span data-ttu-id="98e4e-154">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="98e4e-154">editionUpgradeLicenseType</span></span>](../resources/intune_deviceconfig_editionupgradelicensetype.md)|<span data-ttu-id="98e4e-155">Tipo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="98e4e-155">Edition Upgrade License Type.</span></span> <span data-ttu-id="98e4e-156">Os valores possíveis são: `productKey`, `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="98e4e-156">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="98e4e-157">targetEdition</span><span class="sxs-lookup"><span data-stu-id="98e4e-157">targetEdition</span></span>|[<span data-ttu-id="98e4e-158">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="98e4e-158">windows10EditionType</span></span>](../resources/intune_deviceconfig_windows10editiontype.md)|<span data-ttu-id="98e4e-159">Edição de destino de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="98e4e-159">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="98e4e-160">Os valores possíveis são: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="98e4e-160">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="98e4e-161">license</span><span class="sxs-lookup"><span data-stu-id="98e4e-161">license</span></span>|<span data-ttu-id="98e4e-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98e4e-162">String</span></span>|<span data-ttu-id="98e4e-163">Conteúdo do arquivo de licença de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="98e4e-163">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="98e4e-164">productKey</span><span class="sxs-lookup"><span data-stu-id="98e4e-164">productKey</span></span>|<span data-ttu-id="98e4e-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98e4e-165">String</span></span>|<span data-ttu-id="98e4e-166">Chave de produto de atualização de edição.</span><span class="sxs-lookup"><span data-stu-id="98e4e-166">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="98e4e-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="98e4e-167">Response</span></span>
<span data-ttu-id="98e4e-168">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98e4e-168">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98e4e-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98e4e-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="98e4e-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98e4e-170">Request</span></span>
<span data-ttu-id="98e4e-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98e4e-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 311

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```

### <a name="response"></a><span data-ttu-id="98e4e-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="98e4e-172">Response</span></span>
<span data-ttu-id="98e4e-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98e4e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



