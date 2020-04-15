---
title: Criar deviceComplianceScheduledActionForRule
description: Criar um novo objeto deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14ecd6ad49c2a51287fcf0b6de8cc75853ab4847
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399728"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="165a1-103">Criar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="165a1-103">Create deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="165a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="165a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="165a1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="165a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="165a1-106">Criar um novo objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="165a1-106">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="165a1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="165a1-107">Prerequisites</span></span>
<span data-ttu-id="165a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="165a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="165a1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="165a1-110">Permission type</span></span>|<span data-ttu-id="165a1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="165a1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="165a1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="165a1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="165a1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="165a1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="165a1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="165a1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="165a1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="165a1-115">Not supported.</span></span>|
|<span data-ttu-id="165a1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="165a1-116">Application</span></span>|<span data-ttu-id="165a1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="165a1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="165a1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="165a1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="165a1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="165a1-119">Request headers</span></span>
|<span data-ttu-id="165a1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="165a1-120">Header</span></span>|<span data-ttu-id="165a1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="165a1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="165a1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="165a1-122">Authorization</span></span>|<span data-ttu-id="165a1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="165a1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="165a1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="165a1-124">Accept</span></span>|<span data-ttu-id="165a1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="165a1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="165a1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="165a1-126">Request body</span></span>
<span data-ttu-id="165a1-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="165a1-127">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="165a1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="165a1-128">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="165a1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="165a1-129">Property</span></span>|<span data-ttu-id="165a1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="165a1-130">Type</span></span>|<span data-ttu-id="165a1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="165a1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="165a1-132">id</span><span class="sxs-lookup"><span data-stu-id="165a1-132">id</span></span>|<span data-ttu-id="165a1-133">String</span><span class="sxs-lookup"><span data-stu-id="165a1-133">String</span></span>|<span data-ttu-id="165a1-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="165a1-134">Key of the entity.</span></span>|
|<span data-ttu-id="165a1-135">ruleName</span><span class="sxs-lookup"><span data-stu-id="165a1-135">ruleName</span></span>|<span data-ttu-id="165a1-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="165a1-136">String</span></span>|<span data-ttu-id="165a1-137">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="165a1-137">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="165a1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="165a1-138">Response</span></span>
<span data-ttu-id="165a1-139">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="165a1-139">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="165a1-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="165a1-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="165a1-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="165a1-141">Request</span></span>
<span data-ttu-id="165a1-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="165a1-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="165a1-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="165a1-143">Response</span></span>
<span data-ttu-id="165a1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="165a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```






