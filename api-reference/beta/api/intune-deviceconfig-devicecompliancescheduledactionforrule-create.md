---
title: Criar deviceComplianceScheduledActionForRule
description: Criar um novo objeto deviceComplianceScheduledActionForRule.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f203b0a4d12dfd3124e359210f13527b8e8b8401
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443171"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="1044c-103">Criar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="1044c-103">Create deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="1044c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1044c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1044c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1044c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1044c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1044c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1044c-107">Criar um novo objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="1044c-107">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1044c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1044c-108">Prerequisites</span></span>
<span data-ttu-id="1044c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1044c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1044c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1044c-111">Permission type</span></span>|<span data-ttu-id="1044c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1044c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1044c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1044c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1044c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1044c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1044c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1044c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1044c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1044c-116">Not supported.</span></span>|
|<span data-ttu-id="1044c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1044c-117">Application</span></span>|<span data-ttu-id="1044c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1044c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1044c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1044c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="1044c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1044c-120">Request headers</span></span>
|<span data-ttu-id="1044c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1044c-121">Header</span></span>|<span data-ttu-id="1044c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1044c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1044c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1044c-123">Authorization</span></span>|<span data-ttu-id="1044c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1044c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1044c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1044c-125">Accept</span></span>|<span data-ttu-id="1044c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1044c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1044c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1044c-127">Request body</span></span>
<span data-ttu-id="1044c-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="1044c-128">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="1044c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="1044c-129">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="1044c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1044c-130">Property</span></span>|<span data-ttu-id="1044c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1044c-131">Type</span></span>|<span data-ttu-id="1044c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1044c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1044c-133">id</span><span class="sxs-lookup"><span data-stu-id="1044c-133">id</span></span>|<span data-ttu-id="1044c-134">String</span><span class="sxs-lookup"><span data-stu-id="1044c-134">String</span></span>|<span data-ttu-id="1044c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1044c-135">Key of the entity.</span></span>|
|<span data-ttu-id="1044c-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="1044c-136">ruleName</span></span>|<span data-ttu-id="1044c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1044c-137">String</span></span>|<span data-ttu-id="1044c-138">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="1044c-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="1044c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1044c-139">Response</span></span>
<span data-ttu-id="1044c-140">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1044c-140">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1044c-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1044c-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="1044c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1044c-142">Request</span></span>
<span data-ttu-id="1044c-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1044c-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="1044c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="1044c-144">Response</span></span>
<span data-ttu-id="1044c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1044c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





