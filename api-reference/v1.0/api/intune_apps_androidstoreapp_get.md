# <a name="get-androidstoreapp"></a><span data-ttu-id="56a93-101">Get androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="56a93-101">Get androidStoreApp</span></span>

> <span data-ttu-id="56a93-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="56a93-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56a93-103">Ler propriedades e relações do objeto [androidStoreApp](../resources/intune_apps_androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="56a93-103">Read properties and relationships of the [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56a93-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56a93-104">Prerequisites</span></span>
<span data-ttu-id="56a93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="56a93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="56a93-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56a93-107">Permission type</span></span>|<span data-ttu-id="56a93-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56a93-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56a93-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56a93-109">Delegated (work or school account)</span></span>|<span data-ttu-id="56a93-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="56a93-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="56a93-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56a93-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56a93-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56a93-112">Not supported.</span></span>|
|<span data-ttu-id="56a93-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56a93-113">Application</span></span>|<span data-ttu-id="56a93-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56a93-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56a93-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56a93-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56a93-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="56a93-116">Optional query parameters</span></span>
<span data-ttu-id="56a93-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="56a93-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="56a93-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56a93-118">Request headers</span></span>
|<span data-ttu-id="56a93-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56a93-119">Header</span></span>|<span data-ttu-id="56a93-120">Valor</span><span class="sxs-lookup"><span data-stu-id="56a93-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56a93-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="56a93-121">Authorization</span></span>|<span data-ttu-id="56a93-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56a93-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56a93-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="56a93-123">Accept</span></span>|<span data-ttu-id="56a93-124">application/json</span><span class="sxs-lookup"><span data-stu-id="56a93-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56a93-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56a93-125">Request body</span></span>
<span data-ttu-id="56a93-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56a93-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56a93-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="56a93-127">Response</span></span>
<span data-ttu-id="56a93-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidStoreApp](../resources/intune_apps_androidstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56a93-128">If successful, this method returns a `200 OK` response code and [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56a93-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56a93-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="56a93-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56a93-130">Request</span></span>
<span data-ttu-id="56a93-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56a93-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="56a93-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="56a93-132">Response</span></span>
<span data-ttu-id="56a93-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56a93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1193

{
  "value": {
    "@odata.type": "#microsoft.graph.androidStoreApp",
    "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
    "packageId": "Package Id value",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true
    }
  }
}
```



