# <a name="get-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="e3f54-101">Acessar managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="e3f54-101">Get managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="e3f54-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e3f54-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3f54-103">Leia as propriedades e as relações do objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="e3f54-103">Read properties and relationships of [plannerProgressTaskBoardTaskFormat](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3f54-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3f54-104">Prerequisites</span></span>
<span data-ttu-id="e3f54-p101">Uma das permissões a seguir é obrigatória para chamar esta API. Para saber mais, inclusive como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3f54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e3f54-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3f54-107">Permission type</span></span>|<span data-ttu-id="e3f54-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3f54-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3f54-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3f54-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e3f54-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3f54-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e3f54-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3f54-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3f54-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3f54-112">Not supported.</span></span>|
|<span data-ttu-id="e3f54-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3f54-113">Application</span></span>|<span data-ttu-id="e3f54-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3f54-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3f54-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3f54-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3f54-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e3f54-116">Optional query parameters</span></span>
<span data-ttu-id="e3f54-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e3f54-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e3f54-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3f54-118">Request headers</span></span>
|<span data-ttu-id="e3f54-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3f54-119">Header</span></span>|<span data-ttu-id="e3f54-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e3f54-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3f54-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3f54-121">Authorization</span></span>|<span data-ttu-id="e3f54-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3f54-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e3f54-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3f54-123">Accept</span></span>|<span data-ttu-id="e3f54-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e3f54-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3f54-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3f54-125">Request body</span></span>
<span data-ttu-id="e3f54-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3f54-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3f54-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3f54-127">Response</span></span>
<span data-ttu-id="e3f54-128">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3f54-128">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3f54-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3f54-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3f54-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3f54-130">Request</span></span>
<span data-ttu-id="e3f54-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3f54-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="e3f54-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3f54-132">Response</span></span>
<span data-ttu-id="e3f54-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3f54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 388

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
    "id": "44960944-0944-4496-4409-964444099644",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



