---
title: Atualizar deviceComplianceActionItem
description: Atualizar as propriedades de um objeto deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c5a80c04ced36a87519217d135257cad640fc29b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861191"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="9b10b-103">Atualizar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9b10b-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="9b10b-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9b10b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b10b-105">Atualizar as propriedades de um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="9b10b-105">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b10b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9b10b-106">Prerequisites</span></span>
<span data-ttu-id="9b10b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b10b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b10b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b10b-109">Permission type</span></span>|<span data-ttu-id="9b10b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9b10b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b10b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b10b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9b10b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b10b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b10b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b10b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b10b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b10b-114">Not supported.</span></span>|
|<span data-ttu-id="9b10b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b10b-115">Application</span></span>|<span data-ttu-id="9b10b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b10b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b10b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b10b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="9b10b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b10b-118">Request headers</span></span>
|<span data-ttu-id="9b10b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b10b-119">Header</span></span>|<span data-ttu-id="9b10b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9b10b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b10b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b10b-121">Authorization</span></span>|<span data-ttu-id="9b10b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b10b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b10b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9b10b-123">Accept</span></span>|<span data-ttu-id="9b10b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9b10b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b10b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b10b-125">Request body</span></span>
<span data-ttu-id="9b10b-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="9b10b-126">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="9b10b-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="9b10b-127">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="9b10b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b10b-128">Property</span></span>|<span data-ttu-id="9b10b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b10b-129">Type</span></span>|<span data-ttu-id="9b10b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b10b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b10b-131">id</span><span class="sxs-lookup"><span data-stu-id="9b10b-131">id</span></span>|<span data-ttu-id="9b10b-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b10b-132">String</span></span>|<span data-ttu-id="9b10b-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9b10b-133">Key of the entity.</span></span>|
|<span data-ttu-id="9b10b-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="9b10b-134">gracePeriodHours</span></span>|<span data-ttu-id="9b10b-135">Int32</span><span class="sxs-lookup"><span data-stu-id="9b10b-135">Int32</span></span>|<span data-ttu-id="9b10b-136">Número de horas a aguardar até que a ação seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="9b10b-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="9b10b-137">Valores válidos de 0 a 8760</span><span class="sxs-lookup"><span data-stu-id="9b10b-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="9b10b-138">actionType</span><span class="sxs-lookup"><span data-stu-id="9b10b-138">actionType</span></span>|[<span data-ttu-id="9b10b-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="9b10b-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="9b10b-140">Ação que será executada.</span><span class="sxs-lookup"><span data-stu-id="9b10b-140">What action to take.</span></span> <span data-ttu-id="9b10b-141">Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="9b10b-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="9b10b-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="9b10b-142">notificationTemplateId</span></span>|<span data-ttu-id="9b10b-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b10b-143">String</span></span>|<span data-ttu-id="9b10b-144">Qual modelo de notificação de mensagem será usado</span><span class="sxs-lookup"><span data-stu-id="9b10b-144">What notification Message template to use</span></span>|
|<span data-ttu-id="9b10b-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="9b10b-145">notificationMessageCCList</span></span>|<span data-ttu-id="9b10b-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b10b-146">String collection</span></span>|<span data-ttu-id="9b10b-147">Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="9b10b-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="9b10b-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b10b-148">Response</span></span>
<span data-ttu-id="9b10b-149">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b10b-149">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b10b-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b10b-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b10b-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b10b-151">Request</span></span>
<span data-ttu-id="9b10b-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b10b-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
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

### <a name="response"></a><span data-ttu-id="9b10b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b10b-153">Response</span></span>
<span data-ttu-id="9b10b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b10b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



