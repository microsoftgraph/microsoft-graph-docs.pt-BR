# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="1e78d-101">Get deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="1e78d-101">Get deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="1e78d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1e78d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e78d-103">Ler propriedades e relações do objeto [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="1e78d-103">Read properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e78d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e78d-104">Prerequisites</span></span>
<span data-ttu-id="1e78d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1e78d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1e78d-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e78d-107">Permission type</span></span>|<span data-ttu-id="1e78d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e78d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e78d-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e78d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1e78d-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e78d-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1e78d-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e78d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e78d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e78d-112">Not supported.</span></span>|
|<span data-ttu-id="1e78d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e78d-113">Application</span></span>|<span data-ttu-id="1e78d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e78d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e78d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e78d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1e78d-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1e78d-116">Optional query parameters</span></span>
<span data-ttu-id="1e78d-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1e78d-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1e78d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e78d-118">Request headers</span></span>
|<span data-ttu-id="1e78d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e78d-119">Header</span></span>|<span data-ttu-id="1e78d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1e78d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e78d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e78d-121">Authorization</span></span>|<span data-ttu-id="1e78d-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="1e78d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e78d-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e78d-123">Accept</span></span>|<span data-ttu-id="1e78d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1e78d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e78d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e78d-125">Request body</span></span>
<span data-ttu-id="1e78d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e78d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e78d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e78d-127">Response</span></span>
<span data-ttu-id="1e78d-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e78d-128">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e78d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e78d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e78d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e78d-130">Request</span></span>
<span data-ttu-id="1e78d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e78d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="1e78d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e78d-132">Response</span></span>
<span data-ttu-id="1e78d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e78d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
    "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```








