---
title: Criar deviceComplianceScheduledActionForRule
description: Criar um novo objeto deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 217ad13de93f45ce288a39cad766ce2e64dc97cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926607"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="217a3-103">Criar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="217a3-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="217a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="217a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="217a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="217a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="217a3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="217a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="217a3-107">Criar um novo objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="217a3-107">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="217a3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="217a3-108">Prerequisites</span></span>
<span data-ttu-id="217a3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="217a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="217a3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="217a3-111">Permission type</span></span>|<span data-ttu-id="217a3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="217a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="217a3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="217a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="217a3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="217a3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="217a3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="217a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="217a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="217a3-116">Not supported.</span></span>|
|<span data-ttu-id="217a3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="217a3-117">Application</span></span>|<span data-ttu-id="217a3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="217a3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="217a3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="217a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="217a3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="217a3-120">Request headers</span></span>
|<span data-ttu-id="217a3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="217a3-121">Header</span></span>|<span data-ttu-id="217a3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="217a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="217a3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="217a3-123">Authorization</span></span>|<span data-ttu-id="217a3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="217a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="217a3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="217a3-125">Accept</span></span>|<span data-ttu-id="217a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="217a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="217a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="217a3-127">Request body</span></span>
<span data-ttu-id="217a3-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="217a3-128">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="217a3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="217a3-129">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="217a3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="217a3-130">Property</span></span>|<span data-ttu-id="217a3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="217a3-131">Type</span></span>|<span data-ttu-id="217a3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="217a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="217a3-133">id</span><span class="sxs-lookup"><span data-stu-id="217a3-133">id</span></span>|<span data-ttu-id="217a3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="217a3-134">String</span></span>|<span data-ttu-id="217a3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="217a3-135">Key of the entity.</span></span>|
|<span data-ttu-id="217a3-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="217a3-136">ruleName</span></span>|<span data-ttu-id="217a3-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="217a3-137">String</span></span>|<span data-ttu-id="217a3-138">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="217a3-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="217a3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="217a3-139">Response</span></span>
<span data-ttu-id="217a3-140">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="217a3-140">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="217a3-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="217a3-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="217a3-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="217a3-142">Request</span></span>
<span data-ttu-id="217a3-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="217a3-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="217a3-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="217a3-144">Response</span></span>
<span data-ttu-id="217a3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="217a3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





