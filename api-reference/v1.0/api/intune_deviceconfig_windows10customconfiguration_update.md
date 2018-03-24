# <a name="update-windows10customconfiguration"></a><span data-ttu-id="19691-101">Atualizar windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="19691-101">Update windows10CustomConfiguration</span></span>

> <span data-ttu-id="19691-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="19691-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19691-103">Atualizar as propriedades de um objeto [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19691-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windows10customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19691-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="19691-104">Prerequisites</span></span>
<span data-ttu-id="19691-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="19691-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="19691-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19691-107">Permission type</span></span>|<span data-ttu-id="19691-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="19691-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19691-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19691-109">Delegated (work or school account)</span></span>|<span data-ttu-id="19691-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19691-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19691-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19691-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19691-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19691-112">Not supported.</span></span>|
|<span data-ttu-id="19691-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19691-113">Application</span></span>|<span data-ttu-id="19691-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19691-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19691-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19691-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="19691-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19691-116">Request headers</span></span>
|<span data-ttu-id="19691-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19691-117">Header</span></span>|<span data-ttu-id="19691-118">Valor</span><span class="sxs-lookup"><span data-stu-id="19691-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19691-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="19691-119">Authorization</span></span>|<span data-ttu-id="19691-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19691-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="19691-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="19691-121">Accept</span></span>|<span data-ttu-id="19691-122">application/json</span><span class="sxs-lookup"><span data-stu-id="19691-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19691-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19691-123">Request body</span></span>
<span data-ttu-id="19691-124">No corpo da solicitação, forneça uma representação JSON do objeto [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19691-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="19691-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19691-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="19691-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19691-126">Property</span></span>|<span data-ttu-id="19691-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="19691-127">Type</span></span>|<span data-ttu-id="19691-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="19691-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19691-129">id</span><span class="sxs-lookup"><span data-stu-id="19691-129">id</span></span>|<span data-ttu-id="19691-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19691-130">String</span></span>|<span data-ttu-id="19691-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="19691-131">Key of the setting.</span></span> <span data-ttu-id="19691-132">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19691-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19691-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19691-133">lastModifiedDateTime</span></span>|<span data-ttu-id="19691-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19691-134">DateTimeOffset</span></span>|<span data-ttu-id="19691-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="19691-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="19691-136">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19691-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19691-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19691-137">createdDateTime</span></span>|<span data-ttu-id="19691-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19691-138">DateTimeOffset</span></span>|<span data-ttu-id="19691-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="19691-139">DateTime the object was created.</span></span> <span data-ttu-id="19691-140">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19691-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19691-141">descrição</span><span class="sxs-lookup"><span data-stu-id="19691-141">description</span></span>|<span data-ttu-id="19691-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19691-142">String</span></span>|<span data-ttu-id="19691-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19691-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="19691-144">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19691-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19691-145">displayName</span><span class="sxs-lookup"><span data-stu-id="19691-145">displayName</span></span>|<span data-ttu-id="19691-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19691-146">String</span></span>|<span data-ttu-id="19691-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19691-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="19691-148">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19691-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19691-149">version</span><span class="sxs-lookup"><span data-stu-id="19691-149">version</span></span>|<span data-ttu-id="19691-150">Int32</span><span class="sxs-lookup"><span data-stu-id="19691-150">Int32</span></span>|<span data-ttu-id="19691-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19691-151">Version of the device configuration.</span></span> <span data-ttu-id="19691-152">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19691-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19691-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="19691-153">omaSettings</span></span>|<span data-ttu-id="19691-154">Coleção [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="19691-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="19691-155">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="19691-155">OMA settings.</span></span> <span data-ttu-id="19691-156">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="19691-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="19691-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="19691-157">Response</span></span>
<span data-ttu-id="19691-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19691-158">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19691-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19691-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="19691-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19691-160">Request</span></span>
<span data-ttu-id="19691-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19691-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 401

{
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

### <a name="response"></a><span data-ttu-id="19691-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="19691-162">Response</span></span>
<span data-ttu-id="19691-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19691-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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



