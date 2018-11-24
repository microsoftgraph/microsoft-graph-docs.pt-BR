# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="e12cf-101">Get enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e12cf-101">Get enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="e12cf-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e12cf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e12cf-103">Propriedades de leitura e relações do objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e12cf-103">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e12cf-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e12cf-104">Prerequisites</span></span>
<span data-ttu-id="e12cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e12cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e12cf-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e12cf-107">Permission type</span></span>|<span data-ttu-id="e12cf-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e12cf-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e12cf-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e12cf-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e12cf-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e12cf-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e12cf-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e12cf-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e12cf-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e12cf-112">Not supported.</span></span>|
|<span data-ttu-id="e12cf-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e12cf-113">Application</span></span>|<span data-ttu-id="e12cf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e12cf-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e12cf-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e12cf-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e12cf-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e12cf-116">Optional query parameters</span></span>
<span data-ttu-id="e12cf-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e12cf-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e12cf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e12cf-118">Request headers</span></span>
|<span data-ttu-id="e12cf-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e12cf-119">Header</span></span>|<span data-ttu-id="e12cf-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e12cf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e12cf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e12cf-121">Authorization</span></span>|<span data-ttu-id="e12cf-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e12cf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e12cf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e12cf-123">Accept</span></span>|<span data-ttu-id="e12cf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e12cf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e12cf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e12cf-125">Request body</span></span>
<span data-ttu-id="e12cf-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e12cf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e12cf-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e12cf-127">Response</span></span>
<span data-ttu-id="e12cf-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e12cf-128">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e12cf-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e12cf-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e12cf-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e12cf-130">Request</span></span>
<span data-ttu-id="e12cf-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e12cf-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="e12cf-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e12cf-132">Response</span></span>
<span data-ttu-id="e12cf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e12cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 601

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
    "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value",
    "managedDeviceIdentifier": "Managed Device Identifier value",
    "operatingSystem": "Operating System value",
    "osVersion": "Os Version value",
    "userId": "User Id value",
    "deviceId": "Device Id value",
    "enrollmentType": "userEnrollment",
    "failureCategory": "authentication",
    "failureReason": "Failure Reason value"
  }
}
```



