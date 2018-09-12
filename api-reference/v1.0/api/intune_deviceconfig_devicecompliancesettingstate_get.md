# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="789ba-101">Acessar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="789ba-101">Get deviceComplianceSettingState</span></span>

> <span data-ttu-id="789ba-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="789ba-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="789ba-103">Leia as propriedades e as relações do objeto [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="789ba-103">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="789ba-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="789ba-104">Prerequisites</span></span>
<span data-ttu-id="789ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="789ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="789ba-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="789ba-107">Permission type</span></span>|<span data-ttu-id="789ba-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="789ba-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="789ba-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="789ba-109">Delegated (work or school account)</span></span>|<span data-ttu-id="789ba-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="789ba-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="789ba-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="789ba-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="789ba-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="789ba-112">Not supported.</span></span>|
|<span data-ttu-id="789ba-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="789ba-113">Application</span></span>|<span data-ttu-id="789ba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="789ba-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="789ba-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="789ba-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="789ba-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="789ba-116">Optional query parameters</span></span>
<span data-ttu-id="789ba-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="789ba-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="789ba-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="789ba-118">Request headers</span></span>
|<span data-ttu-id="789ba-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="789ba-119">Header</span></span>|<span data-ttu-id="789ba-120">Valor</span><span class="sxs-lookup"><span data-stu-id="789ba-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="789ba-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="789ba-121">Authorization</span></span>|<span data-ttu-id="789ba-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="789ba-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="789ba-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="789ba-123">Accept</span></span>|<span data-ttu-id="789ba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="789ba-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="789ba-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="789ba-125">Request body</span></span>
<span data-ttu-id="789ba-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="789ba-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="789ba-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="789ba-127">Response</span></span>
<span data-ttu-id="789ba-128">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="789ba-128">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="789ba-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="789ba-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="789ba-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="789ba-130">Request</span></span>
<span data-ttu-id="789ba-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="789ba-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="789ba-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="789ba-132">Response</span></span>
<span data-ttu-id="789ba-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="789ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
    "id": "9905f955-f955-9905-55f9-059955f90599",
    "setting": "Setting value",
    "settingName": "Setting Name value",
    "deviceId": "Device Id value",
    "deviceName": "Device Name value",
    "userId": "User Id value",
    "userEmail": "User Email value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value",
    "deviceModel": "Device Model value",
    "state": "notApplicable",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
  }
}
```








