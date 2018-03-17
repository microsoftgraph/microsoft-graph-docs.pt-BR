# <a name="get-auditevent"></a><span data-ttu-id="2fa3d-101">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="2fa3d-101">Get auditEvent</span></span>

> <span data-ttu-id="2fa3d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2fa3d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fa3d-103">Ler propriedades e relações do objeto [auditEvent](../resources/intune_auditing_auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="2fa3d-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_auditing_auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2fa3d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2fa3d-104">Prerequisites</span></span>
<span data-ttu-id="2fa3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2fa3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2fa3d-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fa3d-107">Permission type</span></span>|<span data-ttu-id="2fa3d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2fa3d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fa3d-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fa3d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2fa3d-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2fa3d-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2fa3d-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fa3d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fa3d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fa3d-112">Not supported.</span></span>|
|<span data-ttu-id="2fa3d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fa3d-113">Application</span></span>|<span data-ttu-id="2fa3d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fa3d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fa3d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fa3d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2fa3d-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2fa3d-116">Optional query parameters</span></span>
<span data-ttu-id="2fa3d-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2fa3d-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2fa3d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fa3d-118">Request headers</span></span>
|<span data-ttu-id="2fa3d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2fa3d-119">Header</span></span>|<span data-ttu-id="2fa3d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2fa3d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fa3d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fa3d-121">Authorization</span></span>|<span data-ttu-id="2fa3d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fa3d-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2fa3d-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2fa3d-123">Accept</span></span>|<span data-ttu-id="2fa3d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2fa3d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fa3d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fa3d-125">Request body</span></span>
<span data-ttu-id="2fa3d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2fa3d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fa3d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fa3d-127">Response</span></span>
<span data-ttu-id="2fa3d-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [auditEvent](../resources/intune_auditing_auditevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fa3d-128">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/intune_auditing_auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fa3d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fa3d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2fa3d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fa3d-130">Request</span></span>
<span data-ttu-id="2fa3d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fa3d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="2fa3d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fa3d-132">Response</span></span>
<span data-ttu-id="2fa3d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fa3d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1598

{
  "value": {
    "@odata.type": "#microsoft.graph.auditEvent",
    "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
    "displayName": "Display Name value",
    "componentName": "Component Name value",
    "actor": {
      "@odata.type": "microsoft.graph.auditActor",
      "type": "Type value",
      "permissions": [
        "Permissions value"
      ],
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
    "correlationId": "<Unknown Primitive Type Edm.Guid>",
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
}
```



