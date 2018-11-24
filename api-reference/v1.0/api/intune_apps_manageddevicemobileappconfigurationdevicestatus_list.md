# <a name="list-manageddevicemobileappconfigurationdevicestatuses"></a><span data-ttu-id="c6c29-101">Lista managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c6c29-101">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="c6c29-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c6c29-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6c29-103">Lista as propriedades e os relacionamentos dos objetos [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="c6c29-103">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6c29-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c6c29-104">Prerequisites</span></span>
<span data-ttu-id="c6c29-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c6c29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c6c29-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6c29-107">Permission type</span></span>|<span data-ttu-id="c6c29-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c6c29-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6c29-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6c29-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c6c29-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6c29-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c6c29-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6c29-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6c29-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6c29-112">Not supported.</span></span>|
|<span data-ttu-id="c6c29-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6c29-113">Application</span></span>|<span data-ttu-id="c6c29-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6c29-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6c29-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6c29-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c6c29-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c29-116">Request headers</span></span>
|<span data-ttu-id="c6c29-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6c29-117">Header</span></span>|<span data-ttu-id="c6c29-118">Valor</span><span class="sxs-lookup"><span data-stu-id="c6c29-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6c29-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6c29-119">Authorization</span></span>|<span data-ttu-id="c6c29-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6c29-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6c29-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c6c29-121">Accept</span></span>|<span data-ttu-id="c6c29-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c6c29-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6c29-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c29-123">Request body</span></span>
<span data-ttu-id="c6c29-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6c29-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6c29-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6c29-125">Response</span></span>
<span data-ttu-id="c6c29-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6c29-126">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6c29-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6c29-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6c29-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c29-128">Request</span></span>
<span data-ttu-id="c6c29-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6c29-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="c6c29-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6c29-130">Response</span></span>
<span data-ttu-id="c6c29-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6c29-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 563

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
      "id": "477d3651-3651-477d-5136-7d4751367d47",
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



