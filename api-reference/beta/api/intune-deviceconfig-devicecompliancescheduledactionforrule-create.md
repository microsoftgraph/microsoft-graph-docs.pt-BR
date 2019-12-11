---
title: Criar deviceComplianceScheduledActionForRule
description: Criar um novo objeto deviceComplianceScheduledActionForRule.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: afd2ec830b2bc23276e2d17cee15b8929321c364
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949606"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="2d4ee-103">Criar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="2d4ee-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="2d4ee-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d4ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d4ee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d4ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d4ee-106">Criar um novo objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="2d4ee-106">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d4ee-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d4ee-107">Prerequisites</span></span>
<span data-ttu-id="2d4ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d4ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d4ee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d4ee-110">Permission type</span></span>|<span data-ttu-id="2d4ee-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2d4ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d4ee-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d4ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d4ee-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d4ee-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d4ee-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d4ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d4ee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d4ee-115">Not supported.</span></span>|
|<span data-ttu-id="2d4ee-116">Application</span><span class="sxs-lookup"><span data-stu-id="2d4ee-116">Application</span></span>|<span data-ttu-id="2d4ee-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d4ee-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d4ee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d4ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="2d4ee-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d4ee-119">Request headers</span></span>
|<span data-ttu-id="2d4ee-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d4ee-120">Header</span></span>|<span data-ttu-id="2d4ee-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2d4ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d4ee-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d4ee-122">Authorization</span></span>|<span data-ttu-id="2d4ee-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d4ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d4ee-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d4ee-124">Accept</span></span>|<span data-ttu-id="2d4ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d4ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d4ee-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d4ee-126">Request body</span></span>
<span data-ttu-id="2d4ee-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="2d4ee-127">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="2d4ee-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="2d4ee-128">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="2d4ee-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d4ee-129">Property</span></span>|<span data-ttu-id="2d4ee-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d4ee-130">Type</span></span>|<span data-ttu-id="2d4ee-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d4ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d4ee-132">id</span><span class="sxs-lookup"><span data-stu-id="2d4ee-132">id</span></span>|<span data-ttu-id="2d4ee-133">String</span><span class="sxs-lookup"><span data-stu-id="2d4ee-133">String</span></span>|<span data-ttu-id="2d4ee-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2d4ee-134">Key of the entity.</span></span>|
|<span data-ttu-id="2d4ee-135">ruleName</span><span class="sxs-lookup"><span data-stu-id="2d4ee-135">ruleName</span></span>|<span data-ttu-id="2d4ee-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d4ee-136">String</span></span>|<span data-ttu-id="2d4ee-137">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="2d4ee-137">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="2d4ee-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d4ee-138">Response</span></span>
<span data-ttu-id="2d4ee-139">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d4ee-139">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d4ee-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d4ee-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d4ee-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d4ee-141">Request</span></span>
<span data-ttu-id="2d4ee-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d4ee-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="2d4ee-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d4ee-143">Response</span></span>
<span data-ttu-id="2d4ee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d4ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





