---
title: Criar deviceComplianceActionItem
description: Criar um novo objeto deviceComplianceActionItem.
author: tfitzmac
ms.openlocfilehash: a4e0facb0a9d34d840b6ef737c09737c9a6626a4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317972"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="5840e-103">Criar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="5840e-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="5840e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5840e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5840e-105">Criar um novo objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="5840e-105">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5840e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5840e-106">Prerequisites</span></span>
<span data-ttu-id="5840e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5840e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5840e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5840e-109">Permission type</span></span>|<span data-ttu-id="5840e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5840e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5840e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5840e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5840e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5840e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5840e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5840e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5840e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5840e-114">Not supported.</span></span>|
|<span data-ttu-id="5840e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5840e-115">Application</span></span>|<span data-ttu-id="5840e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5840e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5840e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5840e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5840e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5840e-118">Request headers</span></span>
|<span data-ttu-id="5840e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5840e-119">Header</span></span>|<span data-ttu-id="5840e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5840e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5840e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5840e-121">Authorization</span></span>|<span data-ttu-id="5840e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5840e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5840e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5840e-123">Accept</span></span>|<span data-ttu-id="5840e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5840e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5840e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5840e-125">Request body</span></span>
<span data-ttu-id="5840e-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="5840e-126">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="5840e-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="5840e-127">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="5840e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5840e-128">Property</span></span>|<span data-ttu-id="5840e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="5840e-129">Type</span></span>|<span data-ttu-id="5840e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5840e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5840e-131">id</span><span class="sxs-lookup"><span data-stu-id="5840e-131">id</span></span>|<span data-ttu-id="5840e-132">String</span><span class="sxs-lookup"><span data-stu-id="5840e-132">String</span></span>|<span data-ttu-id="5840e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5840e-133">Key of the entity.</span></span>|
|<span data-ttu-id="5840e-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="5840e-134">gracePeriodHours</span></span>|<span data-ttu-id="5840e-135">Int32</span><span class="sxs-lookup"><span data-stu-id="5840e-135">Int32</span></span>|<span data-ttu-id="5840e-136">Número de horas a aguardar até que a ação seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="5840e-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="5840e-137">Valores válidos de 0 a 8760</span><span class="sxs-lookup"><span data-stu-id="5840e-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="5840e-138">actionType</span><span class="sxs-lookup"><span data-stu-id="5840e-138">actionType</span></span>|[<span data-ttu-id="5840e-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="5840e-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="5840e-140">Ação que será executada.</span><span class="sxs-lookup"><span data-stu-id="5840e-140">What action to take.</span></span> <span data-ttu-id="5840e-141">Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="5840e-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="5840e-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="5840e-142">notificationTemplateId</span></span>|<span data-ttu-id="5840e-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5840e-143">String</span></span>|<span data-ttu-id="5840e-144">Qual modelo de notificação de mensagem será usado</span><span class="sxs-lookup"><span data-stu-id="5840e-144">What notification Message template to use</span></span>|
|<span data-ttu-id="5840e-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="5840e-145">notificationMessageCCList</span></span>|<span data-ttu-id="5840e-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5840e-146">String collection</span></span>|<span data-ttu-id="5840e-147">Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="5840e-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="5840e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="5840e-148">Response</span></span>
<span data-ttu-id="5840e-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5840e-149">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5840e-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5840e-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="5840e-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5840e-151">Request</span></span>
<span data-ttu-id="5840e-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5840e-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5840e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="5840e-153">Response</span></span>
<span data-ttu-id="5840e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5840e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



