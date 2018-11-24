# <a name="list-iosvppebooks"></a><span data-ttu-id="84d27-101">Listar iosVppEBooks</span><span class="sxs-lookup"><span data-stu-id="84d27-101">List iosVppEBooks</span></span>

> <span data-ttu-id="84d27-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="84d27-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84d27-103">Listar propriedades e relações dos objetos [iosVppEBook](../resources/intune_books_iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="84d27-103">List properties and relationships of the [iosVppEBook](../resources/intune_books_iosvppebook.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84d27-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84d27-104">Prerequisites</span></span>
<span data-ttu-id="84d27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="84d27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="84d27-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84d27-107">Permission type</span></span>|<span data-ttu-id="84d27-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84d27-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84d27-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84d27-109">Delegated (work or school account)</span></span>|<span data-ttu-id="84d27-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="84d27-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="84d27-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84d27-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84d27-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84d27-112">Not supported.</span></span>|
|<span data-ttu-id="84d27-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84d27-113">Application</span></span>|<span data-ttu-id="84d27-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84d27-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84d27-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84d27-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="84d27-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84d27-116">Request headers</span></span>
|<span data-ttu-id="84d27-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84d27-117">Header</span></span>|<span data-ttu-id="84d27-118">Valor</span><span class="sxs-lookup"><span data-stu-id="84d27-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84d27-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="84d27-119">Authorization</span></span>|<span data-ttu-id="84d27-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84d27-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84d27-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84d27-121">Accept</span></span>|<span data-ttu-id="84d27-122">application/json</span><span class="sxs-lookup"><span data-stu-id="84d27-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84d27-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84d27-123">Request body</span></span>
<span data-ttu-id="84d27-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="84d27-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84d27-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="84d27-125">Response</span></span>
<span data-ttu-id="84d27-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosVppEBook](../resources/intune_books_iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84d27-126">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune_books_iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84d27-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84d27-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="84d27-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84d27-128">Request</span></span>
<span data-ttu-id="84d27-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84d27-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="84d27-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="84d27-130">Response</span></span>
<span data-ttu-id="84d27-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84d27-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1097

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppEBook",
      "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
      "largeCover": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "informationUrl": "https://example.com/informationUrl/",
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
      "appleId": "Apple Id value",
      "vppOrganizationName": "Vpp Organization Name value",
      "genres": [
        "Genres value"
      ],
      "language": "Language value",
      "seller": "Seller value",
      "totalLicenseCount": 1,
      "usedLicenseCount": 0
    }
  ]
}
```



