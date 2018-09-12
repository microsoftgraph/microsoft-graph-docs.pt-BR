# <a name="create-detectedapp"></a><span data-ttu-id="ceafe-101">Criar detectedApp</span><span class="sxs-lookup"><span data-stu-id="ceafe-101">Create detectedApp</span></span>

> <span data-ttu-id="ceafe-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ceafe-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ceafe-103">Criar um novo objeto [detectedApp](../resources/intune_devices_detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ceafe-103">Create a new [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ceafe-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ceafe-104">Prerequisites</span></span>
<span data-ttu-id="ceafe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ceafe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ceafe-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ceafe-107">Permission type</span></span>|<span data-ttu-id="ceafe-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ceafe-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ceafe-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ceafe-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ceafe-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceafe-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ceafe-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ceafe-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ceafe-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ceafe-112">Not supported.</span></span>|
|<span data-ttu-id="ceafe-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ceafe-113">Application</span></span>|<span data-ttu-id="ceafe-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ceafe-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ceafe-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ceafe-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="ceafe-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ceafe-116">Request headers</span></span>
|<span data-ttu-id="ceafe-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ceafe-117">Header</span></span>|<span data-ttu-id="ceafe-118">Valor</span><span class="sxs-lookup"><span data-stu-id="ceafe-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ceafe-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ceafe-119">Authorization</span></span>|<span data-ttu-id="ceafe-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="ceafe-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ceafe-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ceafe-121">Accept</span></span>|<span data-ttu-id="ceafe-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ceafe-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ceafe-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ceafe-123">Request body</span></span>
<span data-ttu-id="ceafe-124">No corpo da solicitação, forneça uma representação JSON do objeto detectedApp.</span><span class="sxs-lookup"><span data-stu-id="ceafe-124">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="ceafe-125">A tabela a seguir mostra as propriedades que são necessárias ao criar detectedApp.</span><span class="sxs-lookup"><span data-stu-id="ceafe-125">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="ceafe-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ceafe-126">Property</span></span>|<span data-ttu-id="ceafe-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ceafe-127">Type</span></span>|<span data-ttu-id="ceafe-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ceafe-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ceafe-129">id</span><span class="sxs-lookup"><span data-stu-id="ceafe-129">id</span></span>|<span data-ttu-id="ceafe-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ceafe-130">String</span></span>|<span data-ttu-id="ceafe-131">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="ceafe-131">The unique Identifier for the detected application.</span></span> <span data-ttu-id="ceafe-132">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="ceafe-132">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="ceafe-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ceafe-133">Read-only.</span></span>|
|<span data-ttu-id="ceafe-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ceafe-134">displayName</span></span>|<span data-ttu-id="ceafe-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ceafe-135">String</span></span>|<span data-ttu-id="ceafe-136">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="ceafe-136">Name of the discovered application.</span></span> <span data-ttu-id="ceafe-137">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="ceafe-137">Read-only</span></span>|
|<span data-ttu-id="ceafe-138">version</span><span class="sxs-lookup"><span data-stu-id="ceafe-138">version</span></span>|<span data-ttu-id="ceafe-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ceafe-139">String</span></span>|<span data-ttu-id="ceafe-140">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="ceafe-140">Version of the discovered application.</span></span> <span data-ttu-id="ceafe-141">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="ceafe-141">Read-only</span></span>|
|<span data-ttu-id="ceafe-142">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="ceafe-142">sizeInByte</span></span>|<span data-ttu-id="ceafe-143">Int64</span><span class="sxs-lookup"><span data-stu-id="ceafe-143">Int64</span></span>|<span data-ttu-id="ceafe-144">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="ceafe-144">Discovered application size in bytes.</span></span> <span data-ttu-id="ceafe-145">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="ceafe-145">Read-only</span></span>|
|<span data-ttu-id="ceafe-146">deviceCount</span><span class="sxs-lookup"><span data-stu-id="ceafe-146">deviceCount</span></span>|<span data-ttu-id="ceafe-147">Int32</span><span class="sxs-lookup"><span data-stu-id="ceafe-147">Int32</span></span>|<span data-ttu-id="ceafe-148">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="ceafe-148">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="ceafe-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceafe-149">Response</span></span>
<span data-ttu-id="ceafe-150">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [detectedApp](../resources/intune_devices_detectedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ceafe-150">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune_devices_detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceafe-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ceafe-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="ceafe-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ceafe-152">Request</span></span>
<span data-ttu-id="ceafe-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ceafe-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ceafe-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceafe-154">Response</span></span>
<span data-ttu-id="ceafe-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ceafe-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








