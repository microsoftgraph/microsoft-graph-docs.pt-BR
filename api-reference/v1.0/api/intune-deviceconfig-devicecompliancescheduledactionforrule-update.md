---
title: Atualizar deviceComplianceScheduledActionForRule
description: Atualizar as propriedades de um objeto deviceComplianceScheduledActionForRule.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b085d39b9befb4f98a9fc50c55cdb80d1ee36050
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354130"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="0b73b-103">Atualizar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="0b73b-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="0b73b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b73b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b73b-105">Atualizar as propriedades de um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="0b73b-105">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b73b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b73b-106">Prerequisites</span></span>
<span data-ttu-id="0b73b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b73b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b73b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b73b-109">Permission type</span></span>|<span data-ttu-id="0b73b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b73b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b73b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b73b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b73b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b73b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b73b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b73b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b73b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b73b-114">Not supported.</span></span>|
|<span data-ttu-id="0b73b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b73b-115">Application</span></span>|<span data-ttu-id="0b73b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b73b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b73b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b73b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="0b73b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b73b-118">Request headers</span></span>
|<span data-ttu-id="0b73b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b73b-119">Header</span></span>|<span data-ttu-id="0b73b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0b73b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b73b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b73b-121">Authorization</span></span>|<span data-ttu-id="0b73b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b73b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b73b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b73b-123">Accept</span></span>|<span data-ttu-id="0b73b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0b73b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b73b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b73b-125">Request body</span></span>
<span data-ttu-id="0b73b-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="0b73b-126">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="0b73b-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="0b73b-127">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="0b73b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b73b-128">Property</span></span>|<span data-ttu-id="0b73b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b73b-129">Type</span></span>|<span data-ttu-id="0b73b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b73b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b73b-131">id</span><span class="sxs-lookup"><span data-stu-id="0b73b-131">id</span></span>|<span data-ttu-id="0b73b-132">String</span><span class="sxs-lookup"><span data-stu-id="0b73b-132">String</span></span>|<span data-ttu-id="0b73b-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0b73b-133">Key of the entity.</span></span>|
|<span data-ttu-id="0b73b-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="0b73b-134">ruleName</span></span>|<span data-ttu-id="0b73b-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b73b-135">String</span></span>|<span data-ttu-id="0b73b-136">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="0b73b-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="0b73b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b73b-137">Response</span></span>
<span data-ttu-id="0b73b-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b73b-138">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b73b-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b73b-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b73b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b73b-140">Request</span></span>
<span data-ttu-id="0b73b-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b73b-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="0b73b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b73b-142">Response</span></span>
<span data-ttu-id="0b73b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b73b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```




