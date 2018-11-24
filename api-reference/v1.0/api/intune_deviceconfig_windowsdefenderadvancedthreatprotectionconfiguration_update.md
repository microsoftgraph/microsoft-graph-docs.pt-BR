# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="50b5a-101">Atualizar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="50b5a-101">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="50b5a-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="50b5a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50b5a-103">Atualizar as propriedades de um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50b5a-103">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50b5a-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50b5a-104">Prerequisites</span></span>
<span data-ttu-id="50b5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="50b5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="50b5a-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50b5a-107">Permission type</span></span>|<span data-ttu-id="50b5a-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50b5a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50b5a-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50b5a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="50b5a-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50b5a-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50b5a-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50b5a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50b5a-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50b5a-112">Not supported.</span></span>|
|<span data-ttu-id="50b5a-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50b5a-113">Application</span></span>|<span data-ttu-id="50b5a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50b5a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50b5a-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50b5a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="50b5a-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50b5a-116">Request headers</span></span>
|<span data-ttu-id="50b5a-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50b5a-117">Header</span></span>|<span data-ttu-id="50b5a-118">Valor</span><span class="sxs-lookup"><span data-stu-id="50b5a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50b5a-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="50b5a-119">Authorization</span></span>|<span data-ttu-id="50b5a-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50b5a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50b5a-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50b5a-121">Accept</span></span>|<span data-ttu-id="50b5a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="50b5a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50b5a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50b5a-123">Request body</span></span>
<span data-ttu-id="50b5a-124">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50b5a-124">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="50b5a-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50b5a-125">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="50b5a-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50b5a-126">Property</span></span>|<span data-ttu-id="50b5a-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="50b5a-127">Type</span></span>|<span data-ttu-id="50b5a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="50b5a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50b5a-129">id</span><span class="sxs-lookup"><span data-stu-id="50b5a-129">id</span></span>|<span data-ttu-id="50b5a-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50b5a-130">String</span></span>|<span data-ttu-id="50b5a-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="50b5a-131">Key of the entity.</span></span> <span data-ttu-id="50b5a-132">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50b5a-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50b5a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50b5a-133">lastModifiedDateTime</span></span>|<span data-ttu-id="50b5a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50b5a-134">DateTimeOffset</span></span>|<span data-ttu-id="50b5a-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="50b5a-135">DateTime the object was last modified.</span></span> <span data-ttu-id="50b5a-136">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50b5a-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50b5a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50b5a-137">createdDateTime</span></span>|<span data-ttu-id="50b5a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50b5a-138">DateTimeOffset</span></span>|<span data-ttu-id="50b5a-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="50b5a-139">DateTime the object was created.</span></span> <span data-ttu-id="50b5a-140">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50b5a-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50b5a-141">descrição</span><span class="sxs-lookup"><span data-stu-id="50b5a-141">description</span></span>|<span data-ttu-id="50b5a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50b5a-142">String</span></span>|<span data-ttu-id="50b5a-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="50b5a-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="50b5a-144">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50b5a-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50b5a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="50b5a-145">displayName</span></span>|<span data-ttu-id="50b5a-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50b5a-146">String</span></span>|<span data-ttu-id="50b5a-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="50b5a-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="50b5a-148">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50b5a-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50b5a-149">version</span><span class="sxs-lookup"><span data-stu-id="50b5a-149">version</span></span>|<span data-ttu-id="50b5a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="50b5a-150">Int32</span></span>|<span data-ttu-id="50b5a-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="50b5a-151">Version of the device configuration.</span></span> <span data-ttu-id="50b5a-152">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="50b5a-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50b5a-153">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="50b5a-153">allowSampleSharing</span></span>|<span data-ttu-id="50b5a-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="50b5a-154">Boolean</span></span>|<span data-ttu-id="50b5a-155">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="50b5a-155">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="50b5a-156">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="50b5a-156">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="50b5a-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="50b5a-157">Boolean</span></span>|<span data-ttu-id="50b5a-158">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="50b5a-158">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="50b5a-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="50b5a-159">Response</span></span>
<span data-ttu-id="50b5a-160">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50b5a-160">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50b5a-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50b5a-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="50b5a-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50b5a-162">Request</span></span>
<span data-ttu-id="50b5a-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50b5a-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

### <a name="response"></a><span data-ttu-id="50b5a-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="50b5a-164">Response</span></span>
<span data-ttu-id="50b5a-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50b5a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



