# <a name="update-devicecategory"></a><span data-ttu-id="af779-101">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="af779-101">Update deviceCategory</span></span>

> <span data-ttu-id="af779-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="af779-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af779-103">Atualizar as propriedades de um objeto [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="af779-103">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af779-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af779-104">Prerequisites</span></span>
<span data-ttu-id="af779-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="af779-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="af779-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af779-107">Permission type</span></span>|<span data-ttu-id="af779-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af779-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af779-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af779-109">Delegated (work or school account)</span></span>|<span data-ttu-id="af779-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af779-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="af779-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af779-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af779-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af779-112">Not supported.</span></span>|
|<span data-ttu-id="af779-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af779-113">Application</span></span>|<span data-ttu-id="af779-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af779-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af779-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af779-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="af779-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af779-116">Request headers</span></span>
|<span data-ttu-id="af779-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af779-117">Header</span></span>|<span data-ttu-id="af779-118">Valor</span><span class="sxs-lookup"><span data-stu-id="af779-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af779-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="af779-119">Authorization</span></span>|<span data-ttu-id="af779-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="af779-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af779-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af779-121">Accept</span></span>|<span data-ttu-id="af779-122">application/json</span><span class="sxs-lookup"><span data-stu-id="af779-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af779-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af779-123">Request body</span></span>
<span data-ttu-id="af779-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="af779-124">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

<span data-ttu-id="af779-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="af779-125">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>

|<span data-ttu-id="af779-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af779-126">Property</span></span>|<span data-ttu-id="af779-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="af779-127">Type</span></span>|<span data-ttu-id="af779-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="af779-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af779-129">id</span><span class="sxs-lookup"><span data-stu-id="af779-129">id</span></span>|<span data-ttu-id="af779-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af779-130">String</span></span>|<span data-ttu-id="af779-131">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="af779-131">Unique identifier for the device category.</span></span> <span data-ttu-id="af779-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af779-132">Read-only.</span></span>|
|<span data-ttu-id="af779-133">**Nível de contratação**</span><span class="sxs-lookup"><span data-stu-id="af779-133">**On-boarding**</span></span>|
|<span data-ttu-id="af779-134">displayName</span><span class="sxs-lookup"><span data-stu-id="af779-134">displayName</span></span>|<span data-ttu-id="af779-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af779-135">String</span></span>|<span data-ttu-id="af779-136">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="af779-136">Display name for the device category.</span></span>|
|<span data-ttu-id="af779-137">descrição</span><span class="sxs-lookup"><span data-stu-id="af779-137">description</span></span>|<span data-ttu-id="af779-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af779-138">String</span></span>|<span data-ttu-id="af779-139">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="af779-139">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="af779-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="af779-140">Response</span></span>
<span data-ttu-id="af779-141">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune_shared_devicecategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af779-141">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af779-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af779-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="af779-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af779-143">Request</span></span>
<span data-ttu-id="af779-144">Estes são exemplos da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af779-144">Here are a couple of examples of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="af779-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="af779-145">Response</span></span>
<span data-ttu-id="af779-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af779-146">Here is an example of the response.</span></span> <span data-ttu-id="af779-147">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="af779-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="af779-148">Propriedades de resposta irão variar de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="af779-148">Response properties will vary according to context.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



