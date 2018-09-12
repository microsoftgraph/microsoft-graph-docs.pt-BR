# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="aee45-101">Criar macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="aee45-101">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="aee45-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="aee45-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aee45-103">Cria um novo objeto [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aee45-103">Create a new [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aee45-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aee45-104">Prerequisites</span></span>
<span data-ttu-id="aee45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aee45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aee45-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aee45-107">Permission type</span></span>|<span data-ttu-id="aee45-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aee45-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aee45-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aee45-109">Delegated (work or school account)</span></span>|<span data-ttu-id="aee45-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aee45-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aee45-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aee45-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aee45-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aee45-112">Not supported.</span></span>|
|<span data-ttu-id="aee45-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aee45-113">Application</span></span>|<span data-ttu-id="aee45-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aee45-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aee45-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aee45-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="aee45-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aee45-116">Request headers</span></span>
|<span data-ttu-id="aee45-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aee45-117">Header</span></span>|<span data-ttu-id="aee45-118">Valor</span><span class="sxs-lookup"><span data-stu-id="aee45-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aee45-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="aee45-119">Authorization</span></span>|<span data-ttu-id="aee45-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="aee45-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aee45-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aee45-121">Accept</span></span>|<span data-ttu-id="aee45-122">application/json</span><span class="sxs-lookup"><span data-stu-id="aee45-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aee45-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aee45-123">Request body</span></span>
<span data-ttu-id="aee45-124">No corpo da solicitação, forneça uma representação JSON do objeto macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="aee45-124">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="aee45-125">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="aee45-125">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="aee45-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aee45-126">Property</span></span>|<span data-ttu-id="aee45-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="aee45-127">Type</span></span>|<span data-ttu-id="aee45-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="aee45-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aee45-129">id</span><span class="sxs-lookup"><span data-stu-id="aee45-129">id</span></span>|<span data-ttu-id="aee45-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aee45-130">String</span></span>|<span data-ttu-id="aee45-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aee45-131">Key of the entity.</span></span> <span data-ttu-id="aee45-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aee45-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee45-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aee45-133">lastModifiedDateTime</span></span>|<span data-ttu-id="aee45-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aee45-134">DateTimeOffset</span></span>|<span data-ttu-id="aee45-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="aee45-135">DateTime the object was last modified.</span></span> <span data-ttu-id="aee45-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aee45-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee45-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aee45-137">createdDateTime</span></span>|<span data-ttu-id="aee45-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aee45-138">DateTimeOffset</span></span>|<span data-ttu-id="aee45-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="aee45-139">DateTime the object was created.</span></span> <span data-ttu-id="aee45-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aee45-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee45-141">descrição</span><span class="sxs-lookup"><span data-stu-id="aee45-141">description</span></span>|<span data-ttu-id="aee45-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aee45-142">String</span></span>|<span data-ttu-id="aee45-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aee45-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aee45-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aee45-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee45-145">displayName</span><span class="sxs-lookup"><span data-stu-id="aee45-145">displayName</span></span>|<span data-ttu-id="aee45-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aee45-146">String</span></span>|<span data-ttu-id="aee45-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aee45-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aee45-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aee45-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee45-149">version</span><span class="sxs-lookup"><span data-stu-id="aee45-149">version</span></span>|<span data-ttu-id="aee45-150">Int32</span><span class="sxs-lookup"><span data-stu-id="aee45-150">Int32</span></span>|<span data-ttu-id="aee45-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aee45-151">Version of the device configuration.</span></span> <span data-ttu-id="aee45-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aee45-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee45-153">payloadName</span><span class="sxs-lookup"><span data-stu-id="aee45-153">payloadName</span></span>|<span data-ttu-id="aee45-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aee45-154">String</span></span>|<span data-ttu-id="aee45-155">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="aee45-155">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="aee45-156">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="aee45-156">payloadFileName</span></span>|<span data-ttu-id="aee45-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aee45-157">String</span></span>|<span data-ttu-id="aee45-158">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="aee45-158">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="aee45-159">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="aee45-159">\*.xml).</span></span>|
|<span data-ttu-id="aee45-160">payload</span><span class="sxs-lookup"><span data-stu-id="aee45-160">payload</span></span>|<span data-ttu-id="aee45-161">Binária</span><span class="sxs-lookup"><span data-stu-id="aee45-161">Binary</span></span>|<span data-ttu-id="aee45-162">Carga.</span><span class="sxs-lookup"><span data-stu-id="aee45-162">Payload.</span></span> <span data-ttu-id="aee45-163">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="aee45-163">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="aee45-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="aee45-164">Response</span></span>
<span data-ttu-id="aee45-165">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aee45-165">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aee45-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aee45-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="aee45-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aee45-167">Request</span></span>
<span data-ttu-id="aee45-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aee45-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 345

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="aee45-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="aee45-169">Response</span></span>
<span data-ttu-id="aee45-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aee45-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```








