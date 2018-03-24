# <a name="get-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="321af-101">Obter managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="321af-101">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="321af-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="321af-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="321af-103">Ler propriedades e relações do objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="321af-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="321af-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="321af-104">Prerequisites</span></span>
<span data-ttu-id="321af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="321af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="321af-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="321af-107">Permission type</span></span>|<span data-ttu-id="321af-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="321af-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="321af-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="321af-109">Delegated (work or school account)</span></span>|<span data-ttu-id="321af-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="321af-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="321af-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="321af-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="321af-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="321af-112">Not supported.</span></span>|
|<span data-ttu-id="321af-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="321af-113">Application</span></span>|<span data-ttu-id="321af-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="321af-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="321af-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="321af-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="321af-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="321af-116">Optional query parameters</span></span>
<span data-ttu-id="321af-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="321af-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="321af-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="321af-118">Request headers</span></span>
|<span data-ttu-id="321af-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="321af-119">Header</span></span>|<span data-ttu-id="321af-120">Valor</span><span class="sxs-lookup"><span data-stu-id="321af-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="321af-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="321af-121">Authorization</span></span>|<span data-ttu-id="321af-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="321af-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="321af-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="321af-123">Accept</span></span>|<span data-ttu-id="321af-124">application/json</span><span class="sxs-lookup"><span data-stu-id="321af-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="321af-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="321af-125">Request body</span></span>
<span data-ttu-id="321af-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="321af-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="321af-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="321af-127">Response</span></span>
<span data-ttu-id="321af-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="321af-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="321af-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="321af-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="321af-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="321af-130">Request</span></span>
<span data-ttu-id="321af-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="321af-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

### <a name="response"></a><span data-ttu-id="321af-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="321af-132">Response</span></span>
<span data-ttu-id="321af-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="321af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
    "id": "9997c455-c455-9997-55c4-979955c49799",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```



