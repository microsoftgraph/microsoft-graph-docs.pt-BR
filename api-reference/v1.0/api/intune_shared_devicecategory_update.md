# <a name="update-devicecategory"></a><span data-ttu-id="e50a6-101">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="e50a6-101">Update deviceCategory</span></span>

> <span data-ttu-id="e50a6-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e50a6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e50a6-103">Atualizar as propriedades de um objeto [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="e50a6-103">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e50a6-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e50a6-104">Prerequisites</span></span>
<span data-ttu-id="e50a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e50a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e50a6-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e50a6-107">Permission type</span></span>|<span data-ttu-id="e50a6-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e50a6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e50a6-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e50a6-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e50a6-110">&nbsp;&nbsp; **Onboarding** e</span><span class="sxs-lookup"><span data-stu-id="e50a6-110">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="e50a6-111">&nbsp;&nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="e50a6-111">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="e50a6-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e50a6-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e50a6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e50a6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e50a6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e50a6-114">Not supported.</span></span>|
|<span data-ttu-id="e50a6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e50a6-115">Application</span></span>|<span data-ttu-id="e50a6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e50a6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e50a6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e50a6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="e50a6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e50a6-118">Request headers</span></span>
|<span data-ttu-id="e50a6-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e50a6-119">Header</span></span>|<span data-ttu-id="e50a6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e50a6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e50a6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e50a6-121">Authorization</span></span>|<span data-ttu-id="e50a6-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e50a6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e50a6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e50a6-123">Accept</span></span>|<span data-ttu-id="e50a6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e50a6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e50a6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e50a6-125">Request body</span></span>
<span data-ttu-id="e50a6-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="e50a6-126">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

<span data-ttu-id="e50a6-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="e50a6-127">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>

|<span data-ttu-id="e50a6-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e50a6-128">Property</span></span>|<span data-ttu-id="e50a6-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e50a6-129">Type</span></span>|<span data-ttu-id="e50a6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e50a6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e50a6-131">id</span><span class="sxs-lookup"><span data-stu-id="e50a6-131">id</span></span>|<span data-ttu-id="e50a6-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e50a6-132">String</span></span>|<span data-ttu-id="e50a6-133">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e50a6-133">Unique identifier for the device category.</span></span> <span data-ttu-id="e50a6-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e50a6-134">Read-only.</span></span>|
|<span data-ttu-id="e50a6-135">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="e50a6-135">**Onboarding**</span></span>|
|<span data-ttu-id="e50a6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e50a6-136">displayName</span></span>|<span data-ttu-id="e50a6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e50a6-137">String</span></span>|<span data-ttu-id="e50a6-138">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e50a6-138">Display name for the device category.</span></span>|
|<span data-ttu-id="e50a6-139">description</span><span class="sxs-lookup"><span data-stu-id="e50a6-139">description</span></span>|<span data-ttu-id="e50a6-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e50a6-140">String</span></span>|<span data-ttu-id="e50a6-141">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e50a6-141">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="e50a6-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e50a6-142">Response</span></span>
<span data-ttu-id="e50a6-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune_shared_devicecategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e50a6-143">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e50a6-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e50a6-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="e50a6-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e50a6-145">Request</span></span>
<span data-ttu-id="e50a6-146">Estes são exemplos da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e50a6-146">Here are examples of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e50a6-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e50a6-147">Response</span></span>
<span data-ttu-id="e50a6-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e50a6-148">Here is an example of the response.</span></span> <span data-ttu-id="e50a6-149">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="e50a6-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e50a6-150">Propriedades de resposta irá variar de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="e50a6-150">Response properties will vary according to context.</span></span>
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



