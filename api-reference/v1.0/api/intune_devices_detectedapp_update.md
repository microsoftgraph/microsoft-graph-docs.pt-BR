# <a name="update-detectedapp"></a><span data-ttu-id="224a0-101">Atualizar detectedApp</span><span class="sxs-lookup"><span data-stu-id="224a0-101">Update detectedApp</span></span>

> <span data-ttu-id="224a0-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="224a0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="224a0-103">Atualizar as propriedades de um objeto [detectedApp](../resources/intune_devices_detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="224a0-103">Update the properties of a [calendar](../resources/intune_devices_detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="224a0-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="224a0-104">Prerequisites</span></span>
<span data-ttu-id="224a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="224a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="224a0-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="224a0-107">Permission type</span></span>|<span data-ttu-id="224a0-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="224a0-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="224a0-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="224a0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="224a0-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="224a0-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="224a0-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="224a0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="224a0-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="224a0-112">Not supported.</span></span>|
|<span data-ttu-id="224a0-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="224a0-113">Application</span></span>|<span data-ttu-id="224a0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="224a0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="224a0-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="224a0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="224a0-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="224a0-116">Request headers</span></span>
|<span data-ttu-id="224a0-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="224a0-117">Header</span></span>|<span data-ttu-id="224a0-118">Valor</span><span class="sxs-lookup"><span data-stu-id="224a0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="224a0-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="224a0-119">Authorization</span></span>|<span data-ttu-id="224a0-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="224a0-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="224a0-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="224a0-121">Accept</span></span>|<span data-ttu-id="224a0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="224a0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="224a0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="224a0-123">Request body</span></span>
<span data-ttu-id="224a0-124">No corpo da solicitação, forneça uma representação JSON do objeto [detectedApp](../resources/intune_devices_detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="224a0-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_devices_detectedapp.md) object.</span></span>

<span data-ttu-id="224a0-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [detectedApp](../resources/intune_devices_detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="224a0-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="224a0-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="224a0-126">Property</span></span>|<span data-ttu-id="224a0-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="224a0-127">Type</span></span>|<span data-ttu-id="224a0-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="224a0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="224a0-129">id</span><span class="sxs-lookup"><span data-stu-id="224a0-129">id</span></span>|<span data-ttu-id="224a0-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="224a0-130">String</span></span>|<span data-ttu-id="224a0-131">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="224a0-131">The unique Identifier for the detected application.</span></span> <span data-ttu-id="224a0-132">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="224a0-132">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="224a0-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="224a0-133">Read-only.</span></span>|
|<span data-ttu-id="224a0-134">displayName</span><span class="sxs-lookup"><span data-stu-id="224a0-134">displayName</span></span>|<span data-ttu-id="224a0-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="224a0-135">String</span></span>|<span data-ttu-id="224a0-136">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="224a0-136">Name of the discovered application.</span></span> <span data-ttu-id="224a0-137">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="224a0-137">Read-only</span></span>|
|<span data-ttu-id="224a0-138">version</span><span class="sxs-lookup"><span data-stu-id="224a0-138">version</span></span>|<span data-ttu-id="224a0-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="224a0-139">String</span></span>|<span data-ttu-id="224a0-140">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="224a0-140">Version of the discovered application.</span></span> <span data-ttu-id="224a0-141">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="224a0-141">Read-only</span></span>|
|<span data-ttu-id="224a0-142">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="224a0-142">sizeInByte</span></span>|<span data-ttu-id="224a0-143">Int64</span><span class="sxs-lookup"><span data-stu-id="224a0-143">Int64</span></span>|<span data-ttu-id="224a0-144">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="224a0-144">Discovered application size in bytes.</span></span> <span data-ttu-id="224a0-145">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="224a0-145">Read-only</span></span>|
|<span data-ttu-id="224a0-146">deviceCount</span><span class="sxs-lookup"><span data-stu-id="224a0-146">deviceCount</span></span>|<span data-ttu-id="224a0-147">Int32</span><span class="sxs-lookup"><span data-stu-id="224a0-147">Int32</span></span>|<span data-ttu-id="224a0-148">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="224a0-148">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="224a0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="224a0-149">Response</span></span>
<span data-ttu-id="224a0-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [detectedApp](../resources/intune_devices_detectedapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="224a0-150">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_devices_detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="224a0-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="224a0-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="224a0-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="224a0-152">Request</span></span>
<span data-ttu-id="224a0-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="224a0-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}
Content-type: application/json
Content-length: 117

{
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="224a0-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="224a0-154">Response</span></span>
<span data-ttu-id="224a0-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="224a0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 216

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```



