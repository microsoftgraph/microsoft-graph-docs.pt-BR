# <a name="get-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="60488-101">Acessar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="60488-101">Get managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="60488-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="60488-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60488-103">Leia as propriedades e as relações do objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="60488-103">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60488-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60488-104">Prerequisites</span></span>
<span data-ttu-id="60488-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="60488-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="60488-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60488-107">Permission type</span></span>|<span data-ttu-id="60488-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60488-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60488-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60488-109">Delegated (work or school account)</span></span>|<span data-ttu-id="60488-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="60488-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="60488-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60488-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60488-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60488-112">Not supported.</span></span>|
|<span data-ttu-id="60488-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60488-113">Application</span></span>|<span data-ttu-id="60488-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60488-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60488-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60488-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60488-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="60488-116">Optional query parameters</span></span>
<span data-ttu-id="60488-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="60488-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="60488-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60488-118">Request headers</span></span>
|<span data-ttu-id="60488-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60488-119">Header</span></span>|<span data-ttu-id="60488-120">Valor</span><span class="sxs-lookup"><span data-stu-id="60488-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60488-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="60488-121">Authorization</span></span>|<span data-ttu-id="60488-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="60488-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60488-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60488-123">Accept</span></span>|<span data-ttu-id="60488-124">application/json</span><span class="sxs-lookup"><span data-stu-id="60488-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60488-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60488-125">Request body</span></span>
<span data-ttu-id="60488-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60488-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60488-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="60488-127">Response</span></span>
<span data-ttu-id="60488-128">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60488-128">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60488-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60488-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="60488-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60488-130">Request</span></span>
<span data-ttu-id="60488-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60488-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

### <a name="response"></a><span data-ttu-id="60488-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="60488-132">Response</span></span>
<span data-ttu-id="60488-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60488-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 383

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
    "id": "7b953742-3742-7b95-4237-957b4237957b",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```








