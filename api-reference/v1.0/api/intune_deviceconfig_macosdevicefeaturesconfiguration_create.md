# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="0a1b0-101">Criar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0a1b0-101">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="0a1b0-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a1b0-103">Criar um novo objeto [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a1b0-103">Create a new [plannerBucket](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a1b0-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a1b0-104">Prerequisites</span></span>
<span data-ttu-id="0a1b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0a1b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0a1b0-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a1b0-107">Permission type</span></span>|<span data-ttu-id="0a1b0-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a1b0-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a1b0-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a1b0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0a1b0-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a1b0-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0a1b0-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a1b0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a1b0-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-112">Not supported.</span></span>|
|<span data-ttu-id="0a1b0-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a1b0-113">Application</span></span>|<span data-ttu-id="0a1b0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a1b0-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a1b0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0a1b0-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1b0-116">Request headers</span></span>
|<span data-ttu-id="0a1b0-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a1b0-117">Header</span></span>|<span data-ttu-id="0a1b0-118">Valor</span><span class="sxs-lookup"><span data-stu-id="0a1b0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a1b0-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a1b0-119">Authorization</span></span>|<span data-ttu-id="0a1b0-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0a1b0-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0a1b0-121">Accept</span></span>|<span data-ttu-id="0a1b0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0a1b0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a1b0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1b0-123">Request body</span></span>
<span data-ttu-id="0a1b0-124">No corpo da solicitação, forneça uma representação JSON do objeto macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="0a1b0-125">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="0a1b0-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a1b0-126">Property</span></span>|<span data-ttu-id="0a1b0-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a1b0-127">Type</span></span>|<span data-ttu-id="0a1b0-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a1b0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a1b0-129">id</span><span class="sxs-lookup"><span data-stu-id="0a1b0-129">id</span></span>|<span data-ttu-id="0a1b0-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a1b0-130">String</span></span>|<span data-ttu-id="0a1b0-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-131">Key of the setting.</span></span> <span data-ttu-id="0a1b0-132">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a1b0-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a1b0-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a1b0-133">lastModifiedDateTime</span></span>|<span data-ttu-id="0a1b0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a1b0-134">DateTimeOffset</span></span>|<span data-ttu-id="0a1b0-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="0a1b0-136">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a1b0-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a1b0-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a1b0-137">createdDateTime</span></span>|<span data-ttu-id="0a1b0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a1b0-138">DateTimeOffset</span></span>|<span data-ttu-id="0a1b0-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-139">DateTime the object was created.</span></span> <span data-ttu-id="0a1b0-140">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a1b0-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a1b0-141">descrição</span><span class="sxs-lookup"><span data-stu-id="0a1b0-141">description</span></span>|<span data-ttu-id="0a1b0-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a1b0-142">String</span></span>|<span data-ttu-id="0a1b0-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0a1b0-144">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a1b0-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a1b0-145">displayName</span><span class="sxs-lookup"><span data-stu-id="0a1b0-145">displayName</span></span>|<span data-ttu-id="0a1b0-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a1b0-146">String</span></span>|<span data-ttu-id="0a1b0-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0a1b0-148">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a1b0-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a1b0-149">version</span><span class="sxs-lookup"><span data-stu-id="0a1b0-149">version</span></span>|<span data-ttu-id="0a1b0-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0a1b0-150">Int32</span></span>|<span data-ttu-id="0a1b0-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-151">Version of the device configuration.</span></span> <span data-ttu-id="0a1b0-152">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0a1b0-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0a1b0-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a1b0-153">Response</span></span>
<span data-ttu-id="0a1b0-154">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-154">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a1b0-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a1b0-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a1b0-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1b0-156">Request</span></span>
<span data-ttu-id="0a1b0-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 234

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="0a1b0-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a1b0-158">Response</span></span>
<span data-ttu-id="0a1b0-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a1b0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



