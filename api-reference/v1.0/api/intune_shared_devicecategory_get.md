# <a name="get-devicecategory"></a><span data-ttu-id="37021-101">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="37021-101">Get deviceCategory</span></span>



> <span data-ttu-id="37021-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="37021-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37021-103">Ler propriedades de leitura e relações do objeto [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="37021-103">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37021-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37021-104">Prerequisites</span></span>
<span data-ttu-id="37021-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="37021-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="37021-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37021-107">Permission type</span></span>|<span data-ttu-id="37021-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37021-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37021-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37021-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="37021-110">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="37021-110">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="37021-111">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="37021-111">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="37021-112">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="37021-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="37021-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="37021-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="37021-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37021-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37021-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37021-115">Not supported.</span></span>|
|<span data-ttu-id="37021-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37021-116">Application</span></span>|<span data-ttu-id="37021-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37021-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37021-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37021-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37021-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="37021-119">Optional query parameters</span></span>
<span data-ttu-id="37021-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="37021-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37021-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37021-121">Request headers</span></span>
|<span data-ttu-id="37021-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37021-122">Header</span></span>|<span data-ttu-id="37021-123">Valor</span><span class="sxs-lookup"><span data-stu-id="37021-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37021-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="37021-124">Authorization</span></span>|<span data-ttu-id="37021-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37021-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37021-126">Accept</span><span class="sxs-lookup"><span data-stu-id="37021-126">Accept</span></span>|<span data-ttu-id="37021-127">application/json</span><span class="sxs-lookup"><span data-stu-id="37021-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37021-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37021-128">Request body</span></span>
<span data-ttu-id="37021-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37021-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37021-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="37021-130">Response</span></span>
<span data-ttu-id="37021-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune_shared_devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37021-131">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37021-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37021-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="37021-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37021-133">Request</span></span>
<span data-ttu-id="37021-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37021-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="37021-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="37021-135">Response</span></span>
<span data-ttu-id="37021-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37021-136">Here is an example of the response.</span></span> <span data-ttu-id="37021-137">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="37021-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="37021-138">Propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="37021-138">Properties returned from an actual call vary according to context.</span></span>

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



