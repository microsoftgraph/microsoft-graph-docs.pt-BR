---
title: Acessar deviceComplianceActionItem
description: Leia as propriedades e as relações do objeto deviceComplianceActionItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c36d4bca4d442108edb683719782894108e1b0b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968627"
---
# <a name="get-devicecomplianceactionitem"></a><span data-ttu-id="b3b19-103">Acessar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b3b19-103">Get deviceComplianceActionItem</span></span>

> <span data-ttu-id="b3b19-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b3b19-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3b19-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3b19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3b19-106">Leia as propriedades e as relações do objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="b3b19-106">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3b19-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3b19-107">Prerequisites</span></span>
<span data-ttu-id="b3b19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3b19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3b19-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3b19-110">Permission type</span></span>|<span data-ttu-id="b3b19-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b3b19-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3b19-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3b19-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3b19-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3b19-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b3b19-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3b19-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3b19-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3b19-115">Not supported.</span></span>|
|<span data-ttu-id="b3b19-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3b19-116">Application</span></span>|<span data-ttu-id="b3b19-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3b19-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3b19-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3b19-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3b19-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b3b19-119">Optional query parameters</span></span>
<span data-ttu-id="b3b19-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b3b19-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3b19-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3b19-121">Request headers</span></span>
|<span data-ttu-id="b3b19-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3b19-122">Header</span></span>|<span data-ttu-id="b3b19-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b3b19-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3b19-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3b19-124">Authorization</span></span>|<span data-ttu-id="b3b19-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3b19-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3b19-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b3b19-126">Accept</span></span>|<span data-ttu-id="b3b19-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b3b19-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3b19-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3b19-128">Request body</span></span>
<span data-ttu-id="b3b19-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3b19-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3b19-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3b19-130">Response</span></span>
<span data-ttu-id="b3b19-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3b19-131">If successful, this method returns a `200 OK` response code and [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3b19-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3b19-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3b19-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3b19-133">Request</span></span>
<span data-ttu-id="b3b19-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3b19-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="b3b19-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3b19-135">Response</span></span>
<span data-ttu-id="b3b19-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3b19-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
    "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
    "gracePeriodHours": 0,
    "actionType": "notification",
    "notificationTemplateId": "Notification Template Id value",
    "notificationMessageCCList": [
      "Notification Message CCList value"
    ]
  }
}
```





