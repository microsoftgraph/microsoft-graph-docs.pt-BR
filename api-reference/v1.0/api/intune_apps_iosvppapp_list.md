# <a name="list-iosvppapps"></a><span data-ttu-id="6258d-101">Listar iosVppApps</span><span class="sxs-lookup"><span data-stu-id="6258d-101">List iosVppApps</span></span>

> <span data-ttu-id="6258d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6258d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6258d-103">Listar propriedades e relações dos objetos [iosVppApp](../resources/intune_apps_iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="6258d-103">List properties and relationships of the [iosVppApp](../resources/intune_apps_iosvppapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6258d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6258d-104">Prerequisites</span></span>
<span data-ttu-id="6258d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6258d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6258d-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6258d-107">Permission type</span></span>|<span data-ttu-id="6258d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6258d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6258d-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6258d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6258d-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6258d-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6258d-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6258d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6258d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6258d-112">Not supported.</span></span>|
|<span data-ttu-id="6258d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6258d-113">Application</span></span>|<span data-ttu-id="6258d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6258d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6258d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6258d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6258d-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6258d-116">Request headers</span></span>
|<span data-ttu-id="6258d-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6258d-117">Header</span></span>|<span data-ttu-id="6258d-118">Valor</span><span class="sxs-lookup"><span data-stu-id="6258d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6258d-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="6258d-119">Authorization</span></span>|<span data-ttu-id="6258d-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6258d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6258d-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6258d-121">Accept</span></span>|<span data-ttu-id="6258d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6258d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6258d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6258d-123">Request body</span></span>
<span data-ttu-id="6258d-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6258d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6258d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="6258d-125">Response</span></span>
<span data-ttu-id="6258d-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosVppApp](../resources/intune_apps_iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6258d-126">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/intune_apps_iosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6258d-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6258d-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="6258d-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6258d-128">Request</span></span>
<span data-ttu-id="6258d-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6258d-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="6258d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6258d-130">Response</span></span>
<span data-ttu-id="6258d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6258d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1575

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppApp",
      "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "licensingType": {
        "@odata.type": "microsoft.graph.vppLicensingType",
        "supportsUserLicensing": true,
        "supportsDeviceLicensing": true
      },
      "applicableDeviceType": {
        "@odata.type": "microsoft.graph.iosDeviceType",
        "iPad": true,
        "iPhoneAndIPod": true
      },
      "vppTokenOrganizationName": "Vpp Token Organization Name value",
      "vppTokenAccountType": "education",
      "vppTokenAppleId": "Vpp Token Apple Id value",
      "bundleId": "Bundle Id value"
    }
  ]
}
```



