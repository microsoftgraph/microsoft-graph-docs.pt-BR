---
title: Listar deviceComplianceActionItems
description: Listar propriedades e relações dos objetos deviceComplianceActionItem.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: accb71381d307d689c33b2a1aea0385eb6270ebe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43400864"
---
# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="38610-103">Listar deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="38610-103">List deviceComplianceActionItems</span></span>

<span data-ttu-id="38610-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38610-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38610-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38610-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38610-106">Listar propriedades e relações dos objetos [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="38610-106">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38610-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38610-107">Prerequisites</span></span>
<span data-ttu-id="38610-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38610-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38610-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38610-110">Permission type</span></span>|<span data-ttu-id="38610-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38610-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38610-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38610-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38610-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38610-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="38610-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38610-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38610-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38610-115">Not supported.</span></span>|
|<span data-ttu-id="38610-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38610-116">Application</span></span>|<span data-ttu-id="38610-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38610-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38610-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38610-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="38610-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38610-119">Request headers</span></span>
|<span data-ttu-id="38610-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38610-120">Header</span></span>|<span data-ttu-id="38610-121">Valor</span><span class="sxs-lookup"><span data-stu-id="38610-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38610-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="38610-122">Authorization</span></span>|<span data-ttu-id="38610-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38610-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38610-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38610-124">Accept</span></span>|<span data-ttu-id="38610-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38610-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38610-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38610-126">Request body</span></span>
<span data-ttu-id="38610-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38610-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38610-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="38610-128">Response</span></span>
<span data-ttu-id="38610-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38610-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38610-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38610-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="38610-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38610-131">Request</span></span>
<span data-ttu-id="38610-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38610-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="38610-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="38610-133">Response</span></span>
<span data-ttu-id="38610-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38610-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": [
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
  ]
}
```






