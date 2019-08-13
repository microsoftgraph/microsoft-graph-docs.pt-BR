---
title: Listar deviceComplianceActionItems
description: Listar propriedades e relações dos objetos deviceComplianceActionItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ae0166800700245f895042bd47fcae413db323e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310903"
---
# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="c5367-103">Listar deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="c5367-103">List deviceComplianceActionItems</span></span>

> <span data-ttu-id="c5367-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5367-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5367-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5367-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5367-106">Listar propriedades e relações dos objetos [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="c5367-106">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5367-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5367-107">Prerequisites</span></span>
<span data-ttu-id="c5367-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5367-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5367-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5367-110">Permission type</span></span>|<span data-ttu-id="c5367-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5367-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5367-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5367-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5367-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5367-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c5367-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5367-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5367-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5367-115">Not supported.</span></span>|
|<span data-ttu-id="c5367-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5367-116">Application</span></span>|<span data-ttu-id="c5367-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5367-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5367-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5367-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c5367-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5367-119">Request headers</span></span>
|<span data-ttu-id="c5367-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5367-120">Header</span></span>|<span data-ttu-id="c5367-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c5367-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5367-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5367-122">Authorization</span></span>|<span data-ttu-id="c5367-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5367-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5367-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5367-124">Accept</span></span>|<span data-ttu-id="c5367-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5367-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5367-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5367-126">Request body</span></span>
<span data-ttu-id="c5367-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5367-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5367-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5367-128">Response</span></span>
<span data-ttu-id="c5367-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5367-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5367-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5367-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5367-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5367-131">Request</span></span>
<span data-ttu-id="c5367-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5367-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="c5367-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5367-133">Response</span></span>
<span data-ttu-id="c5367-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5367-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






