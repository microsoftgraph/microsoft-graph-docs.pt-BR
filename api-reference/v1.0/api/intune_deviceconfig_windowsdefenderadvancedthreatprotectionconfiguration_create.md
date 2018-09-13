# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="43372-101">Criar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="43372-101">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="43372-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="43372-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43372-103">Criar um novo objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43372-103">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43372-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43372-104">Prerequisites</span></span>
<span data-ttu-id="43372-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="43372-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="43372-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43372-107">Permission type</span></span>|<span data-ttu-id="43372-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="43372-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43372-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43372-109">Delegated (work or school account)</span></span>|<span data-ttu-id="43372-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43372-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43372-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43372-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43372-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43372-112">Not supported.</span></span>|
|<span data-ttu-id="43372-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43372-113">Application</span></span>|<span data-ttu-id="43372-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43372-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43372-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43372-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="43372-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43372-116">Request headers</span></span>
|<span data-ttu-id="43372-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43372-117">Header</span></span>|<span data-ttu-id="43372-118">Valor</span><span class="sxs-lookup"><span data-stu-id="43372-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43372-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="43372-119">Authorization</span></span>|<span data-ttu-id="43372-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="43372-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43372-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43372-121">Accept</span></span>|<span data-ttu-id="43372-122">application/json</span><span class="sxs-lookup"><span data-stu-id="43372-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43372-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43372-123">Request body</span></span>
<span data-ttu-id="43372-124">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="43372-124">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="43372-125">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="43372-125">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="43372-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43372-126">Property</span></span>|<span data-ttu-id="43372-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="43372-127">Type</span></span>|<span data-ttu-id="43372-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="43372-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43372-129">id</span><span class="sxs-lookup"><span data-stu-id="43372-129">id</span></span>|<span data-ttu-id="43372-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43372-130">String</span></span>|<span data-ttu-id="43372-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="43372-131">Key of the entity.</span></span> <span data-ttu-id="43372-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43372-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43372-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43372-133">lastModifiedDateTime</span></span>|<span data-ttu-id="43372-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43372-134">DateTimeOffset</span></span>|<span data-ttu-id="43372-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="43372-135">DateTime the object was last modified.</span></span> <span data-ttu-id="43372-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43372-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43372-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43372-137">createdDateTime</span></span>|<span data-ttu-id="43372-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43372-138">DateTimeOffset</span></span>|<span data-ttu-id="43372-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="43372-139">DateTime the object was created.</span></span> <span data-ttu-id="43372-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43372-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43372-141">descrição</span><span class="sxs-lookup"><span data-stu-id="43372-141">description</span></span>|<span data-ttu-id="43372-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43372-142">String</span></span>|<span data-ttu-id="43372-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43372-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="43372-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43372-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43372-145">displayName</span><span class="sxs-lookup"><span data-stu-id="43372-145">displayName</span></span>|<span data-ttu-id="43372-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43372-146">String</span></span>|<span data-ttu-id="43372-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43372-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="43372-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43372-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43372-149">version</span><span class="sxs-lookup"><span data-stu-id="43372-149">version</span></span>|<span data-ttu-id="43372-150">Int32</span><span class="sxs-lookup"><span data-stu-id="43372-150">Int32</span></span>|<span data-ttu-id="43372-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43372-151">Version of the device configuration.</span></span> <span data-ttu-id="43372-152">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43372-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43372-153">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="43372-153">allowSampleSharing</span></span>|<span data-ttu-id="43372-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="43372-154">Boolean</span></span>|<span data-ttu-id="43372-155">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="43372-155">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="43372-156">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="43372-156">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="43372-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="43372-157">Boolean</span></span>|<span data-ttu-id="43372-158">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="43372-158">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="43372-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="43372-159">Response</span></span>
<span data-ttu-id="43372-160">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43372-160">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43372-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43372-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="43372-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43372-162">Request</span></span>
<span data-ttu-id="43372-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43372-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

### <a name="response"></a><span data-ttu-id="43372-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="43372-164">Response</span></span>
<span data-ttu-id="43372-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43372-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```








