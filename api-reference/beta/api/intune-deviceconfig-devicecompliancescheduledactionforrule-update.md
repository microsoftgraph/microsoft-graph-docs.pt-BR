---
title: Atualizar deviceComplianceScheduledActionForRule
description: Atualizar as propriedades de um objeto deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: acf3e522b29fe1783b7480368a82323f13c566c9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128198"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="a7792-103">Atualizar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="a7792-103">Update deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="a7792-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7792-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7792-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a7792-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7792-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a7792-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7792-107">Atualizar as propriedades de um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="a7792-107">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7792-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a7792-108">Prerequisites</span></span>
<span data-ttu-id="a7792-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7792-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7792-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7792-111">Permission type</span></span>|<span data-ttu-id="a7792-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7792-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7792-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7792-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7792-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7792-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7792-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7792-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7792-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7792-116">Not supported.</span></span>|
|<span data-ttu-id="a7792-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7792-117">Application</span></span>|<span data-ttu-id="a7792-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7792-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7792-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7792-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="a7792-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7792-120">Request headers</span></span>
|<span data-ttu-id="a7792-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7792-121">Header</span></span>|<span data-ttu-id="a7792-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a7792-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7792-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7792-123">Authorization</span></span>|<span data-ttu-id="a7792-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7792-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7792-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a7792-125">Accept</span></span>|<span data-ttu-id="a7792-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7792-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7792-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7792-127">Request body</span></span>
<span data-ttu-id="a7792-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="a7792-128">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="a7792-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="a7792-129">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="a7792-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7792-130">Property</span></span>|<span data-ttu-id="a7792-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7792-131">Type</span></span>|<span data-ttu-id="a7792-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7792-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7792-133">id</span><span class="sxs-lookup"><span data-stu-id="a7792-133">id</span></span>|<span data-ttu-id="a7792-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7792-134">String</span></span>|<span data-ttu-id="a7792-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a7792-135">Key of the entity.</span></span>|
|<span data-ttu-id="a7792-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="a7792-136">ruleName</span></span>|<span data-ttu-id="a7792-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7792-137">String</span></span>|<span data-ttu-id="a7792-138">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="a7792-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="a7792-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7792-139">Response</span></span>
<span data-ttu-id="a7792-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7792-140">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7792-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7792-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7792-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7792-142">Request</span></span>
<span data-ttu-id="a7792-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7792-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="a7792-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7792-144">Response</span></span>
<span data-ttu-id="a7792-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7792-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




