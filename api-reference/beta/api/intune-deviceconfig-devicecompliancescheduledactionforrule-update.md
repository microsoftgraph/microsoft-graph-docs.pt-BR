---
title: Atualizar deviceComplianceScheduledActionForRule
description: Atualizar as propriedades de um objeto deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08a9ace90f3b17470cf5d7ced7b9fb8553e6c83d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725005"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="a0102-103">Atualizar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="a0102-103">Update deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="a0102-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0102-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0102-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0102-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0102-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0102-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0102-107">Atualizar as propriedades de um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="a0102-107">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0102-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0102-108">Prerequisites</span></span>
<span data-ttu-id="a0102-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0102-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0102-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0102-111">Permission type</span></span>|<span data-ttu-id="a0102-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0102-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0102-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0102-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0102-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0102-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0102-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0102-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0102-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0102-116">Not supported.</span></span>|
|<span data-ttu-id="a0102-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0102-117">Application</span></span>|<span data-ttu-id="a0102-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0102-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0102-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0102-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="a0102-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0102-120">Request headers</span></span>
|<span data-ttu-id="a0102-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0102-121">Header</span></span>|<span data-ttu-id="a0102-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a0102-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0102-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0102-123">Authorization</span></span>|<span data-ttu-id="a0102-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0102-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0102-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0102-125">Accept</span></span>|<span data-ttu-id="a0102-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0102-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0102-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0102-127">Request body</span></span>
<span data-ttu-id="a0102-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="a0102-128">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="a0102-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="a0102-129">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="a0102-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0102-130">Property</span></span>|<span data-ttu-id="a0102-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0102-131">Type</span></span>|<span data-ttu-id="a0102-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0102-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0102-133">id</span><span class="sxs-lookup"><span data-stu-id="a0102-133">id</span></span>|<span data-ttu-id="a0102-134">String</span><span class="sxs-lookup"><span data-stu-id="a0102-134">String</span></span>|<span data-ttu-id="a0102-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a0102-135">Key of the entity.</span></span>|
|<span data-ttu-id="a0102-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="a0102-136">ruleName</span></span>|<span data-ttu-id="a0102-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0102-137">String</span></span>|<span data-ttu-id="a0102-138">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="a0102-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="a0102-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0102-139">Response</span></span>
<span data-ttu-id="a0102-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0102-140">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0102-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0102-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0102-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0102-142">Request</span></span>
<span data-ttu-id="a0102-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0102-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="a0102-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0102-144">Response</span></span>
<span data-ttu-id="a0102-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0102-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





