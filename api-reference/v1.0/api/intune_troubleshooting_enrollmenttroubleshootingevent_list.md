# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="d4f0b-101">Listar enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="d4f0b-101">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="d4f0b-102">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d4f0b-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4f0b-103">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d4f0b-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4f0b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d4f0b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4f0b-105">Lista propriedades e relações dos objetos [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="d4f0b-105">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4f0b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4f0b-106">Prerequisites</span></span>
<span data-ttu-id="d4f0b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d4f0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d4f0b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4f0b-109">Permission type</span></span>|<span data-ttu-id="d4f0b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4f0b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4f0b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4f0b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d4f0b-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4f0b-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d4f0b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4f0b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4f0b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4f0b-114">Not supported.</span></span>|
|<span data-ttu-id="d4f0b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4f0b-115">Application</span></span>|<span data-ttu-id="d4f0b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4f0b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4f0b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4f0b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="d4f0b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4f0b-118">Request headers</span></span>
|<span data-ttu-id="d4f0b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4f0b-119">Header</span></span>|<span data-ttu-id="d4f0b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d4f0b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4f0b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4f0b-121">Authorization</span></span>|<span data-ttu-id="d4f0b-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="d4f0b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4f0b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d4f0b-123">Accept</span></span>|<span data-ttu-id="d4f0b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d4f0b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4f0b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4f0b-125">Request body</span></span>
<span data-ttu-id="d4f0b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4f0b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4f0b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4f0b-127">Response</span></span>
<span data-ttu-id="d4f0b-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4f0b-128">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4f0b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4f0b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4f0b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4f0b-130">Request</span></span>
<span data-ttu-id="d4f0b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4f0b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="d4f0b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4f0b-132">Response</span></span>
<span data-ttu-id="d4f0b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4f0b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

{
  "value": [
    {
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
  ]
}
```



