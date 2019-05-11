---
title: Atualizar deviceComplianceScheduledActionForRule
description: Atualizar as propriedades de um objeto deviceComplianceScheduledActionForRule.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4ef918e13570b5764678837ed0b49aca2eac1f9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927780"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="64620-103">Atualizar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="64620-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="64620-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64620-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64620-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64620-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64620-106">Atualizar as propriedades de um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="64620-106">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64620-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64620-107">Prerequisites</span></span>
<span data-ttu-id="64620-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64620-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64620-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64620-110">Permission type</span></span>|<span data-ttu-id="64620-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64620-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64620-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64620-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64620-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64620-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64620-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64620-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64620-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64620-115">Not supported.</span></span>|
|<span data-ttu-id="64620-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64620-116">Application</span></span>|<span data-ttu-id="64620-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64620-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64620-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64620-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="64620-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64620-119">Request headers</span></span>
|<span data-ttu-id="64620-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64620-120">Header</span></span>|<span data-ttu-id="64620-121">Valor</span><span class="sxs-lookup"><span data-stu-id="64620-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64620-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="64620-122">Authorization</span></span>|<span data-ttu-id="64620-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64620-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64620-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64620-124">Accept</span></span>|<span data-ttu-id="64620-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64620-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64620-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64620-126">Request body</span></span>
<span data-ttu-id="64620-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="64620-127">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="64620-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="64620-128">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="64620-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64620-129">Property</span></span>|<span data-ttu-id="64620-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="64620-130">Type</span></span>|<span data-ttu-id="64620-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="64620-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64620-132">id</span><span class="sxs-lookup"><span data-stu-id="64620-132">id</span></span>|<span data-ttu-id="64620-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64620-133">String</span></span>|<span data-ttu-id="64620-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="64620-134">Key of the entity.</span></span>|
|<span data-ttu-id="64620-135">ruleName</span><span class="sxs-lookup"><span data-stu-id="64620-135">ruleName</span></span>|<span data-ttu-id="64620-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64620-136">String</span></span>|<span data-ttu-id="64620-137">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="64620-137">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="64620-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="64620-138">Response</span></span>
<span data-ttu-id="64620-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64620-139">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64620-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64620-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="64620-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64620-141">Request</span></span>
<span data-ttu-id="64620-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64620-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="64620-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="64620-143">Response</span></span>
<span data-ttu-id="64620-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64620-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




