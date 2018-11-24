# <a name="create-auditevent"></a><span data-ttu-id="863ae-101">Criar auditEvent</span><span class="sxs-lookup"><span data-stu-id="863ae-101">Create auditEvent</span></span>

> <span data-ttu-id="863ae-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="863ae-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="863ae-103">Criar um novo objeto [auditEvent](../resources/intune_auditing_auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="863ae-103">Create a new [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="863ae-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="863ae-104">Prerequisites</span></span>
<span data-ttu-id="863ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="863ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="863ae-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="863ae-107">Permission type</span></span>|<span data-ttu-id="863ae-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="863ae-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="863ae-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="863ae-109">Delegated (work or school account)</span></span>|<span data-ttu-id="863ae-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="863ae-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="863ae-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="863ae-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="863ae-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="863ae-112">Not supported.</span></span>|
|<span data-ttu-id="863ae-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="863ae-113">Application</span></span>|<span data-ttu-id="863ae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="863ae-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="863ae-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="863ae-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="863ae-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="863ae-116">Request headers</span></span>
|<span data-ttu-id="863ae-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="863ae-117">Header</span></span>|<span data-ttu-id="863ae-118">Valor</span><span class="sxs-lookup"><span data-stu-id="863ae-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="863ae-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="863ae-119">Authorization</span></span>|<span data-ttu-id="863ae-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="863ae-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="863ae-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="863ae-121">Accept</span></span>|<span data-ttu-id="863ae-122">application/json</span><span class="sxs-lookup"><span data-stu-id="863ae-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="863ae-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="863ae-123">Request body</span></span>
<span data-ttu-id="863ae-124">No corpo da solicitação, forneça uma representação JSON do objeto auditEvent.</span><span class="sxs-lookup"><span data-stu-id="863ae-124">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="863ae-125">A tabela a seguir mostra as propriedades que são necessárias ao criar auditEvent.</span><span class="sxs-lookup"><span data-stu-id="863ae-125">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="863ae-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="863ae-126">Property</span></span>|<span data-ttu-id="863ae-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="863ae-127">Type</span></span>|<span data-ttu-id="863ae-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="863ae-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="863ae-129">id</span><span class="sxs-lookup"><span data-stu-id="863ae-129">id</span></span>|<span data-ttu-id="863ae-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="863ae-130">String</span></span>|<span data-ttu-id="863ae-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="863ae-131">Key of the entity.</span></span>|
|<span data-ttu-id="863ae-132">displayName</span><span class="sxs-lookup"><span data-stu-id="863ae-132">displayName</span></span>|<span data-ttu-id="863ae-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="863ae-133">String</span></span>|<span data-ttu-id="863ae-134">Nome de exibição do evento.</span><span class="sxs-lookup"><span data-stu-id="863ae-134">Event display name.</span></span>|
|<span data-ttu-id="863ae-135">componentName</span><span class="sxs-lookup"><span data-stu-id="863ae-135">componentName</span></span>|<span data-ttu-id="863ae-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="863ae-136">String</span></span>|<span data-ttu-id="863ae-137">Nome do componente.</span><span class="sxs-lookup"><span data-stu-id="863ae-137">Component name.</span></span>|
|<span data-ttu-id="863ae-138">actor</span><span class="sxs-lookup"><span data-stu-id="863ae-138">actor</span></span>|[<span data-ttu-id="863ae-139">auditActor</span><span class="sxs-lookup"><span data-stu-id="863ae-139">auditActor</span></span>](../resources/intune_auditing_auditactor.md)|<span data-ttu-id="863ae-140">Usuários e aplicativos do AAD associados com o evento de auditoria.</span><span class="sxs-lookup"><span data-stu-id="863ae-140">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="863ae-141">atividade</span><span class="sxs-lookup"><span data-stu-id="863ae-141">activity</span></span>|<span data-ttu-id="863ae-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="863ae-142">String</span></span>|<span data-ttu-id="863ae-143">Nome amigável da atividade.</span><span class="sxs-lookup"><span data-stu-id="863ae-143">Friendly name of the activity.</span></span>|
|<span data-ttu-id="863ae-144">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="863ae-144">activityDateTime</span></span>|<span data-ttu-id="863ae-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="863ae-145">DateTimeOffset</span></span>|<span data-ttu-id="863ae-146">A hora e data em UTC em que a atividade foi executada.</span><span class="sxs-lookup"><span data-stu-id="863ae-146">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="863ae-147">activityType</span><span class="sxs-lookup"><span data-stu-id="863ae-147">activityType</span></span>|<span data-ttu-id="863ae-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="863ae-148">String</span></span>|<span data-ttu-id="863ae-149">O tipo de atividade que foi executada.</span><span class="sxs-lookup"><span data-stu-id="863ae-149">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="863ae-150">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="863ae-150">activityOperationType</span></span>|<span data-ttu-id="863ae-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="863ae-151">String</span></span>|<span data-ttu-id="863ae-152">O tipo de operação HTTP da atividade.</span><span class="sxs-lookup"><span data-stu-id="863ae-152">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="863ae-153">activityResult</span><span class="sxs-lookup"><span data-stu-id="863ae-153">activityResult</span></span>|<span data-ttu-id="863ae-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="863ae-154">String</span></span>|<span data-ttu-id="863ae-155">O resultado da atividade.</span><span class="sxs-lookup"><span data-stu-id="863ae-155">The result of the activity.</span></span>|
|<span data-ttu-id="863ae-156">correlationId</span><span class="sxs-lookup"><span data-stu-id="863ae-156">correlationId</span></span>|<span data-ttu-id="863ae-157">Guid</span><span class="sxs-lookup"><span data-stu-id="863ae-157">Guid</span></span>|<span data-ttu-id="863ae-158">A ID da solicitação de cliente usada para correlacionar a atividade dentro do sistema.</span><span class="sxs-lookup"><span data-stu-id="863ae-158">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="863ae-159">recursos</span><span class="sxs-lookup"><span data-stu-id="863ae-159">resources</span></span>|<span data-ttu-id="863ae-160">Coleção [auditResource](../resources/intune_auditing_auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="863ae-160">[auditResource](../resources/intune_auditing_auditresource.md) collection</span></span>|<span data-ttu-id="863ae-161">Recursos em modificação.</span><span class="sxs-lookup"><span data-stu-id="863ae-161">Resources being modified.</span></span>|
|<span data-ttu-id="863ae-162">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="863ae-162">category</span></span>|<span data-ttu-id="863ae-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="863ae-163">String</span></span>|<span data-ttu-id="863ae-164">Categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="863ae-164">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="863ae-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="863ae-165">Response</span></span>
<span data-ttu-id="863ae-166">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [auditEvent](../resources/intune_auditing_auditevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="863ae-166">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune_auditing_auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="863ae-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="863ae-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="863ae-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="863ae-168">Request</span></span>
<span data-ttu-id="863ae-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="863ae-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/auditEvents
Content-type: application/json
Content-length: 1390

{
  "@odata.type": "#microsoft.graph.auditEvent",
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
  "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
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
```

### <a name="response"></a><span data-ttu-id="863ae-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="863ae-170">Response</span></span>
<span data-ttu-id="863ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="863ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1439

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
  "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
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
```



