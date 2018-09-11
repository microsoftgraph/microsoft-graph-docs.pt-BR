# <a name="get-mobilelobapp"></a><span data-ttu-id="3a533-101">Acessar mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="3a533-101">Get mobileLobApp</span></span>

> <span data-ttu-id="3a533-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3a533-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a533-103">Leia as propriedades e as relações do objeto [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a533-103">Read properties and relationships of the [mobileLobApp](../resources/intune_apps_mobilelobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3a533-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3a533-104">Prerequisites</span></span>
<span data-ttu-id="3a533-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3a533-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3a533-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a533-107">Permission type</span></span>|<span data-ttu-id="3a533-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3a533-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a533-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a533-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3a533-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a533-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3a533-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a533-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a533-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a533-112">Not supported.</span></span>|
|<span data-ttu-id="3a533-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a533-113">Application</span></span>|<span data-ttu-id="3a533-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a533-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a533-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a533-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a533-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3a533-116">Optional query parameters</span></span>
<span data-ttu-id="3a533-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3a533-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3a533-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a533-118">Request headers</span></span>
|<span data-ttu-id="3a533-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a533-119">Header</span></span>|<span data-ttu-id="3a533-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3a533-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a533-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a533-121">Authorization</span></span>|<span data-ttu-id="3a533-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="3a533-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a533-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3a533-123">Accept</span></span>|<span data-ttu-id="3a533-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3a533-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a533-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a533-125">Request body</span></span>
<span data-ttu-id="3a533-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a533-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a533-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a533-127">Response</span></span>
<span data-ttu-id="3a533-128">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileLobApp](../resources/intune_apps_mobilelobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a533-128">If successful, this method returns a `200 OK` response code and [mobileLobApp](../resources/intune_apps_mobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a533-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a533-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a533-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a533-130">Request</span></span>
<span data-ttu-id="3a533-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a533-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="3a533-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a533-132">Response</span></span>
<span data-ttu-id="3a533-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a533-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 925

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileLobApp",
    "id": "2fc11935-1935-2fc1-3519-c12f3519c12f",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4
  }
}
```








