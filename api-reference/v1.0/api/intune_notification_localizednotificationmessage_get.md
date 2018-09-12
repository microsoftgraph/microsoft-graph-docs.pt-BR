# <a name="get-localizednotificationmessage"></a><span data-ttu-id="72992-101">Obter localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="72992-101">Get localizedNotificationMessage</span></span>

> <span data-ttu-id="72992-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="72992-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72992-103">Ler propriedades e relações do objeto [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="72992-103">Read properties and relationships of the [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="72992-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72992-104">Prerequisites</span></span>
<span data-ttu-id="72992-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="72992-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="72992-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72992-107">Permission type</span></span>|<span data-ttu-id="72992-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="72992-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72992-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72992-109">Delegated (work or school account)</span></span>|<span data-ttu-id="72992-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="72992-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="72992-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72992-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72992-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72992-112">Not supported.</span></span>|
|<span data-ttu-id="72992-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72992-113">Application</span></span>|<span data-ttu-id="72992-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72992-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72992-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72992-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72992-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="72992-116">Optional query parameters</span></span>
<span data-ttu-id="72992-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="72992-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="72992-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72992-118">Request headers</span></span>
|<span data-ttu-id="72992-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72992-119">Header</span></span>|<span data-ttu-id="72992-120">Valor</span><span class="sxs-lookup"><span data-stu-id="72992-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72992-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="72992-121">Authorization</span></span>|<span data-ttu-id="72992-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="72992-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72992-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="72992-123">Accept</span></span>|<span data-ttu-id="72992-124">application/json</span><span class="sxs-lookup"><span data-stu-id="72992-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72992-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72992-125">Request body</span></span>
<span data-ttu-id="72992-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72992-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72992-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="72992-127">Response</span></span>
<span data-ttu-id="72992-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72992-128">If successful, this method returns a `200 OK` response code and [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72992-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72992-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="72992-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72992-130">Request</span></span>
<span data-ttu-id="72992-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72992-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="72992-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="72992-132">Response</span></span>
<span data-ttu-id="72992-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72992-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.localizedNotificationMessage",
    "id": "7a777708-7708-7a77-0877-777a0877777a",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "locale": "Locale value",
    "subject": "Subject value",
    "messageTemplate": "Message Template value",
    "isDefault": true
  }
}
```








