---
title: Acessar deviceComplianceActionItem
description: Leia as propriedades e as relações do objeto deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 23a34f0f3da6023dfb62e270b834549972a72305
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997775"
---
# <a name="get-devicecomplianceactionitem"></a><span data-ttu-id="eb7b5-103">Acessar deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="eb7b5-103">Get deviceComplianceActionItem</span></span>

> <span data-ttu-id="eb7b5-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb7b5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb7b5-105">Leia as propriedades e as relações do objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="eb7b5-105">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb7b5-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb7b5-106">Prerequisites</span></span>
<span data-ttu-id="eb7b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb7b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb7b5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb7b5-109">Permission type</span></span>|<span data-ttu-id="eb7b5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb7b5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb7b5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb7b5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eb7b5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb7b5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eb7b5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb7b5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb7b5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb7b5-114">Not supported.</span></span>|
|<span data-ttu-id="eb7b5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb7b5-115">Application</span></span>|<span data-ttu-id="eb7b5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb7b5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb7b5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb7b5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb7b5-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eb7b5-118">Optional query parameters</span></span>
<span data-ttu-id="eb7b5-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eb7b5-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb7b5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb7b5-120">Request headers</span></span>
|<span data-ttu-id="eb7b5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb7b5-121">Header</span></span>|<span data-ttu-id="eb7b5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eb7b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb7b5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb7b5-123">Authorization</span></span>|<span data-ttu-id="eb7b5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb7b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb7b5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb7b5-125">Accept</span></span>|<span data-ttu-id="eb7b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb7b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb7b5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb7b5-127">Request body</span></span>
<span data-ttu-id="eb7b5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb7b5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb7b5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb7b5-129">Response</span></span>
<span data-ttu-id="eb7b5-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb7b5-130">If successful, this method returns a `200 OK` response code and [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb7b5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb7b5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb7b5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb7b5-132">Request</span></span>
<span data-ttu-id="eb7b5-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb7b5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="eb7b5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb7b5-134">Response</span></span>
<span data-ttu-id="eb7b5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb7b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



