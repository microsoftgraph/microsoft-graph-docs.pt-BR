# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="ec979-101">Criar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="ec979-101">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="ec979-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ec979-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec979-103">Criar um novo objeto [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="ec979-103">Create a new [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ec979-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ec979-104">Prerequisites</span></span>
<span data-ttu-id="ec979-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ec979-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ec979-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec979-107">Permission type</span></span>|<span data-ttu-id="ec979-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ec979-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec979-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec979-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ec979-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec979-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ec979-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec979-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec979-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec979-112">Not supported.</span></span>|
|<span data-ttu-id="ec979-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec979-113">Application</span></span>|<span data-ttu-id="ec979-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec979-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec979-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec979-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ec979-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec979-116">Request headers</span></span>
|<span data-ttu-id="ec979-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec979-117">Header</span></span>|<span data-ttu-id="ec979-118">Valor</span><span class="sxs-lookup"><span data-stu-id="ec979-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec979-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec979-119">Authorization</span></span>|<span data-ttu-id="ec979-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="ec979-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec979-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ec979-121">Accept</span></span>|<span data-ttu-id="ec979-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ec979-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec979-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec979-123">Request body</span></span>
<span data-ttu-id="ec979-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="ec979-124">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="ec979-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="ec979-125">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="ec979-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec979-126">Property</span></span>|<span data-ttu-id="ec979-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec979-127">Type</span></span>|<span data-ttu-id="ec979-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec979-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec979-129">id</span><span class="sxs-lookup"><span data-stu-id="ec979-129">id</span></span>|<span data-ttu-id="ec979-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec979-130">String</span></span>|<span data-ttu-id="ec979-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ec979-131">Key of the entity.</span></span>|
|<span data-ttu-id="ec979-132">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="ec979-132">gracePeriodHours</span></span>|<span data-ttu-id="ec979-133">Int32</span><span class="sxs-lookup"><span data-stu-id="ec979-133">Int32</span></span>|<span data-ttu-id="ec979-134">Número de horas a aguardar até que a ação seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="ec979-134">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="ec979-135">Valores válidos de 0 a 8760</span><span class="sxs-lookup"><span data-stu-id="ec979-135">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="ec979-136">actionType</span><span class="sxs-lookup"><span data-stu-id="ec979-136">actionType</span></span>|[<span data-ttu-id="ec979-137">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="ec979-137">deviceComplianceActionType</span></span>](../resources/intune_deviceconfig_devicecomplianceactiontype.md)|<span data-ttu-id="ec979-138">Ação que será executada.</span><span class="sxs-lookup"><span data-stu-id="ec979-138">What action to take.</span></span> <span data-ttu-id="ec979-139">Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`.</span><span class="sxs-lookup"><span data-stu-id="ec979-139">The possible values are `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, , , , , , or .</span></span>|
|<span data-ttu-id="ec979-140">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="ec979-140">notificationTemplateId</span></span>|<span data-ttu-id="ec979-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec979-141">String</span></span>|<span data-ttu-id="ec979-142">Qual modelo de notificação de mensagem será usado</span><span class="sxs-lookup"><span data-stu-id="ec979-142">What notification Message template to use</span></span>|
|<span data-ttu-id="ec979-143">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="ec979-143">notificationMessageCCList</span></span>|<span data-ttu-id="ec979-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec979-144">String collection</span></span>|<span data-ttu-id="ec979-145">Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="ec979-145">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="ec979-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec979-146">Response</span></span>
<span data-ttu-id="ec979-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec979-147">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec979-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec979-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="ec979-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec979-149">Request</span></span>
<span data-ttu-id="ec979-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec979-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ec979-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec979-151">Response</span></span>
<span data-ttu-id="ec979-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec979-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 320

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```



