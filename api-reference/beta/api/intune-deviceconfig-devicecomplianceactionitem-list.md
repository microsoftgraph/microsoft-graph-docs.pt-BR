---
title: Listar deviceComplianceActionItems
description: Listar propriedades e relações dos objetos deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d1b05e6e5a6b55995f793610ead82e2cb4474b6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961019"
---
# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="dfbad-103">Listar deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="dfbad-103">List deviceComplianceActionItems</span></span>

> <span data-ttu-id="dfbad-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dfbad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfbad-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dfbad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dfbad-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dfbad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfbad-107">Listar propriedades e relações dos objetos [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="dfbad-107">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dfbad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dfbad-108">Prerequisites</span></span>
<span data-ttu-id="dfbad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfbad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfbad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfbad-111">Permission type</span></span>|<span data-ttu-id="dfbad-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dfbad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfbad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfbad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dfbad-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfbad-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dfbad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfbad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfbad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfbad-116">Not supported.</span></span>|
|<span data-ttu-id="dfbad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfbad-117">Application</span></span>|<span data-ttu-id="dfbad-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfbad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfbad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfbad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dfbad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfbad-120">Request headers</span></span>
|<span data-ttu-id="dfbad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dfbad-121">Header</span></span>|<span data-ttu-id="dfbad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dfbad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfbad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfbad-123">Authorization</span></span>|<span data-ttu-id="dfbad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfbad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfbad-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dfbad-125">Accept</span></span>|<span data-ttu-id="dfbad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dfbad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfbad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfbad-127">Request body</span></span>
<span data-ttu-id="dfbad-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfbad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfbad-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfbad-129">Response</span></span>
<span data-ttu-id="dfbad-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfbad-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfbad-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfbad-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="dfbad-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfbad-132">Request</span></span>
<span data-ttu-id="dfbad-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfbad-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="dfbad-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfbad-134">Response</span></span>
<span data-ttu-id="dfbad-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfbad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





