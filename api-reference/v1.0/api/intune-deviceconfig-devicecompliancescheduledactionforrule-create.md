---
title: Criar deviceComplianceScheduledActionForRule
description: Criar um novo objeto deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fac03ca9bf037a92bdc36cbadbf1ac7da437e849
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941755"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="6a6a0-103">Criar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="6a6a0-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="6a6a0-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6a6a0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a6a0-105">Criar um novo objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="6a6a0-105">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6a6a0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a6a0-106">Prerequisites</span></span>
<span data-ttu-id="6a6a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a6a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a6a0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a6a0-109">Permission type</span></span>|<span data-ttu-id="6a6a0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a6a0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a6a0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a6a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a6a0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a6a0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a6a0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a6a0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a6a0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a6a0-114">Not supported.</span></span>|
|<span data-ttu-id="6a6a0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a6a0-115">Application</span></span>|<span data-ttu-id="6a6a0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a6a0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a6a0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a6a0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="6a6a0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a6a0-118">Request headers</span></span>
|<span data-ttu-id="6a6a0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a6a0-119">Header</span></span>|<span data-ttu-id="6a6a0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6a6a0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a6a0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a6a0-121">Authorization</span></span>|<span data-ttu-id="6a6a0-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a6a0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a6a0-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a6a0-123">Accept</span></span>|<span data-ttu-id="6a6a0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6a6a0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a6a0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a6a0-125">Request body</span></span>
<span data-ttu-id="6a6a0-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="6a6a0-126">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="6a6a0-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="6a6a0-127">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="6a6a0-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a6a0-128">Property</span></span>|<span data-ttu-id="6a6a0-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a6a0-129">Type</span></span>|<span data-ttu-id="6a6a0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a6a0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a6a0-131">id</span><span class="sxs-lookup"><span data-stu-id="6a6a0-131">id</span></span>|<span data-ttu-id="6a6a0-132">String</span><span class="sxs-lookup"><span data-stu-id="6a6a0-132">String</span></span>|<span data-ttu-id="6a6a0-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6a6a0-133">Key of the entity.</span></span>|
|<span data-ttu-id="6a6a0-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="6a6a0-134">ruleName</span></span>|<span data-ttu-id="6a6a0-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a6a0-135">String</span></span>|<span data-ttu-id="6a6a0-136">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="6a6a0-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="6a6a0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a6a0-137">Response</span></span>
<span data-ttu-id="6a6a0-138">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a6a0-138">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a6a0-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a6a0-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="6a6a0-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a6a0-140">Request</span></span>
<span data-ttu-id="6a6a0-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a6a0-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="6a6a0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a6a0-142">Response</span></span>
<span data-ttu-id="6a6a0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a6a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



