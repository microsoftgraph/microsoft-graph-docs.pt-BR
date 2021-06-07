---
title: Criar deviceComplianceScheduledActionForRule
description: Criar um novo objeto deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a7b85d77192aedbdcea862aebcca9694b7852e72
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756621"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="dcb26-103">Criar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="dcb26-103">Create deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="dcb26-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcb26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcb26-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dcb26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcb26-106">Criar um novo objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="dcb26-106">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcb26-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dcb26-107">Prerequisites</span></span>
<span data-ttu-id="dcb26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcb26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcb26-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcb26-110">Permission type</span></span>|<span data-ttu-id="dcb26-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dcb26-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcb26-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcb26-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dcb26-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcb26-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dcb26-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcb26-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcb26-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcb26-115">Not supported.</span></span>|
|<span data-ttu-id="dcb26-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcb26-116">Application</span></span>|<span data-ttu-id="dcb26-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcb26-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcb26-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcb26-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="dcb26-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcb26-119">Request headers</span></span>
|<span data-ttu-id="dcb26-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dcb26-120">Header</span></span>|<span data-ttu-id="dcb26-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dcb26-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcb26-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcb26-122">Authorization</span></span>|<span data-ttu-id="dcb26-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcb26-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcb26-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dcb26-124">Accept</span></span>|<span data-ttu-id="dcb26-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dcb26-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcb26-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcb26-126">Request body</span></span>
<span data-ttu-id="dcb26-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="dcb26-127">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="dcb26-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="dcb26-128">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="dcb26-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dcb26-129">Property</span></span>|<span data-ttu-id="dcb26-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcb26-130">Type</span></span>|<span data-ttu-id="dcb26-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcb26-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcb26-132">id</span><span class="sxs-lookup"><span data-stu-id="dcb26-132">id</span></span>|<span data-ttu-id="dcb26-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dcb26-133">String</span></span>|<span data-ttu-id="dcb26-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dcb26-134">Key of the entity.</span></span>|
|<span data-ttu-id="dcb26-135">ruleName</span><span class="sxs-lookup"><span data-stu-id="dcb26-135">ruleName</span></span>|<span data-ttu-id="dcb26-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dcb26-136">String</span></span>|<span data-ttu-id="dcb26-137">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="dcb26-137">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="dcb26-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcb26-138">Response</span></span>
<span data-ttu-id="dcb26-139">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcb26-139">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcb26-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dcb26-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcb26-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcb26-141">Request</span></span>
<span data-ttu-id="dcb26-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcb26-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="dcb26-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcb26-143">Response</span></span>
<span data-ttu-id="dcb26-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcb26-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




