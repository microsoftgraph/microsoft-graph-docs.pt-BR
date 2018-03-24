# <a name="get-androidforworkenrollmentprofile"></a><span data-ttu-id="fd009-101">Obter androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="fd009-101">Get androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="fd009-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fd009-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd009-103">Ler propriedades e relações do objeto [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="fd009-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd009-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd009-104">Prerequisites</span></span>
<span data-ttu-id="fd009-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd009-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd009-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd009-107">Permission type</span></span>|<span data-ttu-id="fd009-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd009-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd009-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd009-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fd009-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd009-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fd009-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd009-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd009-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd009-112">Not supported.</span></span>|
|<span data-ttu-id="fd009-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd009-113">Application</span></span>|<span data-ttu-id="fd009-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd009-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd009-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd009-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd009-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fd009-116">Optional query parameters</span></span>
<span data-ttu-id="fd009-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fd009-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fd009-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd009-118">Request headers</span></span>
|<span data-ttu-id="fd009-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd009-119">Header</span></span>|<span data-ttu-id="fd009-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fd009-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd009-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd009-121">Authorization</span></span>|<span data-ttu-id="fd009-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd009-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fd009-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd009-123">Accept</span></span>|<span data-ttu-id="fd009-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fd009-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd009-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd009-125">Request body</span></span>
<span data-ttu-id="fd009-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fd009-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd009-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd009-127">Response</span></span>
<span data-ttu-id="fd009-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd009-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd009-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd009-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd009-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd009-130">Request</span></span>
<span data-ttu-id="fd009-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd009-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="fd009-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd009-132">Response</span></span>
<span data-ttu-id="fd009-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd009-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 872

{
  "value": {
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
}
```



