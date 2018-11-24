# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="32d07-101">Criar androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="32d07-101">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="32d07-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="32d07-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32d07-103">Criar um novo objeto [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32d07-103">Create a new [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32d07-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32d07-104">Prerequisites</span></span>
<span data-ttu-id="32d07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="32d07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="32d07-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32d07-107">Permission type</span></span>|<span data-ttu-id="32d07-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="32d07-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32d07-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32d07-109">Delegated (work or school account)</span></span>|<span data-ttu-id="32d07-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32d07-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32d07-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32d07-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32d07-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32d07-112">Not supported.</span></span>|
|<span data-ttu-id="32d07-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32d07-113">Application</span></span>|<span data-ttu-id="32d07-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32d07-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32d07-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32d07-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="32d07-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32d07-116">Request headers</span></span>
|<span data-ttu-id="32d07-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32d07-117">Header</span></span>|<span data-ttu-id="32d07-118">Valor</span><span class="sxs-lookup"><span data-stu-id="32d07-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32d07-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="32d07-119">Authorization</span></span>|<span data-ttu-id="32d07-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32d07-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32d07-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="32d07-121">Accept</span></span>|<span data-ttu-id="32d07-122">application/json</span><span class="sxs-lookup"><span data-stu-id="32d07-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32d07-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32d07-123">Request body</span></span>
<span data-ttu-id="32d07-124">No corpo da solicitação, forneça uma representação JSON do objeto androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="32d07-124">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="32d07-125">A tabela a seguir mostra as propriedades que são necessárias ao criar androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="32d07-125">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="32d07-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32d07-126">Property</span></span>|<span data-ttu-id="32d07-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="32d07-127">Type</span></span>|<span data-ttu-id="32d07-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="32d07-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32d07-129">id</span><span class="sxs-lookup"><span data-stu-id="32d07-129">id</span></span>|<span data-ttu-id="32d07-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32d07-130">String</span></span>|<span data-ttu-id="32d07-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="32d07-131">Key of the entity.</span></span> <span data-ttu-id="32d07-132">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="32d07-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32d07-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32d07-133">lastModifiedDateTime</span></span>|<span data-ttu-id="32d07-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32d07-134">DateTimeOffset</span></span>|<span data-ttu-id="32d07-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="32d07-135">DateTime the object was last modified.</span></span> <span data-ttu-id="32d07-136">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="32d07-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32d07-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32d07-137">createdDateTime</span></span>|<span data-ttu-id="32d07-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32d07-138">DateTimeOffset</span></span>|<span data-ttu-id="32d07-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="32d07-139">DateTime the object was created.</span></span> <span data-ttu-id="32d07-140">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="32d07-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32d07-141">descrição</span><span class="sxs-lookup"><span data-stu-id="32d07-141">description</span></span>|<span data-ttu-id="32d07-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32d07-142">String</span></span>|<span data-ttu-id="32d07-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32d07-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="32d07-144">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="32d07-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32d07-145">displayName</span><span class="sxs-lookup"><span data-stu-id="32d07-145">displayName</span></span>|<span data-ttu-id="32d07-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32d07-146">String</span></span>|<span data-ttu-id="32d07-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32d07-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="32d07-148">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="32d07-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32d07-149">version</span><span class="sxs-lookup"><span data-stu-id="32d07-149">version</span></span>|<span data-ttu-id="32d07-150">Int32</span><span class="sxs-lookup"><span data-stu-id="32d07-150">Int32</span></span>|<span data-ttu-id="32d07-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="32d07-151">Version of the device configuration.</span></span> <span data-ttu-id="32d07-152">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="32d07-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32d07-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="32d07-153">omaSettings</span></span>|<span data-ttu-id="32d07-154">Coleção [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="32d07-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="32d07-155">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="32d07-155">OMA settings.</span></span> <span data-ttu-id="32d07-156">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="32d07-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="32d07-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="32d07-157">Response</span></span>
<span data-ttu-id="32d07-158">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32d07-158">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32d07-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32d07-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="32d07-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32d07-160">Request</span></span>
<span data-ttu-id="32d07-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32d07-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="32d07-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="32d07-162">Response</span></span>
<span data-ttu-id="32d07-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32d07-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



