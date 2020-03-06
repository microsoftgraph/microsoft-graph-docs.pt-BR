---
title: Atualizar deviceComplianceActionItem
description: Atualizar as propriedades de um objeto deviceComplianceActionItem.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 112a9f77af4ea5daba53253002a239d93fc374b6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515144"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="47717-103">Atualizar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="47717-103">Update deviceComplianceActionItem</span></span>

<span data-ttu-id="47717-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47717-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47717-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47717-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47717-106">Atualizar as propriedades de um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="47717-106">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47717-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47717-107">Prerequisites</span></span>
<span data-ttu-id="47717-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47717-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47717-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47717-110">Permission type</span></span>|<span data-ttu-id="47717-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47717-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47717-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47717-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47717-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47717-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47717-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47717-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47717-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47717-115">Not supported.</span></span>|
|<span data-ttu-id="47717-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47717-116">Application</span></span>|<span data-ttu-id="47717-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47717-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47717-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47717-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="47717-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47717-119">Request headers</span></span>
|<span data-ttu-id="47717-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47717-120">Header</span></span>|<span data-ttu-id="47717-121">Valor</span><span class="sxs-lookup"><span data-stu-id="47717-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47717-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="47717-122">Authorization</span></span>|<span data-ttu-id="47717-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47717-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47717-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47717-124">Accept</span></span>|<span data-ttu-id="47717-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47717-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47717-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47717-126">Request body</span></span>
<span data-ttu-id="47717-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="47717-127">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="47717-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="47717-128">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="47717-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47717-129">Property</span></span>|<span data-ttu-id="47717-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="47717-130">Type</span></span>|<span data-ttu-id="47717-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="47717-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47717-132">id</span><span class="sxs-lookup"><span data-stu-id="47717-132">id</span></span>|<span data-ttu-id="47717-133">String</span><span class="sxs-lookup"><span data-stu-id="47717-133">String</span></span>|<span data-ttu-id="47717-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="47717-134">Key of the entity.</span></span>|
|<span data-ttu-id="47717-135">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="47717-135">gracePeriodHours</span></span>|<span data-ttu-id="47717-136">Int32</span><span class="sxs-lookup"><span data-stu-id="47717-136">Int32</span></span>|<span data-ttu-id="47717-137">Número de horas a aguardar até que a ação seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="47717-137">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="47717-138">Valores válidos de 0 a 8760</span><span class="sxs-lookup"><span data-stu-id="47717-138">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="47717-139">actionType</span><span class="sxs-lookup"><span data-stu-id="47717-139">actionType</span></span>|[<span data-ttu-id="47717-140">Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="47717-140">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="47717-141">Qual ação executar.</span><span class="sxs-lookup"><span data-stu-id="47717-141">What action to take.</span></span> <span data-ttu-id="47717-142">Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="47717-142">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="47717-143">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="47717-143">notificationTemplateId</span></span>|<span data-ttu-id="47717-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47717-144">String</span></span>|<span data-ttu-id="47717-145">Qual modelo de notificação de mensagem será usado</span><span class="sxs-lookup"><span data-stu-id="47717-145">What notification Message template to use</span></span>|
|<span data-ttu-id="47717-146">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="47717-146">notificationMessageCCList</span></span>|<span data-ttu-id="47717-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="47717-147">String collection</span></span>|<span data-ttu-id="47717-148">Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="47717-148">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="47717-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="47717-149">Response</span></span>
<span data-ttu-id="47717-150">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47717-150">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47717-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47717-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="47717-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47717-152">Request</span></span>
<span data-ttu-id="47717-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47717-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47717-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="47717-154">Response</span></span>
<span data-ttu-id="47717-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47717-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




