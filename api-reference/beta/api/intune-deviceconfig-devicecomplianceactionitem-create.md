---
title: Criar deviceComplianceActionItem
description: Criar um novo objeto deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfbccac27a5c3adee6c972c1ae7ad2fa541b410a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807599"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="fc805-103">Criar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="fc805-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="fc805-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc805-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc805-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc805-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc805-106">Criar um novo objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="fc805-106">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc805-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fc805-107">Prerequisites</span></span>
<span data-ttu-id="fc805-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc805-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc805-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc805-110">Permission type</span></span>|<span data-ttu-id="fc805-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fc805-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc805-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc805-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc805-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc805-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc805-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc805-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc805-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc805-115">Not supported.</span></span>|
|<span data-ttu-id="fc805-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc805-116">Application</span></span>|<span data-ttu-id="fc805-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc805-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc805-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc805-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fc805-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc805-119">Request headers</span></span>
|<span data-ttu-id="fc805-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc805-120">Header</span></span>|<span data-ttu-id="fc805-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fc805-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc805-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc805-122">Authorization</span></span>|<span data-ttu-id="fc805-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc805-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc805-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fc805-124">Accept</span></span>|<span data-ttu-id="fc805-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc805-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc805-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc805-126">Request body</span></span>
<span data-ttu-id="fc805-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="fc805-127">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="fc805-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="fc805-128">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="fc805-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc805-129">Property</span></span>|<span data-ttu-id="fc805-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc805-130">Type</span></span>|<span data-ttu-id="fc805-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc805-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc805-132">id</span><span class="sxs-lookup"><span data-stu-id="fc805-132">id</span></span>|<span data-ttu-id="fc805-133">String</span><span class="sxs-lookup"><span data-stu-id="fc805-133">String</span></span>|<span data-ttu-id="fc805-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fc805-134">Key of the entity.</span></span>|
|<span data-ttu-id="fc805-135">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="fc805-135">gracePeriodHours</span></span>|<span data-ttu-id="fc805-136">Int32</span><span class="sxs-lookup"><span data-stu-id="fc805-136">Int32</span></span>|<span data-ttu-id="fc805-137">Número de horas a aguardar até que a ação seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="fc805-137">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="fc805-138">Valores válidos de 0 a 8760</span><span class="sxs-lookup"><span data-stu-id="fc805-138">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="fc805-139">actionType</span><span class="sxs-lookup"><span data-stu-id="fc805-139">actionType</span></span>|[<span data-ttu-id="fc805-140">Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="fc805-140">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="fc805-141">Qual ação executar.</span><span class="sxs-lookup"><span data-stu-id="fc805-141">What action to take.</span></span> <span data-ttu-id="fc805-142">Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="fc805-142">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="fc805-143">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="fc805-143">notificationTemplateId</span></span>|<span data-ttu-id="fc805-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc805-144">String</span></span>|<span data-ttu-id="fc805-145">Qual modelo de notificação de mensagem será usado</span><span class="sxs-lookup"><span data-stu-id="fc805-145">What notification Message template to use</span></span>|
|<span data-ttu-id="fc805-146">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="fc805-146">notificationMessageCCList</span></span>|<span data-ttu-id="fc805-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc805-147">String collection</span></span>|<span data-ttu-id="fc805-148">Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="fc805-148">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="fc805-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc805-149">Response</span></span>
<span data-ttu-id="fc805-150">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc805-150">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc805-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc805-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc805-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc805-152">Request</span></span>
<span data-ttu-id="fc805-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc805-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
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

### <a name="response"></a><span data-ttu-id="fc805-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc805-154">Response</span></span>
<span data-ttu-id="fc805-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc805-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





