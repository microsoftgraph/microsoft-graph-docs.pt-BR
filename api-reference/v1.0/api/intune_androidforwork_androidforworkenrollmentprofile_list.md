# <a name="list-androidforworkenrollmentprofiles"></a><span data-ttu-id="e1971-101">Listar androidForWorkEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="e1971-101">List androidForWorkEnrollmentProfiles</span></span>

> <span data-ttu-id="e1971-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e1971-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1971-103">Listar propriedades e relações dos objetos [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e1971-103">List properties and relationships of the [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1971-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1971-104">Prerequisites</span></span>
<span data-ttu-id="e1971-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e1971-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1971-107">Permission type</span></span>|<span data-ttu-id="e1971-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1971-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1971-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1971-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e1971-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1971-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e1971-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1971-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1971-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1971-112">Not supported.</span></span>|
|<span data-ttu-id="e1971-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1971-113">Application</span></span>|<span data-ttu-id="e1971-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1971-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1971-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1971-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e1971-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1971-116">Request headers</span></span>
|<span data-ttu-id="e1971-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1971-117">Header</span></span>|<span data-ttu-id="e1971-118">Valor</span><span class="sxs-lookup"><span data-stu-id="e1971-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1971-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1971-119">Authorization</span></span>|<span data-ttu-id="e1971-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1971-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e1971-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1971-121">Accept</span></span>|<span data-ttu-id="e1971-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e1971-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1971-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1971-123">Request body</span></span>
<span data-ttu-id="e1971-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1971-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1971-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1971-125">Response</span></span>
<span data-ttu-id="e1971-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1971-126">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1971-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1971-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1971-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1971-128">Request</span></span>
<span data-ttu-id="e1971-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1971-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="e1971-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1971-130">Response</span></span>
<span data-ttu-id="e1971-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1971-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 926

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
      "accountId": "Account Id value",
      "id": "e6742553-2553-e674-5325-74e6532574e6",
      "name": "Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "tokenValue": "Token Value value",
      "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
      "totalEnrollmentCount": 4,
      "enrolledDeviceCount": 3,
      "qrCode": "Qr Code value",
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ]
}
```



