---
title: Get deviceComplianceScheduledActionForRule
description: Ler propriedades e relações do objeto deviceComplianceScheduledActionForRule.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 265049509bff84d8d008354cf0e7d649e8801979
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42755284"
---
# <a name="get-devicecompliancescheduledactionforrule"></a><span data-ttu-id="840bb-103">Get deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="840bb-103">Get deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="840bb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="840bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="840bb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="840bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="840bb-106">Ler propriedades e relações do objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="840bb-106">Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="840bb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="840bb-107">Prerequisites</span></span>
<span data-ttu-id="840bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="840bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="840bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="840bb-110">Permission type</span></span>|<span data-ttu-id="840bb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="840bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="840bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="840bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="840bb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="840bb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="840bb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="840bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="840bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="840bb-115">Not supported.</span></span>|
|<span data-ttu-id="840bb-116">Application</span><span class="sxs-lookup"><span data-stu-id="840bb-116">Application</span></span>|<span data-ttu-id="840bb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="840bb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="840bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="840bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="840bb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="840bb-119">Optional query parameters</span></span>
<span data-ttu-id="840bb-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="840bb-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="840bb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="840bb-121">Request headers</span></span>
|<span data-ttu-id="840bb-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="840bb-122">Header</span></span>|<span data-ttu-id="840bb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="840bb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="840bb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="840bb-124">Authorization</span></span>|<span data-ttu-id="840bb-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="840bb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="840bb-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="840bb-126">Accept</span></span>|<span data-ttu-id="840bb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="840bb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="840bb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="840bb-128">Request body</span></span>
<span data-ttu-id="840bb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="840bb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="840bb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="840bb-130">Response</span></span>
<span data-ttu-id="840bb-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="840bb-131">If successful, this method returns a `200 OK` response code and [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="840bb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="840bb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="840bb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="840bb-133">Request</span></span>
<span data-ttu-id="840bb-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="840bb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

### <a name="response"></a><span data-ttu-id="840bb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="840bb-135">Response</span></span>
<span data-ttu-id="840bb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="840bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 188

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
    "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
    "ruleName": "Rule Name value"
  }
}
```




