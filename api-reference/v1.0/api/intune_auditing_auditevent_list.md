# <a name="list-auditevents"></a><span data-ttu-id="f5c55-101">Listar auditEvents</span><span class="sxs-lookup"><span data-stu-id="f5c55-101">List auditEvents</span></span>

> <span data-ttu-id="f5c55-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f5c55-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5c55-103">Listar propriedades e relações dos objetos [auditEvent](../resources/intune_auditing_auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="f5c55-103">List properties and relationships of the [auditEvent](../resources/intune_auditing_auditevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5c55-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5c55-104">Prerequisites</span></span>
<span data-ttu-id="f5c55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f5c55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f5c55-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5c55-107">Permission type</span></span>|<span data-ttu-id="f5c55-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f5c55-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5c55-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5c55-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f5c55-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c55-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f5c55-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5c55-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5c55-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5c55-112">Not supported.</span></span>|
|<span data-ttu-id="f5c55-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5c55-113">Application</span></span>|<span data-ttu-id="f5c55-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5c55-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5c55-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5c55-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="f5c55-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c55-116">Request headers</span></span>
|<span data-ttu-id="f5c55-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5c55-117">Header</span></span>|<span data-ttu-id="f5c55-118">Valor</span><span class="sxs-lookup"><span data-stu-id="f5c55-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5c55-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5c55-119">Authorization</span></span>|<span data-ttu-id="f5c55-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="f5c55-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5c55-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5c55-121">Accept</span></span>|<span data-ttu-id="f5c55-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f5c55-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5c55-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c55-123">Request body</span></span>
<span data-ttu-id="f5c55-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5c55-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5c55-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5c55-125">Response</span></span>
<span data-ttu-id="f5c55-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [auditEvent](../resources/intune_auditing_auditevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5c55-126">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune_auditing_auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5c55-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5c55-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="f5c55-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c55-128">Request</span></span>
<span data-ttu-id="f5c55-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5c55-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="f5c55-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5c55-130">Response</span></span>
<span data-ttu-id="f5c55-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5c55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1629

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.auditEvent",
      "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
      "displayName": "Display Name value",
      "componentName": "Component Name value",
      "actor": {
        "@odata.type": "microsoft.graph.auditActor",
        "type": "Type value",
        "userPermissions": [
          "User Permissions value"
        ],
        "applicationId": "Application Id value",
        "applicationDisplayName": "Application Display Name value",
        "userPrincipalName": "User Principal Name value",
        "servicePrincipalName": "Service Principal Name value",
        "ipAddress": "Ip Address value",
        "userId": "User Id value"
      },
      "activity": "Activity value",
      "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
      "activityType": "Activity Type value",
      "activityOperationType": "Activity Operation Type value",
      "activityResult": "Activity Result value",
      "correlationId": "79199ed9-e50b-4257-8de4-70b9c8685061",
      "resources": [
        {
          "@odata.type": "microsoft.graph.auditResource",
          "displayName": "Display Name value",
          "modifiedProperties": [
            {
              "@odata.type": "microsoft.graph.auditProperty",
              "displayName": "Display Name value",
              "oldValue": "Old Value value",
              "newValue": "New Value value"
            }
          ],
          "type": "Type value",
          "resourceId": "Resource Id value"
        }
      ],
      "category": "Category value"
    }
  ]
}
```



