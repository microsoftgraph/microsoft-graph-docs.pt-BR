---
title: Atualizar deviceComplianceScheduledActionForRule
description: Atualizar as propriedades de um objeto deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8936ad39af18e51a7f5e7b17a26357a587a3d5d8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399603"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="a5116-103">Atualizar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="a5116-103">Update deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="a5116-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5116-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5116-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5116-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5116-106">Atualizar as propriedades de um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="a5116-106">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5116-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a5116-107">Prerequisites</span></span>
<span data-ttu-id="a5116-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5116-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5116-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5116-110">Permission type</span></span>|<span data-ttu-id="a5116-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a5116-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5116-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5116-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5116-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5116-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5116-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5116-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5116-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5116-115">Not supported.</span></span>|
|<span data-ttu-id="a5116-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5116-116">Application</span></span>|<span data-ttu-id="a5116-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5116-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5116-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5116-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="a5116-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5116-119">Request headers</span></span>
|<span data-ttu-id="a5116-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5116-120">Header</span></span>|<span data-ttu-id="a5116-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a5116-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5116-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5116-122">Authorization</span></span>|<span data-ttu-id="a5116-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5116-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5116-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a5116-124">Accept</span></span>|<span data-ttu-id="a5116-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5116-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5116-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5116-126">Request body</span></span>
<span data-ttu-id="a5116-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="a5116-127">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="a5116-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="a5116-128">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="a5116-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5116-129">Property</span></span>|<span data-ttu-id="a5116-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5116-130">Type</span></span>|<span data-ttu-id="a5116-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5116-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5116-132">id</span><span class="sxs-lookup"><span data-stu-id="a5116-132">id</span></span>|<span data-ttu-id="a5116-133">String</span><span class="sxs-lookup"><span data-stu-id="a5116-133">String</span></span>|<span data-ttu-id="a5116-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a5116-134">Key of the entity.</span></span>|
|<span data-ttu-id="a5116-135">ruleName</span><span class="sxs-lookup"><span data-stu-id="a5116-135">ruleName</span></span>|<span data-ttu-id="a5116-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5116-136">String</span></span>|<span data-ttu-id="a5116-137">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="a5116-137">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="a5116-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5116-138">Response</span></span>
<span data-ttu-id="a5116-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5116-139">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5116-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5116-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5116-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5116-141">Request</span></span>
<span data-ttu-id="a5116-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5116-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="a5116-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5116-143">Response</span></span>
<span data-ttu-id="a5116-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5116-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






