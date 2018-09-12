# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="ea962-101">Criar windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea962-101">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="ea962-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ea962-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea962-103">Cria um novo objeto [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea962-103">Create a new [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea962-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ea962-104">Prerequisites</span></span>
<span data-ttu-id="ea962-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ea962-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ea962-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea962-107">Permission type</span></span>|<span data-ttu-id="ea962-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ea962-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea962-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea962-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ea962-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea962-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea962-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea962-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea962-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea962-112">Not supported.</span></span>|
|<span data-ttu-id="ea962-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea962-113">Application</span></span>|<span data-ttu-id="ea962-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea962-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea962-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea962-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ea962-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea962-116">Request headers</span></span>
|<span data-ttu-id="ea962-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ea962-117">Header</span></span>|<span data-ttu-id="ea962-118">Valor</span><span class="sxs-lookup"><span data-stu-id="ea962-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea962-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea962-119">Authorization</span></span>|<span data-ttu-id="ea962-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="ea962-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea962-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ea962-121">Accept</span></span>|<span data-ttu-id="ea962-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ea962-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea962-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea962-123">Request body</span></span>
<span data-ttu-id="ea962-124">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ea962-124">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="ea962-125">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ea962-125">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="ea962-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea962-126">Property</span></span>|<span data-ttu-id="ea962-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea962-127">Type</span></span>|<span data-ttu-id="ea962-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea962-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea962-129">id</span><span class="sxs-lookup"><span data-stu-id="ea962-129">id</span></span>|<span data-ttu-id="ea962-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea962-130">String</span></span>|<span data-ttu-id="ea962-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ea962-131">Key of the entity.</span></span> <span data-ttu-id="ea962-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea962-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea962-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea962-133">lastModifiedDateTime</span></span>|<span data-ttu-id="ea962-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea962-134">DateTimeOffset</span></span>|<span data-ttu-id="ea962-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ea962-135">DateTime the object was last modified.</span></span> <span data-ttu-id="ea962-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea962-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea962-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea962-137">createdDateTime</span></span>|<span data-ttu-id="ea962-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea962-138">DateTimeOffset</span></span>|<span data-ttu-id="ea962-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ea962-139">DateTime the object was created.</span></span> <span data-ttu-id="ea962-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea962-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea962-141">descrição</span><span class="sxs-lookup"><span data-stu-id="ea962-141">description</span></span>|<span data-ttu-id="ea962-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea962-142">String</span></span>|<span data-ttu-id="ea962-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ea962-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ea962-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea962-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea962-145">displayName</span><span class="sxs-lookup"><span data-stu-id="ea962-145">displayName</span></span>|<span data-ttu-id="ea962-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea962-146">String</span></span>|<span data-ttu-id="ea962-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ea962-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ea962-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea962-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea962-149">version</span><span class="sxs-lookup"><span data-stu-id="ea962-149">version</span></span>|<span data-ttu-id="ea962-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ea962-150">Int32</span></span>|<span data-ttu-id="ea962-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ea962-151">Version of the device configuration.</span></span> <span data-ttu-id="ea962-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea962-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea962-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="ea962-153">omaSettings</span></span>|<span data-ttu-id="ea962-154">Coleção [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ea962-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="ea962-155">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="ea962-155">OMA settings.</span></span> <span data-ttu-id="ea962-156">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="ea962-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ea962-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea962-157">Response</span></span>
<span data-ttu-id="ea962-158">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea962-158">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea962-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea962-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea962-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea962-160">Request</span></span>
<span data-ttu-id="ea962-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea962-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 473

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ea962-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea962-162">Response</span></span>
<span data-ttu-id="ea962-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea962-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```








