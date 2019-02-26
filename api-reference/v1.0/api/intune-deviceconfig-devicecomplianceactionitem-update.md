---
title: Atualizar deviceComplianceActionItem
description: Atualizar as propriedades de um objeto deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5da502820ccf13b0494a6914811db698ff8abc65
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254020"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="aba88-103">Atualizar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="aba88-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="aba88-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aba88-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aba88-105">Atualizar as propriedades de um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="aba88-105">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aba88-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aba88-106">Prerequisites</span></span>
<span data-ttu-id="aba88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="aba88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aba88-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aba88-109">Permission type</span></span>|<span data-ttu-id="aba88-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aba88-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aba88-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aba88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aba88-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aba88-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aba88-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aba88-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aba88-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aba88-114">Not supported.</span></span>|
|<span data-ttu-id="aba88-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aba88-115">Application</span></span>|<span data-ttu-id="aba88-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aba88-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aba88-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aba88-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="aba88-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aba88-118">Request headers</span></span>
|<span data-ttu-id="aba88-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aba88-119">Header</span></span>|<span data-ttu-id="aba88-120">Valor</span><span class="sxs-lookup"><span data-stu-id="aba88-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aba88-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="aba88-121">Authorization</span></span>|<span data-ttu-id="aba88-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aba88-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aba88-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aba88-123">Accept</span></span>|<span data-ttu-id="aba88-124">application/json</span><span class="sxs-lookup"><span data-stu-id="aba88-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aba88-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aba88-125">Request body</span></span>
<span data-ttu-id="aba88-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="aba88-126">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="aba88-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="aba88-127">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="aba88-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aba88-128">Property</span></span>|<span data-ttu-id="aba88-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="aba88-129">Type</span></span>|<span data-ttu-id="aba88-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="aba88-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aba88-131">id</span><span class="sxs-lookup"><span data-stu-id="aba88-131">id</span></span>|<span data-ttu-id="aba88-132">String</span><span class="sxs-lookup"><span data-stu-id="aba88-132">String</span></span>|<span data-ttu-id="aba88-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aba88-133">Key of the entity.</span></span>|
|<span data-ttu-id="aba88-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="aba88-134">gracePeriodHours</span></span>|<span data-ttu-id="aba88-135">Int32</span><span class="sxs-lookup"><span data-stu-id="aba88-135">Int32</span></span>|<span data-ttu-id="aba88-136">Número de horas a aguardar até que a ação seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="aba88-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="aba88-137">Valores válidos de 0 a 8760</span><span class="sxs-lookup"><span data-stu-id="aba88-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="aba88-138">actionType</span><span class="sxs-lookup"><span data-stu-id="aba88-138">actionType</span></span>|[<span data-ttu-id="aba88-139">Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="aba88-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="aba88-140">Qual ação executar.</span><span class="sxs-lookup"><span data-stu-id="aba88-140">What action to take.</span></span> <span data-ttu-id="aba88-141">Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="aba88-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="aba88-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="aba88-142">notificationTemplateId</span></span>|<span data-ttu-id="aba88-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aba88-143">String</span></span>|<span data-ttu-id="aba88-144">Qual modelo de notificação de mensagem será usado</span><span class="sxs-lookup"><span data-stu-id="aba88-144">What notification Message template to use</span></span>|
|<span data-ttu-id="aba88-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="aba88-145">notificationMessageCCList</span></span>|<span data-ttu-id="aba88-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aba88-146">String collection</span></span>|<span data-ttu-id="aba88-147">Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="aba88-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="aba88-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="aba88-148">Response</span></span>
<span data-ttu-id="aba88-149">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aba88-149">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aba88-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aba88-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="aba88-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aba88-151">Request</span></span>
<span data-ttu-id="aba88-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aba88-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aba88-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="aba88-153">Response</span></span>
<span data-ttu-id="aba88-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aba88-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



