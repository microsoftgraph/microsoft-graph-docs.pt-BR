---
title: Criar deviceComplianceScheduledActionForRule
description: Criar um novo objeto deviceComplianceScheduledActionForRule.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 59e19e57de47bfa3e2ad4322b09129d07546317d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35949654"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="2cdb2-103">Criar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="2cdb2-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="2cdb2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2cdb2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cdb2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2cdb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cdb2-106">Criar um novo objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="2cdb2-106">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cdb2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2cdb2-107">Prerequisites</span></span>
<span data-ttu-id="2cdb2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cdb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cdb2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2cdb2-110">Permission type</span></span>|<span data-ttu-id="2cdb2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2cdb2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cdb2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2cdb2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2cdb2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cdb2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2cdb2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2cdb2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cdb2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cdb2-115">Not supported.</span></span>|
|<span data-ttu-id="2cdb2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2cdb2-116">Application</span></span>|<span data-ttu-id="2cdb2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cdb2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cdb2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2cdb2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="2cdb2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2cdb2-119">Request headers</span></span>
|<span data-ttu-id="2cdb2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2cdb2-120">Header</span></span>|<span data-ttu-id="2cdb2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2cdb2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cdb2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2cdb2-122">Authorization</span></span>|<span data-ttu-id="2cdb2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2cdb2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cdb2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2cdb2-124">Accept</span></span>|<span data-ttu-id="2cdb2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2cdb2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cdb2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2cdb2-126">Request body</span></span>
<span data-ttu-id="2cdb2-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="2cdb2-127">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="2cdb2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="2cdb2-128">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="2cdb2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2cdb2-129">Property</span></span>|<span data-ttu-id="2cdb2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cdb2-130">Type</span></span>|<span data-ttu-id="2cdb2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cdb2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cdb2-132">id</span><span class="sxs-lookup"><span data-stu-id="2cdb2-132">id</span></span>|<span data-ttu-id="2cdb2-133">String</span><span class="sxs-lookup"><span data-stu-id="2cdb2-133">String</span></span>|<span data-ttu-id="2cdb2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2cdb2-134">Key of the entity.</span></span>|
|<span data-ttu-id="2cdb2-135">ruleName</span><span class="sxs-lookup"><span data-stu-id="2cdb2-135">ruleName</span></span>|<span data-ttu-id="2cdb2-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2cdb2-136">String</span></span>|<span data-ttu-id="2cdb2-137">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="2cdb2-137">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="2cdb2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cdb2-138">Response</span></span>
<span data-ttu-id="2cdb2-139">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2cdb2-139">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cdb2-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2cdb2-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cdb2-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2cdb2-141">Request</span></span>
<span data-ttu-id="2cdb2-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2cdb2-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="2cdb2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cdb2-143">Response</span></span>
<span data-ttu-id="2cdb2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2cdb2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





