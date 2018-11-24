# <a name="list-devicecomplianceuserstatuses"></a><span data-ttu-id="dc2ee-101">Listar deviceComplianceUserStatuses</span><span class="sxs-lookup"><span data-stu-id="dc2ee-101">List deviceComplianceUserStatuses</span></span>

> <span data-ttu-id="dc2ee-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dc2ee-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc2ee-103">Listar propriedades e relações dos objetos [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="dc2ee-103">List properties and relationships of the [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc2ee-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc2ee-104">Prerequisites</span></span>
<span data-ttu-id="dc2ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dc2ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dc2ee-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc2ee-107">Permission type</span></span>|<span data-ttu-id="dc2ee-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc2ee-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc2ee-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc2ee-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dc2ee-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc2ee-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dc2ee-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc2ee-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc2ee-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc2ee-112">Not supported.</span></span>|
|<span data-ttu-id="dc2ee-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc2ee-113">Application</span></span>|<span data-ttu-id="dc2ee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc2ee-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc2ee-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc2ee-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="dc2ee-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc2ee-116">Request headers</span></span>
|<span data-ttu-id="dc2ee-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc2ee-117">Header</span></span>|<span data-ttu-id="dc2ee-118">Valor</span><span class="sxs-lookup"><span data-stu-id="dc2ee-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc2ee-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc2ee-119">Authorization</span></span>|<span data-ttu-id="dc2ee-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc2ee-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc2ee-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc2ee-121">Accept</span></span>|<span data-ttu-id="dc2ee-122">application/json</span><span class="sxs-lookup"><span data-stu-id="dc2ee-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc2ee-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc2ee-123">Request body</span></span>
<span data-ttu-id="dc2ee-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc2ee-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc2ee-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc2ee-125">Response</span></span>
<span data-ttu-id="dc2ee-126">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc2ee-126">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc2ee-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc2ee-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc2ee-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc2ee-128">Request</span></span>
<span data-ttu-id="dc2ee-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc2ee-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="dc2ee-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc2ee-130">Response</span></span>
<span data-ttu-id="dc2ee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc2ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 397

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
      "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



