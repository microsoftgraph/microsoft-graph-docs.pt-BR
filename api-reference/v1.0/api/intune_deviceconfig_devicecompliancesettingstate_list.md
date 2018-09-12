# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="9570d-101">Listar deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="9570d-101">List deviceComplianceSettingStates</span></span>

> <span data-ttu-id="9570d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9570d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9570d-103">Listar propriedades e relações dos objetos [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="9570d-103">List properties and relationships of the [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9570d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9570d-104">Prerequisites</span></span>
<span data-ttu-id="9570d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9570d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9570d-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9570d-107">Permission type</span></span>|<span data-ttu-id="9570d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9570d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9570d-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9570d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9570d-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9570d-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9570d-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9570d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9570d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9570d-112">Not supported.</span></span>|
|<span data-ttu-id="9570d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9570d-113">Application</span></span>|<span data-ttu-id="9570d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9570d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9570d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9570d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="9570d-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9570d-116">Request headers</span></span>
|<span data-ttu-id="9570d-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9570d-117">Header</span></span>|<span data-ttu-id="9570d-118">Valor</span><span class="sxs-lookup"><span data-stu-id="9570d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9570d-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="9570d-119">Authorization</span></span>|<span data-ttu-id="9570d-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="9570d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9570d-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9570d-121">Accept</span></span>|<span data-ttu-id="9570d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9570d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9570d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9570d-123">Request body</span></span>
<span data-ttu-id="9570d-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9570d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9570d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="9570d-125">Response</span></span>
<span data-ttu-id="9570d-126">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9570d-126">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9570d-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9570d-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="9570d-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9570d-128">Request</span></span>
<span data-ttu-id="9570d-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9570d-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="9570d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9570d-130">Response</span></span>
<span data-ttu-id="9570d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9570d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "value": [
    {
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
  ]
}
```








