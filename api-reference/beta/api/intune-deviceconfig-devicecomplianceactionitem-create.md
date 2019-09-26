---
title: Criar deviceComplianceActionItem
description: Criar um novo objeto deviceComplianceActionItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a28005bc6633335cd6671cd8d1ead1afa9e1558b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37175233"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="c56b6-103">Criar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="c56b6-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="c56b6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c56b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c56b6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c56b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c56b6-106">Criar um novo objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="c56b6-106">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c56b6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c56b6-107">Prerequisites</span></span>
<span data-ttu-id="c56b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c56b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c56b6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c56b6-110">Permission type</span></span>|<span data-ttu-id="c56b6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c56b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c56b6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c56b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c56b6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c56b6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c56b6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c56b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c56b6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c56b6-115">Not supported.</span></span>|
|<span data-ttu-id="c56b6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c56b6-116">Application</span></span>|<span data-ttu-id="c56b6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c56b6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c56b6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c56b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c56b6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c56b6-119">Request headers</span></span>
|<span data-ttu-id="c56b6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c56b6-120">Header</span></span>|<span data-ttu-id="c56b6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c56b6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c56b6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c56b6-122">Authorization</span></span>|<span data-ttu-id="c56b6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c56b6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c56b6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c56b6-124">Accept</span></span>|<span data-ttu-id="c56b6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c56b6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c56b6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c56b6-126">Request body</span></span>
<span data-ttu-id="c56b6-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="c56b6-127">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="c56b6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="c56b6-128">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="c56b6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c56b6-129">Property</span></span>|<span data-ttu-id="c56b6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c56b6-130">Type</span></span>|<span data-ttu-id="c56b6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c56b6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c56b6-132">id</span><span class="sxs-lookup"><span data-stu-id="c56b6-132">id</span></span>|<span data-ttu-id="c56b6-133">String</span><span class="sxs-lookup"><span data-stu-id="c56b6-133">String</span></span>|<span data-ttu-id="c56b6-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c56b6-134">Key of the entity.</span></span>|
|<span data-ttu-id="c56b6-135">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="c56b6-135">gracePeriodHours</span></span>|<span data-ttu-id="c56b6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c56b6-136">Int32</span></span>|<span data-ttu-id="c56b6-137">Número de horas a aguardar até que a ação seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="c56b6-137">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="c56b6-138">Valores válidos de 0 a 8760</span><span class="sxs-lookup"><span data-stu-id="c56b6-138">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="c56b6-139">actionType</span><span class="sxs-lookup"><span data-stu-id="c56b6-139">actionType</span></span>|[<span data-ttu-id="c56b6-140">Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="c56b6-140">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="c56b6-141">Qual ação executar.</span><span class="sxs-lookup"><span data-stu-id="c56b6-141">What action to take.</span></span> <span data-ttu-id="c56b6-142">Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="c56b6-142">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="c56b6-143">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="c56b6-143">notificationTemplateId</span></span>|<span data-ttu-id="c56b6-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c56b6-144">String</span></span>|<span data-ttu-id="c56b6-145">Qual modelo de notificação de mensagem será usado</span><span class="sxs-lookup"><span data-stu-id="c56b6-145">What notification Message template to use</span></span>|
|<span data-ttu-id="c56b6-146">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="c56b6-146">notificationMessageCCList</span></span>|<span data-ttu-id="c56b6-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c56b6-147">String collection</span></span>|<span data-ttu-id="c56b6-148">Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="c56b6-148">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="c56b6-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c56b6-149">Response</span></span>
<span data-ttu-id="c56b6-150">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c56b6-150">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c56b6-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c56b6-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="c56b6-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c56b6-152">Request</span></span>
<span data-ttu-id="c56b6-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c56b6-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c56b6-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="c56b6-154">Response</span></span>
<span data-ttu-id="c56b6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c56b6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




