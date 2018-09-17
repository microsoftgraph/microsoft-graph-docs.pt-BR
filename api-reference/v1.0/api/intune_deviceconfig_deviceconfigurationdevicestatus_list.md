# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="1f42c-101">Listar deviceConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="1f42c-101">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="1f42c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1f42c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f42c-103">Listar propriedades e relações dos objetos [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="1f42c-103">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f42c-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1f42c-104">Prerequisites</span></span>
<span data-ttu-id="1f42c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f42c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1f42c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f42c-107">Permission type</span></span>|<span data-ttu-id="1f42c-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1f42c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f42c-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f42c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1f42c-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f42c-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1f42c-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f42c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f42c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f42c-112">Not supported.</span></span>|
|<span data-ttu-id="1f42c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f42c-113">Application</span></span>|<span data-ttu-id="1f42c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f42c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f42c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f42c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="1f42c-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f42c-116">Request headers</span></span>
|<span data-ttu-id="1f42c-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f42c-117">Header</span></span>|<span data-ttu-id="1f42c-118">Valor</span><span class="sxs-lookup"><span data-stu-id="1f42c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f42c-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f42c-119">Authorization</span></span>|<span data-ttu-id="1f42c-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="1f42c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f42c-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1f42c-121">Accept</span></span>|<span data-ttu-id="1f42c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1f42c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f42c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f42c-123">Request body</span></span>
<span data-ttu-id="1f42c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f42c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f42c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f42c-125">Response</span></span>
<span data-ttu-id="1f42c-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f42c-126">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f42c-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f42c-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f42c-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f42c-128">Request</span></span>
<span data-ttu-id="1f42c-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f42c-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="1f42c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f42c-130">Response</span></span>
<span data-ttu-id="1f42c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f42c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
      "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```








