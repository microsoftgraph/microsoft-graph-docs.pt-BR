# <a name="get-windows10mobilecompliancepolicy"></a><span data-ttu-id="d0849-101">Obter windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d0849-101">Get windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="d0849-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d0849-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0849-103">Ler propriedades e relações do objeto [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d0849-103">Read properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d0849-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d0849-104">Prerequisites</span></span>
<span data-ttu-id="d0849-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d0849-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d0849-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0849-107">Permission type</span></span>|<span data-ttu-id="d0849-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d0849-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0849-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0849-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d0849-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0849-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d0849-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0849-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0849-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0849-112">Not supported.</span></span>|
|<span data-ttu-id="d0849-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0849-113">Application</span></span>|<span data-ttu-id="d0849-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0849-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0849-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0849-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0849-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d0849-116">Optional query parameters</span></span>
<span data-ttu-id="d0849-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d0849-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d0849-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0849-118">Request headers</span></span>
|<span data-ttu-id="d0849-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0849-119">Header</span></span>|<span data-ttu-id="d0849-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d0849-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0849-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0849-121">Authorization</span></span>|<span data-ttu-id="d0849-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="d0849-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0849-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d0849-123">Accept</span></span>|<span data-ttu-id="d0849-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d0849-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0849-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0849-125">Request body</span></span>
<span data-ttu-id="d0849-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0849-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0849-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0849-127">Response</span></span>
<span data-ttu-id="d0849-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0849-128">If successful, this method returns a `200 OK` response code and [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0849-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0849-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d0849-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0849-130">Request</span></span>
<span data-ttu-id="d0849-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0849-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="d0849-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0849-132">Response</span></span>
<span data-ttu-id="d0849-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0849-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1029

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
    "id": "3d4237b0-37b0-3d42-b037-423db037423d",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordMinimumLength": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "passwordExpirationDays": 6,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordRequireToUnlockFromIdle": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "earlyLaunchAntiMalwareDriverEnabled": true,
    "bitLockerEnabled": true,
    "secureBootEnabled": true,
    "codeIntegrityEnabled": true,
    "storageRequireEncryption": true
  }
}
```








