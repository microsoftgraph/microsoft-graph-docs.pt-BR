# <a name="get-devicecategory"></a><span data-ttu-id="9e394-101">Acessar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="9e394-101">Get deviceCategory</span></span>

> <span data-ttu-id="9e394-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9e394-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e394-103">Leia as propriedades e as relações do objeto [deviceCategory](../resources/intune_devices_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="9e394-103">Read properties and relationships of [plannerPlanDetails](../resources/intune_devices_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e394-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e394-104">Prerequisites</span></span>
<span data-ttu-id="9e394-p101">Uma das permissões a seguir é obrigatória para chamar esta API. Para saber mais, inclusive como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9e394-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9e394-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e394-107">Permission type</span></span>|<span data-ttu-id="9e394-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9e394-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e394-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e394-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9e394-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e394-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9e394-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e394-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e394-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e394-112">Not supported.</span></span>|
|<span data-ttu-id="9e394-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e394-113">Application</span></span>|<span data-ttu-id="9e394-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e394-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e394-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e394-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e394-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9e394-116">Optional query parameters</span></span>
<span data-ttu-id="9e394-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e394-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9e394-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e394-118">Request headers</span></span>
|<span data-ttu-id="9e394-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e394-119">Header</span></span>|<span data-ttu-id="9e394-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9e394-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e394-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e394-121">Authorization</span></span>|<span data-ttu-id="9e394-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e394-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9e394-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e394-123">Accept</span></span>|<span data-ttu-id="9e394-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9e394-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e394-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e394-125">Request body</span></span>
<span data-ttu-id="9e394-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e394-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e394-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e394-127">Response</span></span>
<span data-ttu-id="9e394-128">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceCategory](../resources/intune_devices_devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e394-128">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/intune_devices_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e394-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e394-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e394-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e394-130">Request</span></span>
<span data-ttu-id="9e394-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e394-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

### <a name="response"></a><span data-ttu-id="9e394-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e394-132">Response</span></span>
<span data-ttu-id="9e394-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e394-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 128

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCategory",
    "id": "f881b841-b841-f881-41b8-81f841b881f8"
  }
}
```



