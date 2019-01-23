---
title: Criar deviceComplianceActionItem
description: Criar um novo objeto deviceComplianceActionItem.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5e538bd064c2d590eeb743e2c2dea05abc869900
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421575"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="cf109-103">Criar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="cf109-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="cf109-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cf109-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cf109-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cf109-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf109-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cf109-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf109-107">Criar um novo objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="cf109-107">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf109-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf109-108">Prerequisites</span></span>
<span data-ttu-id="cf109-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cf109-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cf109-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf109-111">Permission type</span></span>|<span data-ttu-id="cf109-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf109-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf109-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf109-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf109-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf109-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf109-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf109-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf109-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf109-116">Not supported.</span></span>|
|<span data-ttu-id="cf109-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf109-117">Application</span></span>|<span data-ttu-id="cf109-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf109-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf109-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf109-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cf109-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf109-120">Request headers</span></span>
|<span data-ttu-id="cf109-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf109-121">Header</span></span>|<span data-ttu-id="cf109-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cf109-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf109-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf109-123">Authorization</span></span>|<span data-ttu-id="cf109-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf109-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf109-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf109-125">Accept</span></span>|<span data-ttu-id="cf109-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf109-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf109-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf109-127">Request body</span></span>
<span data-ttu-id="cf109-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="cf109-128">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="cf109-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="cf109-129">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="cf109-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf109-130">Property</span></span>|<span data-ttu-id="cf109-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf109-131">Type</span></span>|<span data-ttu-id="cf109-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf109-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf109-133">id</span><span class="sxs-lookup"><span data-stu-id="cf109-133">id</span></span>|<span data-ttu-id="cf109-134">String</span><span class="sxs-lookup"><span data-stu-id="cf109-134">String</span></span>|<span data-ttu-id="cf109-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cf109-135">Key of the entity.</span></span>|
|<span data-ttu-id="cf109-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="cf109-136">gracePeriodHours</span></span>|<span data-ttu-id="cf109-137">Int32</span><span class="sxs-lookup"><span data-stu-id="cf109-137">Int32</span></span>|<span data-ttu-id="cf109-138">Número de horas a aguardar até que a ação seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="cf109-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="cf109-139">Valores válidos de 0 a 8760</span><span class="sxs-lookup"><span data-stu-id="cf109-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="cf109-140">actionType</span><span class="sxs-lookup"><span data-stu-id="cf109-140">actionType</span></span>|[<span data-ttu-id="cf109-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="cf109-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="cf109-142">Ação que será executada.</span><span class="sxs-lookup"><span data-stu-id="cf109-142">What action to take.</span></span> <span data-ttu-id="cf109-143">Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="cf109-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="cf109-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="cf109-144">notificationTemplateId</span></span>|<span data-ttu-id="cf109-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf109-145">String</span></span>|<span data-ttu-id="cf109-146">Qual modelo de notificação de mensagem será usado</span><span class="sxs-lookup"><span data-stu-id="cf109-146">What notification Message template to use</span></span>|
|<span data-ttu-id="cf109-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="cf109-147">notificationMessageCCList</span></span>|<span data-ttu-id="cf109-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf109-148">String collection</span></span>|<span data-ttu-id="cf109-149">Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.</span><span class="sxs-lookup"><span data-stu-id="cf109-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="cf109-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf109-150">Response</span></span>
<span data-ttu-id="cf109-151">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf109-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf109-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf109-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf109-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf109-153">Request</span></span>
<span data-ttu-id="cf109-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf109-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cf109-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf109-155">Response</span></span>
<span data-ttu-id="cf109-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf109-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




