---
title: Atualizar deviceComplianceActionItem
description: Atualizar as propriedades de um objeto deviceComplianceActionItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fc49ee6822152f65886b7338c787781e3585e6f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443262"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="5ea7b-103">Atualizar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="5ea7b-103">Update deviceComplianceActionItem</span></span>

<span data-ttu-id="5ea7b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5ea7b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ea7b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ea7b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ea7b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ea7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ea7b-107">Atualizar as propriedades de um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="5ea7b-107">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ea7b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ea7b-108">Prerequisites</span></span>
<span data-ttu-id="5ea7b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ea7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ea7b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ea7b-111">Permission type</span></span>|<span data-ttu-id="5ea7b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ea7b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ea7b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ea7b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ea7b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ea7b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ea7b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ea7b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ea7b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ea7b-116">Not supported.</span></span>|
|<span data-ttu-id="5ea7b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ea7b-117">Application</span></span>|<span data-ttu-id="5ea7b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ea7b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ea7b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ea7b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="5ea7b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea7b-120">Request headers</span></span>
|<span data-ttu-id="5ea7b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ea7b-121">Header</span></span>|<span data-ttu-id="5ea7b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5ea7b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ea7b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ea7b-123">Authorization</span></span>|<span data-ttu-id="5ea7b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ea7b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ea7b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ea7b-125">Accept</span></span>|<span data-ttu-id="5ea7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ea7b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ea7b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea7b-127">Request body</span></span>
<span data-ttu-id="5ea7b-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="5ea7b-128">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="5ea7b-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="5ea7b-129">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="5ea7b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ea7b-130">Property</span></span>|<span data-ttu-id="5ea7b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ea7b-131">Type</span></span>|<span data-ttu-id="5ea7b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ea7b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ea7b-133">id</span><span class="sxs-lookup"><span data-stu-id="5ea7b-133">id</span></span>|<span data-ttu-id="5ea7b-134">String</span><span class="sxs-lookup"><span data-stu-id="5ea7b-134">String</span></span>|<span data-ttu-id="5ea7b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ea7b-135">Key of the entity.</span></span>|
|<span data-ttu-id="5ea7b-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="5ea7b-136">gracePeriodHours</span></span>|<span data-ttu-id="5ea7b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5ea7b-137">Int32</span></span>|<span data-ttu-id="5ea7b-138">Número de horas a aguardar até que a ação seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="5ea7b-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="5ea7b-139">Valores válidos de 0 a 8760</span><span class="sxs-lookup"><span data-stu-id="5ea7b-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="5ea7b-140">actionType</span><span class="sxs-lookup"><span data-stu-id="5ea7b-140">actionType</span></span>|[<span data-ttu-id="5ea7b-141">Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="5ea7b-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="5ea7b-142">Qual ação executar.</span><span class="sxs-lookup"><span data-stu-id="5ea7b-142">What action to take.</span></span> <span data-ttu-id="5ea7b-143">Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="5ea7b-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="5ea7b-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="5ea7b-144">notificationTemplateId</span></span>|<span data-ttu-id="5ea7b-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ea7b-145">String</span></span>|<span data-ttu-id="5ea7b-146">Qual modelo de notificação de mensagem será usado</span><span class="sxs-lookup"><span data-stu-id="5ea7b-146">What notification Message template to use</span></span>|
|<span data-ttu-id="5ea7b-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="5ea7b-147">notificationMessageCCList</span></span>|<span data-ttu-id="5ea7b-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ea7b-148">String collection</span></span>|<span data-ttu-id="5ea7b-149">Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="5ea7b-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="5ea7b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ea7b-150">Response</span></span>
<span data-ttu-id="5ea7b-151">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ea7b-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ea7b-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ea7b-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ea7b-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea7b-153">Request</span></span>
<span data-ttu-id="5ea7b-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ea7b-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
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

### <a name="response"></a><span data-ttu-id="5ea7b-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ea7b-155">Response</span></span>
<span data-ttu-id="5ea7b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ea7b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





