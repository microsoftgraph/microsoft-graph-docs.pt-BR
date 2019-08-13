---
title: Get deviceComplianceScheduledActionForRule
description: Ler propriedades e relações do objeto deviceComplianceScheduledActionForRule.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6bfd16be433cd1a6c5914f09b79e6cc5979f3f04
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346160"
---
# <a name="get-devicecompliancescheduledactionforrule"></a><span data-ttu-id="55293-103">Get deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="55293-103">Get deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="55293-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55293-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55293-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55293-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55293-106">Ler propriedades e relações do objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="55293-106">Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55293-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55293-107">Prerequisites</span></span>
<span data-ttu-id="55293-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55293-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55293-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55293-110">Permission type</span></span>|<span data-ttu-id="55293-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55293-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55293-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55293-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55293-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="55293-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="55293-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55293-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55293-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55293-115">Not supported.</span></span>|
|<span data-ttu-id="55293-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55293-116">Application</span></span>|<span data-ttu-id="55293-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="55293-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55293-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55293-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55293-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="55293-119">Optional query parameters</span></span>
<span data-ttu-id="55293-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="55293-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55293-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55293-121">Request headers</span></span>
|<span data-ttu-id="55293-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55293-122">Header</span></span>|<span data-ttu-id="55293-123">Valor</span><span class="sxs-lookup"><span data-stu-id="55293-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55293-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="55293-124">Authorization</span></span>|<span data-ttu-id="55293-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55293-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55293-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="55293-126">Accept</span></span>|<span data-ttu-id="55293-127">application/json</span><span class="sxs-lookup"><span data-stu-id="55293-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55293-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55293-128">Request body</span></span>
<span data-ttu-id="55293-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55293-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55293-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="55293-130">Response</span></span>
<span data-ttu-id="55293-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55293-131">If successful, this method returns a `200 OK` response code and [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55293-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55293-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="55293-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55293-133">Request</span></span>
<span data-ttu-id="55293-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55293-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

### <a name="response"></a><span data-ttu-id="55293-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="55293-135">Response</span></span>
<span data-ttu-id="55293-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55293-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






