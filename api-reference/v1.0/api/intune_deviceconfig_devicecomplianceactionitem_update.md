# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="eede8-101">Atualizar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="eede8-101">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="eede8-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="eede8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eede8-103">Atualizar as propriedades de um objeto [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="eede8-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eede8-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eede8-104">Prerequisites</span></span>
<span data-ttu-id="eede8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eede8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eede8-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eede8-107">Permission type</span></span>|<span data-ttu-id="eede8-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eede8-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eede8-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eede8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="eede8-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eede8-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eede8-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eede8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eede8-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eede8-112">Not supported.</span></span>|
|<span data-ttu-id="eede8-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eede8-113">Application</span></span>|<span data-ttu-id="eede8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eede8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eede8-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eede8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="eede8-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eede8-116">Request headers</span></span>
|<span data-ttu-id="eede8-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eede8-117">Header</span></span>|<span data-ttu-id="eede8-118">Valor</span><span class="sxs-lookup"><span data-stu-id="eede8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eede8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="eede8-119">Authorization</span></span>|<span data-ttu-id="eede8-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eede8-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="eede8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="eede8-121">Accept</span></span>|<span data-ttu-id="eede8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="eede8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eede8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eede8-123">Request body</span></span>
<span data-ttu-id="eede8-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="eede8-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="eede8-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="eede8-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="eede8-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eede8-126">Property</span></span>|<span data-ttu-id="eede8-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="eede8-127">Type</span></span>|<span data-ttu-id="eede8-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="eede8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eede8-129">id</span><span class="sxs-lookup"><span data-stu-id="eede8-129">id</span></span>|<span data-ttu-id="eede8-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eede8-130">String</span></span>|<span data-ttu-id="eede8-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="eede8-131">Key of the setting.</span></span>|
|<span data-ttu-id="eede8-132">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="eede8-132">gracePeriodHours</span></span>|<span data-ttu-id="eede8-133">Int32</span><span class="sxs-lookup"><span data-stu-id="eede8-133">Int32</span></span>|<span data-ttu-id="eede8-134">Número de horas a aguardar até que a ação seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="eede8-134">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="eede8-135">Valores válidos de 0 a 8760</span><span class="sxs-lookup"><span data-stu-id="eede8-135">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="eede8-136">actionType</span><span class="sxs-lookup"><span data-stu-id="eede8-136">actionType</span></span>|<span data-ttu-id="eede8-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eede8-137">String</span></span>|<span data-ttu-id="eede8-138">Qual ação será executada Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`.</span><span class="sxs-lookup"><span data-stu-id="eede8-138">What action to take Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`.</span></span>|
|<span data-ttu-id="eede8-139">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="eede8-139">notificationTemplateId</span></span>|<span data-ttu-id="eede8-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eede8-140">String</span></span>|<span data-ttu-id="eede8-141">Qual modelo de notificação de mensagem será usado</span><span class="sxs-lookup"><span data-stu-id="eede8-141">What notification Message template to use</span></span>|
|<span data-ttu-id="eede8-142">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="eede8-142">notificationMessageCCList</span></span>|<span data-ttu-id="eede8-143">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eede8-143">String collection</span></span>|<span data-ttu-id="eede8-144">Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="eede8-144">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="eede8-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="eede8-145">Response</span></span>
<span data-ttu-id="eede8-146">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eede8-146">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eede8-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eede8-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="eede8-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eede8-148">Request</span></span>
<span data-ttu-id="eede8-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eede8-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
Content-type: application/json
Content-length: 206

{
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="eede8-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="eede8-150">Response</span></span>
<span data-ttu-id="eede8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eede8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



