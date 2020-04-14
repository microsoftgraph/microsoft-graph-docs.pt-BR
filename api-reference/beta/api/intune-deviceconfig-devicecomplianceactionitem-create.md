---
title: Criar deviceComplianceActionItem
description: Criar um novo objeto deviceComplianceActionItem.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 09018eb527351ddae552899727afc8b5edb5a763
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43434279"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="cec8e-103">Criar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="cec8e-103">Create deviceComplianceActionItem</span></span>

<span data-ttu-id="cec8e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cec8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cec8e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cec8e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cec8e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cec8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cec8e-107">Criar um novo objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="cec8e-107">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cec8e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cec8e-108">Prerequisites</span></span>
<span data-ttu-id="cec8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cec8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cec8e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cec8e-111">Permission type</span></span>|<span data-ttu-id="cec8e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cec8e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cec8e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cec8e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cec8e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cec8e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cec8e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cec8e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cec8e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cec8e-116">Not supported.</span></span>|
|<span data-ttu-id="cec8e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cec8e-117">Application</span></span>|<span data-ttu-id="cec8e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cec8e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cec8e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cec8e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cec8e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cec8e-120">Request headers</span></span>
|<span data-ttu-id="cec8e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cec8e-121">Header</span></span>|<span data-ttu-id="cec8e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cec8e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cec8e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cec8e-123">Authorization</span></span>|<span data-ttu-id="cec8e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cec8e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cec8e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cec8e-125">Accept</span></span>|<span data-ttu-id="cec8e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cec8e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cec8e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cec8e-127">Request body</span></span>
<span data-ttu-id="cec8e-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="cec8e-128">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="cec8e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="cec8e-129">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="cec8e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cec8e-130">Property</span></span>|<span data-ttu-id="cec8e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cec8e-131">Type</span></span>|<span data-ttu-id="cec8e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cec8e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cec8e-133">id</span><span class="sxs-lookup"><span data-stu-id="cec8e-133">id</span></span>|<span data-ttu-id="cec8e-134">String</span><span class="sxs-lookup"><span data-stu-id="cec8e-134">String</span></span>|<span data-ttu-id="cec8e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cec8e-135">Key of the entity.</span></span>|
|<span data-ttu-id="cec8e-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="cec8e-136">gracePeriodHours</span></span>|<span data-ttu-id="cec8e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="cec8e-137">Int32</span></span>|<span data-ttu-id="cec8e-138">Número de horas a aguardar até que a ação seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="cec8e-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="cec8e-139">Valores válidos de 0 a 8760</span><span class="sxs-lookup"><span data-stu-id="cec8e-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="cec8e-140">actionType</span><span class="sxs-lookup"><span data-stu-id="cec8e-140">actionType</span></span>|[<span data-ttu-id="cec8e-141">Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="cec8e-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="cec8e-142">Qual ação executar.</span><span class="sxs-lookup"><span data-stu-id="cec8e-142">What action to take.</span></span> <span data-ttu-id="cec8e-143">Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="cec8e-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="cec8e-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="cec8e-144">notificationTemplateId</span></span>|<span data-ttu-id="cec8e-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cec8e-145">String</span></span>|<span data-ttu-id="cec8e-146">Qual modelo de notificação de mensagem será usado</span><span class="sxs-lookup"><span data-stu-id="cec8e-146">What notification Message template to use</span></span>|
|<span data-ttu-id="cec8e-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="cec8e-147">notificationMessageCCList</span></span>|<span data-ttu-id="cec8e-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cec8e-148">String collection</span></span>|<span data-ttu-id="cec8e-149">Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="cec8e-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="cec8e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="cec8e-150">Response</span></span>
<span data-ttu-id="cec8e-151">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cec8e-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cec8e-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cec8e-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="cec8e-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cec8e-153">Request</span></span>
<span data-ttu-id="cec8e-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cec8e-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cec8e-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="cec8e-155">Response</span></span>
<span data-ttu-id="cec8e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cec8e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



