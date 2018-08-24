# <a name="create-devicecategory"></a><span data-ttu-id="20560-101">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="20560-101">Create deviceCategory</span></span>

> <span data-ttu-id="20560-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="20560-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20560-103">Cria um novo objeto [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="20560-103">Create a new [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20560-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20560-104">Prerequisites</span></span>
<span data-ttu-id="20560-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="20560-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="20560-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20560-107">Permission type</span></span>|<span data-ttu-id="20560-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="20560-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20560-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20560-109">Delegated (work or school account)</span></span>|<span data-ttu-id="20560-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20560-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="20560-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20560-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20560-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20560-112">Not supported.</span></span>|
|<span data-ttu-id="20560-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20560-113">Application</span></span>|<span data-ttu-id="20560-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20560-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20560-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20560-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="20560-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20560-116">Request headers</span></span>
|<span data-ttu-id="20560-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20560-117">Header</span></span>|<span data-ttu-id="20560-118">Valor</span><span class="sxs-lookup"><span data-stu-id="20560-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20560-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="20560-119">Authorization</span></span>|<span data-ttu-id="20560-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="20560-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20560-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="20560-121">Accept</span></span>|<span data-ttu-id="20560-122">application/json</span><span class="sxs-lookup"><span data-stu-id="20560-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20560-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20560-123">Request body</span></span>
<span data-ttu-id="20560-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="20560-124">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="20560-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="20560-125">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="20560-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20560-126">Property</span></span>|<span data-ttu-id="20560-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="20560-127">Type</span></span>|<span data-ttu-id="20560-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="20560-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20560-129">id</span><span class="sxs-lookup"><span data-stu-id="20560-129">id</span></span>|<span data-ttu-id="20560-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20560-130">String</span></span>|<span data-ttu-id="20560-131">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="20560-131">Unique identifier for the device category.</span></span> <span data-ttu-id="20560-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20560-132">Read-only.</span></span>|
|<span data-ttu-id="20560-133">displayName</span><span class="sxs-lookup"><span data-stu-id="20560-133">displayName</span></span>|<span data-ttu-id="20560-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20560-134">String</span></span>|<span data-ttu-id="20560-135">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="20560-135">Display name for the device category.</span></span>|
|<span data-ttu-id="20560-136">descrição</span><span class="sxs-lookup"><span data-stu-id="20560-136">description</span></span>|<span data-ttu-id="20560-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20560-137">String</span></span>|<span data-ttu-id="20560-138">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="20560-138">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="20560-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="20560-139">Response</span></span>
<span data-ttu-id="20560-140">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCategory](../resources/intune_shared_devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20560-140">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20560-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20560-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="20560-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20560-142">Request</span></span>
<span data-ttu-id="20560-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20560-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="20560-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="20560-144">Response</span></span>
<span data-ttu-id="20560-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20560-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



