# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="14eaf-101">Atualizar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="14eaf-101">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="14eaf-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="14eaf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14eaf-103">Atualizar as propriedades de um objeto [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eaf-103">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="14eaf-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14eaf-104">Prerequisites</span></span>
<span data-ttu-id="14eaf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="14eaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="14eaf-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14eaf-107">Permission type</span></span>|<span data-ttu-id="14eaf-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14eaf-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14eaf-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14eaf-109">Delegated (work or school account)</span></span>|<span data-ttu-id="14eaf-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14eaf-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14eaf-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14eaf-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14eaf-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14eaf-112">Not supported.</span></span>|
|<span data-ttu-id="14eaf-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14eaf-113">Application</span></span>|<span data-ttu-id="14eaf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14eaf-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14eaf-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14eaf-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="14eaf-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14eaf-116">Request headers</span></span>
|<span data-ttu-id="14eaf-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14eaf-117">Header</span></span>|<span data-ttu-id="14eaf-118">Valor</span><span class="sxs-lookup"><span data-stu-id="14eaf-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14eaf-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="14eaf-119">Authorization</span></span>|<span data-ttu-id="14eaf-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="14eaf-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14eaf-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14eaf-121">Accept</span></span>|<span data-ttu-id="14eaf-122">application/json</span><span class="sxs-lookup"><span data-stu-id="14eaf-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14eaf-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14eaf-123">Request body</span></span>
<span data-ttu-id="14eaf-124">No corpo da solicitação, forneça uma representação JSON do objeto [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eaf-124">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="14eaf-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eaf-125">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="14eaf-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14eaf-126">Property</span></span>|<span data-ttu-id="14eaf-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="14eaf-127">Type</span></span>|<span data-ttu-id="14eaf-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="14eaf-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14eaf-129">id</span><span class="sxs-lookup"><span data-stu-id="14eaf-129">id</span></span>|<span data-ttu-id="14eaf-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14eaf-130">String</span></span>|<span data-ttu-id="14eaf-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="14eaf-131">Key of the entity.</span></span> <span data-ttu-id="14eaf-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14eaf-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eaf-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14eaf-133">lastModifiedDateTime</span></span>|<span data-ttu-id="14eaf-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14eaf-134">DateTimeOffset</span></span>|<span data-ttu-id="14eaf-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="14eaf-135">DateTime the object was last modified.</span></span> <span data-ttu-id="14eaf-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14eaf-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eaf-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14eaf-137">createdDateTime</span></span>|<span data-ttu-id="14eaf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14eaf-138">DateTimeOffset</span></span>|<span data-ttu-id="14eaf-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="14eaf-139">DateTime the object was created.</span></span> <span data-ttu-id="14eaf-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14eaf-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eaf-141">descrição</span><span class="sxs-lookup"><span data-stu-id="14eaf-141">description</span></span>|<span data-ttu-id="14eaf-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14eaf-142">String</span></span>|<span data-ttu-id="14eaf-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="14eaf-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="14eaf-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14eaf-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eaf-145">displayName</span><span class="sxs-lookup"><span data-stu-id="14eaf-145">displayName</span></span>|<span data-ttu-id="14eaf-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14eaf-146">String</span></span>|<span data-ttu-id="14eaf-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="14eaf-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="14eaf-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14eaf-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eaf-149">version</span><span class="sxs-lookup"><span data-stu-id="14eaf-149">version</span></span>|<span data-ttu-id="14eaf-150">Int32</span><span class="sxs-lookup"><span data-stu-id="14eaf-150">Int32</span></span>|<span data-ttu-id="14eaf-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="14eaf-151">Version of the device configuration.</span></span> <span data-ttu-id="14eaf-152">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14eaf-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="14eaf-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="14eaf-153">Response</span></span>
<span data-ttu-id="14eaf-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14eaf-154">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14eaf-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14eaf-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="14eaf-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14eaf-156">Request</span></span>
<span data-ttu-id="14eaf-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14eaf-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 163

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="14eaf-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="14eaf-158">Response</span></span>
<span data-ttu-id="14eaf-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14eaf-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```








