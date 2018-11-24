# <a name="get-windowsphone81compliancepolicy"></a><span data-ttu-id="b2253-101">Get windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b2253-101">Get windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="b2253-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b2253-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2253-103">Ler propriedades e relações do objeto [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b2253-103">Read properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2253-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2253-104">Prerequisites</span></span>
<span data-ttu-id="b2253-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b2253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b2253-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2253-107">Permission type</span></span>|<span data-ttu-id="b2253-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2253-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2253-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2253-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b2253-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2253-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b2253-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2253-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2253-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2253-112">Not supported.</span></span>|
|<span data-ttu-id="b2253-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2253-113">Application</span></span>|<span data-ttu-id="b2253-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2253-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2253-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2253-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b2253-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b2253-116">Optional query parameters</span></span>
<span data-ttu-id="b2253-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b2253-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b2253-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2253-118">Request headers</span></span>
|<span data-ttu-id="b2253-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2253-119">Header</span></span>|<span data-ttu-id="b2253-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b2253-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2253-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2253-121">Authorization</span></span>|<span data-ttu-id="b2253-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2253-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2253-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2253-123">Accept</span></span>|<span data-ttu-id="b2253-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b2253-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2253-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2253-125">Request body</span></span>
<span data-ttu-id="b2253-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b2253-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2253-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2253-127">Response</span></span>
<span data-ttu-id="b2253-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2253-128">If successful, this method returns a `200 OK` response code and [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2253-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2253-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b2253-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2253-130">Request</span></span>
<span data-ttu-id="b2253-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2253-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="b2253-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2253-132">Response</span></span>
<span data-ttu-id="b2253-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2253-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 834

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
    "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "storageRequireEncryption": true
  }
}
```



