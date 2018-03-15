# <a name="get-managedmobilelobapp"></a><span data-ttu-id="e7578-101">Acessar managedMobileLobApp</span><span class="sxs-lookup"><span data-stu-id="e7578-101">Get managedMobileLobApp</span></span>

> <span data-ttu-id="e7578-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e7578-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7578-103">Leia as propriedades e as relações do objeto [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e7578-103">Read properties and relationships of [plannerPlanDetails](../resources/intune_apps_managedmobilelobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7578-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7578-104">Prerequisites</span></span>
<span data-ttu-id="e7578-p101">Uma das permissões a seguir é obrigatória para chamar esta API. Para saber mais, inclusive como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7578-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e7578-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7578-107">Permission type</span></span>|<span data-ttu-id="e7578-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7578-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7578-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7578-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e7578-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7578-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e7578-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7578-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7578-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7578-112">Not supported.</span></span>|
|<span data-ttu-id="e7578-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7578-113">Application</span></span>|<span data-ttu-id="e7578-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7578-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7578-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7578-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7578-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e7578-116">Optional query parameters</span></span>
<span data-ttu-id="e7578-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e7578-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e7578-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7578-118">Request headers</span></span>
|<span data-ttu-id="e7578-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7578-119">Header</span></span>|<span data-ttu-id="e7578-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e7578-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7578-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7578-121">Authorization</span></span>|<span data-ttu-id="e7578-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7578-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e7578-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7578-123">Accept</span></span>|<span data-ttu-id="e7578-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e7578-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7578-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7578-125">Request body</span></span>
<span data-ttu-id="e7578-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7578-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7578-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7578-127">Response</span></span>
<span data-ttu-id="e7578-128">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7578-128">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/intune_apps_managedmobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7578-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7578-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7578-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7578-130">Request</span></span>
<span data-ttu-id="e7578-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7578-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="e7578-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7578-132">Response</span></span>
<span data-ttu-id="e7578-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7578-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1007

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileLobApp",
    "id": "cded7cc4-7cc4-cded-c47c-edcdc47cedcd",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "publishingState": "processing",
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4
  }
}
```



