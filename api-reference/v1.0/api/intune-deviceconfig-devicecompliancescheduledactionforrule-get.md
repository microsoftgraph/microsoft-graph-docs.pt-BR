---
title: Get deviceComplianceScheduledActionForRule
description: Ler propriedades e relações do objeto deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1317927a45310400bd9fa464a56ac7df968d2e59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580873"
---
# <a name="get-devicecompliancescheduledactionforrule"></a><span data-ttu-id="5fd6a-103">Get deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="5fd6a-103">Get deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="5fd6a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5fd6a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fd6a-105">Ler propriedades e relações do objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="5fd6a-105">Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fd6a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5fd6a-106">Prerequisites</span></span>
<span data-ttu-id="5fd6a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fd6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fd6a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5fd6a-109">Permission type</span></span>|<span data-ttu-id="5fd6a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5fd6a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fd6a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5fd6a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5fd6a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5fd6a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5fd6a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5fd6a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fd6a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fd6a-114">Not supported.</span></span>|
|<span data-ttu-id="5fd6a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5fd6a-115">Application</span></span>|<span data-ttu-id="5fd6a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fd6a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fd6a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fd6a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5fd6a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5fd6a-118">Optional query parameters</span></span>
<span data-ttu-id="5fd6a-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5fd6a-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5fd6a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fd6a-120">Request headers</span></span>
|<span data-ttu-id="5fd6a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5fd6a-121">Header</span></span>|<span data-ttu-id="5fd6a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5fd6a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fd6a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5fd6a-123">Authorization</span></span>|<span data-ttu-id="5fd6a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fd6a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fd6a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5fd6a-125">Accept</span></span>|<span data-ttu-id="5fd6a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5fd6a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fd6a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5fd6a-127">Request body</span></span>
<span data-ttu-id="5fd6a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5fd6a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fd6a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fd6a-129">Response</span></span>
<span data-ttu-id="5fd6a-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fd6a-130">If successful, this method returns a `200 OK` response code and [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fd6a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5fd6a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fd6a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fd6a-132">Request</span></span>
<span data-ttu-id="5fd6a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5fd6a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

### <a name="response"></a><span data-ttu-id="5fd6a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fd6a-134">Response</span></span>
<span data-ttu-id="5fd6a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5fd6a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



