# <a name="get-devicecategory"></a><span data-ttu-id="fa4dc-101">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="fa4dc-101">Get deviceCategory</span></span>

> <span data-ttu-id="fa4dc-102">**Importante:** as APIs na versão /beta no Microsoft Graph estão em versão prévia e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fa4dc-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa4dc-103">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fa4dc-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa4dc-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fa4dc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa4dc-105">Ler propriedades de leitura e relações do objeto [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="fa4dc-105">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa4dc-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fa4dc-106">Prerequisites</span></span>
<span data-ttu-id="fa4dc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa4dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fa4dc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa4dc-109">Permission type</span></span>|<span data-ttu-id="fa4dc-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fa4dc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa4dc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa4dc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa4dc-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa4dc-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fa4dc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa4dc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa4dc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa4dc-114">Not supported.</span></span>|
|<span data-ttu-id="fa4dc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa4dc-115">Application</span></span>|<span data-ttu-id="fa4dc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa4dc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa4dc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa4dc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa4dc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fa4dc-118">Optional query parameters</span></span>
<span data-ttu-id="fa4dc-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fa4dc-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa4dc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa4dc-120">Request headers</span></span>
|<span data-ttu-id="fa4dc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa4dc-121">Header</span></span>|<span data-ttu-id="fa4dc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fa4dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa4dc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa4dc-123">Authorization</span></span>|<span data-ttu-id="fa4dc-124">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="fa4dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa4dc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fa4dc-125">Accept</span></span>|<span data-ttu-id="fa4dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa4dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa4dc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa4dc-127">Request body</span></span>
<span data-ttu-id="fa4dc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa4dc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa4dc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa4dc-129">Response</span></span>
<span data-ttu-id="fa4dc-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune_shared_devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa4dc-130">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa4dc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa4dc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa4dc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa4dc-132">Request</span></span>
<span data-ttu-id="fa4dc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa4dc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="fa4dc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa4dc-134">Response</span></span>
<span data-ttu-id="fa4dc-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa4dc-135">Here is an example of the response.</span></span> <span data-ttu-id="fa4dc-136">Observação: o objeto resposta mostrado aqui pode estar truncado por motivo de concisão.</span><span class="sxs-lookup"><span data-stu-id="fa4dc-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fa4dc-137">Propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="fa4dc-137">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 211

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCategory",
    "id": "f881b841-b841-f881-41b8-81f841b881f8",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```



