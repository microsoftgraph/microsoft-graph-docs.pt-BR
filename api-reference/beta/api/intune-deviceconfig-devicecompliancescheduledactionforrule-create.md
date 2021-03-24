---
title: Criar deviceComplianceScheduledActionForRule
description: Criar um novo objeto deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f884c4168de0f8737552e7d3b367c7e60018058
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130151"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="41b67-103">Criar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="41b67-103">Create deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="41b67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41b67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41b67-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41b67-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41b67-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41b67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41b67-107">Criar um novo objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="41b67-107">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41b67-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41b67-108">Prerequisites</span></span>
<span data-ttu-id="41b67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41b67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41b67-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41b67-111">Permission type</span></span>|<span data-ttu-id="41b67-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41b67-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41b67-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41b67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41b67-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41b67-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41b67-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41b67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41b67-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41b67-116">Not supported.</span></span>|
|<span data-ttu-id="41b67-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41b67-117">Application</span></span>|<span data-ttu-id="41b67-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41b67-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41b67-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41b67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="41b67-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41b67-120">Request headers</span></span>
|<span data-ttu-id="41b67-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41b67-121">Header</span></span>|<span data-ttu-id="41b67-122">Valor</span><span class="sxs-lookup"><span data-stu-id="41b67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41b67-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="41b67-123">Authorization</span></span>|<span data-ttu-id="41b67-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41b67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41b67-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41b67-125">Accept</span></span>|<span data-ttu-id="41b67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41b67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41b67-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41b67-127">Request body</span></span>
<span data-ttu-id="41b67-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="41b67-128">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="41b67-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="41b67-129">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="41b67-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41b67-130">Property</span></span>|<span data-ttu-id="41b67-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="41b67-131">Type</span></span>|<span data-ttu-id="41b67-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="41b67-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41b67-133">id</span><span class="sxs-lookup"><span data-stu-id="41b67-133">id</span></span>|<span data-ttu-id="41b67-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41b67-134">String</span></span>|<span data-ttu-id="41b67-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="41b67-135">Key of the entity.</span></span>|
|<span data-ttu-id="41b67-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="41b67-136">ruleName</span></span>|<span data-ttu-id="41b67-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41b67-137">String</span></span>|<span data-ttu-id="41b67-138">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="41b67-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="41b67-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="41b67-139">Response</span></span>
<span data-ttu-id="41b67-140">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41b67-140">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41b67-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41b67-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="41b67-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41b67-142">Request</span></span>
<span data-ttu-id="41b67-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41b67-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="41b67-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="41b67-144">Response</span></span>
<span data-ttu-id="41b67-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41b67-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




