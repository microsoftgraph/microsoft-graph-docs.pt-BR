---
title: Atualizar deviceComplianceActionItem
description: Atualizar as propriedades de um objeto deviceComplianceActionItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26f673b8abdf9bb99d417eb9fbcb7e3565324081
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048061"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="86fed-103">Atualizar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="86fed-103">Update deviceComplianceActionItem</span></span>

<span data-ttu-id="86fed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86fed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86fed-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86fed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86fed-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86fed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86fed-107">Atualizar as propriedades de um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="86fed-107">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86fed-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86fed-108">Prerequisites</span></span>
<span data-ttu-id="86fed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86fed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86fed-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86fed-111">Permission type</span></span>|<span data-ttu-id="86fed-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86fed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86fed-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86fed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86fed-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86fed-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86fed-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86fed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86fed-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86fed-116">Not supported.</span></span>|
|<span data-ttu-id="86fed-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86fed-117">Application</span></span>|<span data-ttu-id="86fed-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86fed-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86fed-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86fed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="86fed-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86fed-120">Request headers</span></span>
|<span data-ttu-id="86fed-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86fed-121">Header</span></span>|<span data-ttu-id="86fed-122">Valor</span><span class="sxs-lookup"><span data-stu-id="86fed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86fed-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="86fed-123">Authorization</span></span>|<span data-ttu-id="86fed-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86fed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86fed-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86fed-125">Accept</span></span>|<span data-ttu-id="86fed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86fed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86fed-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86fed-127">Request body</span></span>
<span data-ttu-id="86fed-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="86fed-128">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="86fed-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="86fed-129">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="86fed-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86fed-130">Property</span></span>|<span data-ttu-id="86fed-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="86fed-131">Type</span></span>|<span data-ttu-id="86fed-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="86fed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86fed-133">id</span><span class="sxs-lookup"><span data-stu-id="86fed-133">id</span></span>|<span data-ttu-id="86fed-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86fed-134">String</span></span>|<span data-ttu-id="86fed-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="86fed-135">Key of the entity.</span></span>|
|<span data-ttu-id="86fed-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="86fed-136">gracePeriodHours</span></span>|<span data-ttu-id="86fed-137">Int32</span><span class="sxs-lookup"><span data-stu-id="86fed-137">Int32</span></span>|<span data-ttu-id="86fed-138">Número de horas a aguardar até que a ação seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="86fed-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="86fed-139">Valores válidos de 0 a 8760</span><span class="sxs-lookup"><span data-stu-id="86fed-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="86fed-140">actionType</span><span class="sxs-lookup"><span data-stu-id="86fed-140">actionType</span></span>|[<span data-ttu-id="86fed-141">Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="86fed-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="86fed-142">Qual ação executar.</span><span class="sxs-lookup"><span data-stu-id="86fed-142">What action to take.</span></span> <span data-ttu-id="86fed-143">Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="86fed-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="86fed-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="86fed-144">notificationTemplateId</span></span>|<span data-ttu-id="86fed-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86fed-145">String</span></span>|<span data-ttu-id="86fed-146">Qual modelo de notificação de mensagem será usado</span><span class="sxs-lookup"><span data-stu-id="86fed-146">What notification Message template to use</span></span>|
|<span data-ttu-id="86fed-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="86fed-147">notificationMessageCCList</span></span>|<span data-ttu-id="86fed-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="86fed-148">String collection</span></span>|<span data-ttu-id="86fed-149">Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="86fed-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="86fed-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="86fed-150">Response</span></span>
<span data-ttu-id="86fed-151">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86fed-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86fed-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86fed-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="86fed-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86fed-153">Request</span></span>
<span data-ttu-id="86fed-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86fed-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="86fed-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="86fed-155">Response</span></span>
<span data-ttu-id="86fed-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86fed-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






