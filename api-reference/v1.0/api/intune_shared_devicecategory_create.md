# <a name="create-devicecategory"></a><span data-ttu-id="116e3-101">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="116e3-101">Create deviceCategory</span></span>

> <span data-ttu-id="116e3-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="116e3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="116e3-103">Cria um novo objeto [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="116e3-103">Create a new [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="116e3-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="116e3-104">Prerequisites</span></span>
<span data-ttu-id="116e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="116e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="116e3-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="116e3-107">Permission type</span></span>|<span data-ttu-id="116e3-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="116e3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="116e3-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="116e3-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="116e3-110">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="116e3-110">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="116e3-111">DeviceManagementManaged Devices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="116e3-111">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="116e3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="116e3-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="116e3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="116e3-113">Not supported.</span></span>|
|<span data-ttu-id="116e3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="116e3-114">Application</span></span>|<span data-ttu-id="116e3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="116e3-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="116e3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="116e3-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="116e3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="116e3-117">Request headers</span></span>
|<span data-ttu-id="116e3-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="116e3-118">Header</span></span>|<span data-ttu-id="116e3-119">Valor</span><span class="sxs-lookup"><span data-stu-id="116e3-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="116e3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="116e3-120">Authorization</span></span>|<span data-ttu-id="116e3-121">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="116e3-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="116e3-122">Accept</span><span class="sxs-lookup"><span data-stu-id="116e3-122">Accept</span></span>|<span data-ttu-id="116e3-123">application/json</span><span class="sxs-lookup"><span data-stu-id="116e3-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="116e3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="116e3-124">Request body</span></span>
<span data-ttu-id="116e3-125">No corpo da solicitação, forneça uma representação JSON do objeto deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="116e3-125">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="116e3-126">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="116e3-126">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="116e3-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="116e3-127">Property</span></span>|<span data-ttu-id="116e3-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="116e3-128">Type</span></span>|<span data-ttu-id="116e3-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="116e3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="116e3-130">id</span><span class="sxs-lookup"><span data-stu-id="116e3-130">id</span></span>|<span data-ttu-id="116e3-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="116e3-131">String</span></span>|<span data-ttu-id="116e3-132">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="116e3-132">Unique identifier for the device category.</span></span> <span data-ttu-id="116e3-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="116e3-133">Read-only.</span></span>|
|<span data-ttu-id="116e3-134">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="116e3-134">**Onboarding**</span></span>|
|<span data-ttu-id="116e3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="116e3-135">displayName</span></span>|<span data-ttu-id="116e3-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="116e3-136">String</span></span>|<span data-ttu-id="116e3-137">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="116e3-137">Display name for the device category.</span></span>|
|<span data-ttu-id="116e3-138">description</span><span class="sxs-lookup"><span data-stu-id="116e3-138">description</span></span>|<span data-ttu-id="116e3-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="116e3-139">String</span></span>|<span data-ttu-id="116e3-140">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="116e3-140">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="116e3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="116e3-141">Response</span></span>
<span data-ttu-id="116e3-142">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCategory](../resources/intune_shared_devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="116e3-142">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="116e3-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="116e3-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="116e3-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="116e3-144">Request</span></span>
<span data-ttu-id="116e3-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="116e3-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="116e3-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="116e3-146">Response</span></span>
<span data-ttu-id="116e3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="116e3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



