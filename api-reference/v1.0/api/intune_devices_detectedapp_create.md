# <a name="create-detectedapp"></a><span data-ttu-id="bc652-101">Criar detectedApp</span><span class="sxs-lookup"><span data-stu-id="bc652-101">Create detectedApp</span></span>

> <span data-ttu-id="bc652-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bc652-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc652-103">Criar um novo objeto [detectedApp](../resources/intune_devices_detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc652-103">Create a new [plannerBucket](../resources/intune_devices_detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bc652-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc652-104">Prerequisites</span></span>
<span data-ttu-id="bc652-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc652-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bc652-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc652-107">Permission type</span></span>|<span data-ttu-id="bc652-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bc652-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc652-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc652-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bc652-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc652-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bc652-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc652-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc652-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc652-112">Not supported.</span></span>|
|<span data-ttu-id="bc652-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc652-113">Application</span></span>|<span data-ttu-id="bc652-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc652-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc652-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc652-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="bc652-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc652-116">Request headers</span></span>
|<span data-ttu-id="bc652-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc652-117">Header</span></span>|<span data-ttu-id="bc652-118">Valor</span><span class="sxs-lookup"><span data-stu-id="bc652-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc652-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc652-119">Authorization</span></span>|<span data-ttu-id="bc652-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc652-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bc652-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc652-121">Accept</span></span>|<span data-ttu-id="bc652-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bc652-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc652-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc652-123">Request body</span></span>
<span data-ttu-id="bc652-124">No corpo da solicitação, forneça uma representação JSON do objeto detectedApp.</span><span class="sxs-lookup"><span data-stu-id="bc652-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="bc652-125">A tabela a seguir mostra as propriedades que são necessárias ao criar detectedApp.</span><span class="sxs-lookup"><span data-stu-id="bc652-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="bc652-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc652-126">Property</span></span>|<span data-ttu-id="bc652-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc652-127">Type</span></span>|<span data-ttu-id="bc652-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc652-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc652-129">id</span><span class="sxs-lookup"><span data-stu-id="bc652-129">id</span></span>|<span data-ttu-id="bc652-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc652-130">String</span></span>|<span data-ttu-id="bc652-131">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="bc652-131">The unique Identifier for the detected application.</span></span> <span data-ttu-id="bc652-132">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="bc652-132">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="bc652-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc652-133">Read-only.</span></span>|
|<span data-ttu-id="bc652-134">displayName</span><span class="sxs-lookup"><span data-stu-id="bc652-134">displayName</span></span>|<span data-ttu-id="bc652-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc652-135">String</span></span>|<span data-ttu-id="bc652-136">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="bc652-136">Name of the discovered application.</span></span> <span data-ttu-id="bc652-137">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="bc652-137">Read-only</span></span>|
|<span data-ttu-id="bc652-138">version</span><span class="sxs-lookup"><span data-stu-id="bc652-138">version</span></span>|<span data-ttu-id="bc652-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc652-139">String</span></span>|<span data-ttu-id="bc652-140">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="bc652-140">Version of the discovered application.</span></span> <span data-ttu-id="bc652-141">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="bc652-141">Read-only</span></span>|
|<span data-ttu-id="bc652-142">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="bc652-142">sizeInByte</span></span>|<span data-ttu-id="bc652-143">Int64</span><span class="sxs-lookup"><span data-stu-id="bc652-143">Int64</span></span>|<span data-ttu-id="bc652-144">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="bc652-144">Discovered application size in bytes.</span></span> <span data-ttu-id="bc652-145">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="bc652-145">Read-only</span></span>|
|<span data-ttu-id="bc652-146">deviceCount</span><span class="sxs-lookup"><span data-stu-id="bc652-146">deviceCount</span></span>|<span data-ttu-id="bc652-147">Int32</span><span class="sxs-lookup"><span data-stu-id="bc652-147">Int32</span></span>|<span data-ttu-id="bc652-148">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc652-148">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="bc652-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc652-149">Response</span></span>
<span data-ttu-id="bc652-150">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [detectedApp](../resources/intune_devices_detectedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc652-150">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_devices_detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc652-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc652-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc652-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc652-152">Request</span></span>
<span data-ttu-id="bc652-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc652-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
Content-type: application/json
Content-length: 167

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="bc652-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc652-154">Response</span></span>
<span data-ttu-id="bc652-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc652-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



