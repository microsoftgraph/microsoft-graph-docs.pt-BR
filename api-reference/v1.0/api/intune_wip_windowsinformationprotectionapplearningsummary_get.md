# <a name="get-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="71f9b-101">Obter windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="71f9b-101">Get windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="71f9b-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="71f9b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71f9b-103">Ler propriedades e relações do objeto [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="71f9b-103">Read properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71f9b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71f9b-104">Prerequisites</span></span>
<span data-ttu-id="71f9b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71f9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71f9b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71f9b-107">Permission type</span></span>|<span data-ttu-id="71f9b-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71f9b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71f9b-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71f9b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="71f9b-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="71f9b-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="71f9b-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71f9b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71f9b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71f9b-112">Not supported.</span></span>|
|<span data-ttu-id="71f9b-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71f9b-113">Application</span></span>|<span data-ttu-id="71f9b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71f9b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71f9b-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71f9b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71f9b-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="71f9b-116">Optional query parameters</span></span>
<span data-ttu-id="71f9b-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="71f9b-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="71f9b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71f9b-118">Request headers</span></span>
|<span data-ttu-id="71f9b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71f9b-119">Header</span></span>|<span data-ttu-id="71f9b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="71f9b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71f9b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="71f9b-121">Authorization</span></span>|<span data-ttu-id="71f9b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71f9b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71f9b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71f9b-123">Accept</span></span>|<span data-ttu-id="71f9b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="71f9b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71f9b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71f9b-125">Request body</span></span>
<span data-ttu-id="71f9b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71f9b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71f9b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="71f9b-127">Response</span></span>
<span data-ttu-id="71f9b-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71f9b-128">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71f9b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71f9b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="71f9b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71f9b-130">Request</span></span>
<span data-ttu-id="71f9b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71f9b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="71f9b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="71f9b-132">Response</span></span>
<span data-ttu-id="71f9b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71f9b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
    "id": "063baf50-af50-063b-50af-3b0650af3b06",
    "applicationName": "Application Name value",
    "applicationType": "desktop",
    "deviceCount": 11
  }
}
```



