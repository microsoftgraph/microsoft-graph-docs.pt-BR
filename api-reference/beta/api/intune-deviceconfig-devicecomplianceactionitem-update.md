---
title: Atualizar deviceComplianceActionItem
description: Atualizar as propriedades de um objeto deviceComplianceActionItem.
author: tfitzmac
ms.openlocfilehash: f9aca51db300abf9243ef8abe1246c2a0a6b910d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344125"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="da424-103">Atualizar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="da424-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="da424-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="da424-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da424-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da424-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da424-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="da424-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da424-107">Atualizar as propriedades de um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="da424-107">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da424-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da424-108">Prerequisites</span></span>
<span data-ttu-id="da424-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da424-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da424-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da424-111">Permission type</span></span>|<span data-ttu-id="da424-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da424-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da424-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da424-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da424-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da424-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da424-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da424-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da424-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da424-116">Not supported.</span></span>|
|<span data-ttu-id="da424-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da424-117">Application</span></span>|<span data-ttu-id="da424-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da424-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da424-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da424-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="da424-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da424-120">Request headers</span></span>
|<span data-ttu-id="da424-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da424-121">Header</span></span>|<span data-ttu-id="da424-122">Valor</span><span class="sxs-lookup"><span data-stu-id="da424-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da424-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="da424-123">Authorization</span></span>|<span data-ttu-id="da424-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da424-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da424-125">Accept</span><span class="sxs-lookup"><span data-stu-id="da424-125">Accept</span></span>|<span data-ttu-id="da424-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da424-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da424-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da424-127">Request body</span></span>
<span data-ttu-id="da424-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="da424-128">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="da424-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="da424-129">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="da424-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da424-130">Property</span></span>|<span data-ttu-id="da424-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="da424-131">Type</span></span>|<span data-ttu-id="da424-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="da424-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da424-133">id</span><span class="sxs-lookup"><span data-stu-id="da424-133">id</span></span>|<span data-ttu-id="da424-134">String</span><span class="sxs-lookup"><span data-stu-id="da424-134">String</span></span>|<span data-ttu-id="da424-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="da424-135">Key of the entity.</span></span>|
|<span data-ttu-id="da424-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="da424-136">gracePeriodHours</span></span>|<span data-ttu-id="da424-137">Int32</span><span class="sxs-lookup"><span data-stu-id="da424-137">Int32</span></span>|<span data-ttu-id="da424-138">Número de horas a aguardar até que a ação seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="da424-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="da424-139">Valores válidos de 0 a 8760</span><span class="sxs-lookup"><span data-stu-id="da424-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="da424-140">actionType</span><span class="sxs-lookup"><span data-stu-id="da424-140">actionType</span></span>|[<span data-ttu-id="da424-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="da424-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="da424-142">Ação que será executada.</span><span class="sxs-lookup"><span data-stu-id="da424-142">What action to take.</span></span> <span data-ttu-id="da424-143">Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="da424-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="da424-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="da424-144">notificationTemplateId</span></span>|<span data-ttu-id="da424-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da424-145">String</span></span>|<span data-ttu-id="da424-146">Qual modelo de notificação de mensagem será usado</span><span class="sxs-lookup"><span data-stu-id="da424-146">What notification Message template to use</span></span>|
|<span data-ttu-id="da424-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="da424-147">notificationMessageCCList</span></span>|<span data-ttu-id="da424-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="da424-148">String collection</span></span>|<span data-ttu-id="da424-149">Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="da424-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="da424-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="da424-150">Response</span></span>
<span data-ttu-id="da424-151">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da424-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da424-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da424-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="da424-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da424-153">Request</span></span>
<span data-ttu-id="da424-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da424-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
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

### <a name="response"></a><span data-ttu-id="da424-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="da424-155">Response</span></span>
<span data-ttu-id="da424-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da424-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





