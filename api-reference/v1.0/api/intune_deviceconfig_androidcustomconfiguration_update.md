# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="34cbb-101">Atualizar androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="34cbb-101">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="34cbb-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="34cbb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34cbb-103">Atualiza as propriedades de um objeto [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34cbb-103">Update the properties of a [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="34cbb-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34cbb-104">Prerequisites</span></span>
<span data-ttu-id="34cbb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="34cbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="34cbb-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34cbb-107">Permission type</span></span>|<span data-ttu-id="34cbb-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34cbb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34cbb-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34cbb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="34cbb-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34cbb-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34cbb-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34cbb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34cbb-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34cbb-112">Not supported.</span></span>|
|<span data-ttu-id="34cbb-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34cbb-113">Application</span></span>|<span data-ttu-id="34cbb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34cbb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34cbb-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34cbb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="34cbb-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34cbb-116">Request headers</span></span>
|<span data-ttu-id="34cbb-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34cbb-117">Header</span></span>|<span data-ttu-id="34cbb-118">Valor</span><span class="sxs-lookup"><span data-stu-id="34cbb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34cbb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="34cbb-119">Authorization</span></span>|<span data-ttu-id="34cbb-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34cbb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34cbb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="34cbb-121">Accept</span></span>|<span data-ttu-id="34cbb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="34cbb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34cbb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34cbb-123">Request body</span></span>
<span data-ttu-id="34cbb-124">No corpo da solicitação, forneça uma representação JSON do objeto [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34cbb-124">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="34cbb-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34cbb-125">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="34cbb-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34cbb-126">Property</span></span>|<span data-ttu-id="34cbb-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="34cbb-127">Type</span></span>|<span data-ttu-id="34cbb-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="34cbb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34cbb-129">id</span><span class="sxs-lookup"><span data-stu-id="34cbb-129">id</span></span>|<span data-ttu-id="34cbb-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34cbb-130">String</span></span>|<span data-ttu-id="34cbb-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="34cbb-131">Key of the entity.</span></span> <span data-ttu-id="34cbb-132">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34cbb-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34cbb-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34cbb-133">lastModifiedDateTime</span></span>|<span data-ttu-id="34cbb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34cbb-134">DateTimeOffset</span></span>|<span data-ttu-id="34cbb-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="34cbb-135">DateTime the object was last modified.</span></span> <span data-ttu-id="34cbb-136">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34cbb-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34cbb-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34cbb-137">createdDateTime</span></span>|<span data-ttu-id="34cbb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34cbb-138">DateTimeOffset</span></span>|<span data-ttu-id="34cbb-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="34cbb-139">DateTime the object was created.</span></span> <span data-ttu-id="34cbb-140">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34cbb-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34cbb-141">description</span><span class="sxs-lookup"><span data-stu-id="34cbb-141">description</span></span>|<span data-ttu-id="34cbb-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34cbb-142">String</span></span>|<span data-ttu-id="34cbb-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34cbb-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34cbb-144">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34cbb-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34cbb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="34cbb-145">displayName</span></span>|<span data-ttu-id="34cbb-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34cbb-146">String</span></span>|<span data-ttu-id="34cbb-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34cbb-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34cbb-148">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34cbb-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34cbb-149">version</span><span class="sxs-lookup"><span data-stu-id="34cbb-149">version</span></span>|<span data-ttu-id="34cbb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="34cbb-150">Int32</span></span>|<span data-ttu-id="34cbb-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34cbb-151">Version of the device configuration.</span></span> <span data-ttu-id="34cbb-152">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34cbb-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34cbb-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="34cbb-153">omaSettings</span></span>|<span data-ttu-id="34cbb-154">Coleção [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="34cbb-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="34cbb-155">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="34cbb-155">OMA settings.</span></span> <span data-ttu-id="34cbb-156">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="34cbb-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="34cbb-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="34cbb-157">Response</span></span>
<span data-ttu-id="34cbb-158">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34cbb-158">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34cbb-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34cbb-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="34cbb-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34cbb-160">Request</span></span>
<span data-ttu-id="34cbb-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34cbb-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="34cbb-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="34cbb-162">Response</span></span>
<span data-ttu-id="34cbb-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34cbb-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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



