# <a name="get-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="e9020-101">Acessar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e9020-101">Get deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="e9020-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e9020-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9020-103">Leia as propriedades e as relações do objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e9020-103">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e9020-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9020-104">Prerequisites</span></span>
<span data-ttu-id="e9020-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e9020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e9020-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9020-107">Permission type</span></span>|<span data-ttu-id="e9020-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e9020-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9020-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9020-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e9020-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9020-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e9020-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9020-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9020-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9020-112">Not supported.</span></span>|
|<span data-ttu-id="e9020-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9020-113">Application</span></span>|<span data-ttu-id="e9020-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9020-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9020-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9020-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9020-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9020-116">Optional query parameters</span></span>
<span data-ttu-id="e9020-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9020-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e9020-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9020-118">Request headers</span></span>
|<span data-ttu-id="e9020-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9020-119">Header</span></span>|<span data-ttu-id="e9020-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e9020-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9020-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9020-121">Authorization</span></span>|<span data-ttu-id="e9020-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="e9020-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9020-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9020-123">Accept</span></span>|<span data-ttu-id="e9020-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e9020-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9020-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9020-125">Request body</span></span>
<span data-ttu-id="e9020-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9020-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9020-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9020-127">Response</span></span>
<span data-ttu-id="e9020-128">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9020-128">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9020-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9020-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e9020-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9020-130">Request</span></span>
<span data-ttu-id="e9020-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9020-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

### <a name="response"></a><span data-ttu-id="e9020-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9020-132">Response</span></span>
<span data-ttu-id="e9020-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9020-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
    "inGracePeriodCount": 2,
    "configManagerCount": 2,
    "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
    "unknownDeviceCount": 2,
    "notApplicableDeviceCount": 8,
    "compliantDeviceCount": 4,
    "remediatedDeviceCount": 5,
    "nonCompliantDeviceCount": 7,
    "errorDeviceCount": 0,
    "conflictDeviceCount": 3
  }
}
```








