# <a name="get-devicecompliancepolicy"></a><span data-ttu-id="38447-101">Acessar deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="38447-101">Get deviceCompliancePolicy</span></span>

> <span data-ttu-id="38447-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="38447-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38447-103">Leia as propriedades e as relações do objeto [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="38447-103">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38447-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38447-104">Prerequisites</span></span>
<span data-ttu-id="38447-p101">Uma das permissões a seguir é obrigatória para chamar esta API. Para saber mais, inclusive como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="38447-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="38447-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38447-107">Permission type</span></span>|<span data-ttu-id="38447-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38447-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38447-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38447-109">Delegated (work or school account)</span></span>|<span data-ttu-id="38447-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38447-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="38447-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38447-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38447-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38447-112">Not supported.</span></span>|
|<span data-ttu-id="38447-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38447-113">Application</span></span>|<span data-ttu-id="38447-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38447-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38447-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38447-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38447-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="38447-116">Optional query parameters</span></span>
<span data-ttu-id="38447-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="38447-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="38447-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38447-118">Request headers</span></span>
|<span data-ttu-id="38447-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38447-119">Header</span></span>|<span data-ttu-id="38447-120">Valor</span><span class="sxs-lookup"><span data-stu-id="38447-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38447-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="38447-121">Authorization</span></span>|<span data-ttu-id="38447-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38447-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38447-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38447-123">Accept</span></span>|<span data-ttu-id="38447-124">application/json</span><span class="sxs-lookup"><span data-stu-id="38447-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38447-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38447-125">Request body</span></span>
<span data-ttu-id="38447-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38447-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38447-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="38447-127">Response</span></span>
<span data-ttu-id="38447-128">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38447-128">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38447-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38447-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="38447-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38447-130">Request</span></span>
<span data-ttu-id="38447-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38447-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="38447-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="38447-132">Response</span></span>
<span data-ttu-id="38447-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38447-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 365

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
    "id": "4214b716-b716-4214-16b7-144216b71442",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



