# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="e8446-101">Atualizar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="e8446-101">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="e8446-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e8446-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8446-103">Atualizar as propriedades de um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8446-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8446-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8446-104">Prerequisites</span></span>
<span data-ttu-id="e8446-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e8446-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e8446-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8446-107">Permission type</span></span>|<span data-ttu-id="e8446-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8446-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8446-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8446-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e8446-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8446-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8446-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8446-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8446-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8446-112">Not supported.</span></span>|
|<span data-ttu-id="e8446-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8446-113">Application</span></span>|<span data-ttu-id="e8446-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8446-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8446-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8446-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e8446-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8446-116">Request headers</span></span>
|<span data-ttu-id="e8446-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8446-117">Header</span></span>|<span data-ttu-id="e8446-118">Valor</span><span class="sxs-lookup"><span data-stu-id="e8446-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8446-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8446-119">Authorization</span></span>|<span data-ttu-id="e8446-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8446-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e8446-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8446-121">Accept</span></span>|<span data-ttu-id="e8446-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e8446-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8446-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8446-123">Request body</span></span>
<span data-ttu-id="e8446-124">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8446-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="e8446-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8446-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="e8446-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8446-126">Property</span></span>|<span data-ttu-id="e8446-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8446-127">Type</span></span>|<span data-ttu-id="e8446-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8446-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8446-129">id</span><span class="sxs-lookup"><span data-stu-id="e8446-129">id</span></span>|<span data-ttu-id="e8446-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8446-130">String</span></span>|<span data-ttu-id="e8446-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e8446-131">Key of the setting.</span></span> <span data-ttu-id="e8446-132">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8446-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8446-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8446-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e8446-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8446-134">DateTimeOffset</span></span>|<span data-ttu-id="e8446-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e8446-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="e8446-136">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8446-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8446-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8446-137">createdDateTime</span></span>|<span data-ttu-id="e8446-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8446-138">DateTimeOffset</span></span>|<span data-ttu-id="e8446-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e8446-139">DateTime the object was created.</span></span> <span data-ttu-id="e8446-140">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8446-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8446-141">descrição</span><span class="sxs-lookup"><span data-stu-id="e8446-141">description</span></span>|<span data-ttu-id="e8446-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8446-142">String</span></span>|<span data-ttu-id="e8446-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e8446-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e8446-144">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8446-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8446-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e8446-145">displayName</span></span>|<span data-ttu-id="e8446-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8446-146">String</span></span>|<span data-ttu-id="e8446-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e8446-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e8446-148">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8446-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8446-149">version</span><span class="sxs-lookup"><span data-stu-id="e8446-149">version</span></span>|<span data-ttu-id="e8446-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e8446-150">Int32</span></span>|<span data-ttu-id="e8446-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e8446-151">Version of the device configuration.</span></span> <span data-ttu-id="e8446-152">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e8446-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8446-153">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="e8446-153">allowSampleSharing</span></span>|<span data-ttu-id="e8446-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8446-154">Boolean</span></span>|<span data-ttu-id="e8446-155">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="e8446-155">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="e8446-156">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="e8446-156">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="e8446-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8446-157">Boolean</span></span>|<span data-ttu-id="e8446-158">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="e8446-158">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="e8446-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8446-159">Response</span></span>
<span data-ttu-id="e8446-160">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8446-160">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8446-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8446-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8446-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8446-162">Request</span></span>
<span data-ttu-id="e8446-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8446-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 240

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

### <a name="response"></a><span data-ttu-id="e8446-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8446-164">Response</span></span>
<span data-ttu-id="e8446-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8446-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



