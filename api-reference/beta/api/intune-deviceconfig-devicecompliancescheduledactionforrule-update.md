---
title: Atualizar deviceComplianceScheduledActionForRule
description: Atualizar as propriedades de um objeto deviceComplianceScheduledActionForRule.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d2ae868b5c11220423c4f1ee496c77f8cd0482c4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414638"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="6a76d-103">Atualizar deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="6a76d-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="6a76d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6a76d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6a76d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6a76d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a76d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6a76d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a76d-107">Atualizar as propriedades de um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="6a76d-107">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a76d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a76d-108">Prerequisites</span></span>
<span data-ttu-id="6a76d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6a76d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6a76d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a76d-111">Permission type</span></span>|<span data-ttu-id="6a76d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a76d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a76d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a76d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a76d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a76d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a76d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a76d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a76d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a76d-116">Not supported.</span></span>|
|<span data-ttu-id="6a76d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a76d-117">Application</span></span>|<span data-ttu-id="6a76d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a76d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a76d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a76d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="6a76d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a76d-120">Request headers</span></span>
|<span data-ttu-id="6a76d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a76d-121">Header</span></span>|<span data-ttu-id="6a76d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6a76d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a76d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a76d-123">Authorization</span></span>|<span data-ttu-id="6a76d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a76d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a76d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a76d-125">Accept</span></span>|<span data-ttu-id="6a76d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a76d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a76d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a76d-127">Request body</span></span>
<span data-ttu-id="6a76d-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="6a76d-128">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="6a76d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="6a76d-129">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="6a76d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a76d-130">Property</span></span>|<span data-ttu-id="6a76d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a76d-131">Type</span></span>|<span data-ttu-id="6a76d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a76d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a76d-133">id</span><span class="sxs-lookup"><span data-stu-id="6a76d-133">id</span></span>|<span data-ttu-id="6a76d-134">String</span><span class="sxs-lookup"><span data-stu-id="6a76d-134">String</span></span>|<span data-ttu-id="6a76d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6a76d-135">Key of the entity.</span></span>|
|<span data-ttu-id="6a76d-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="6a76d-136">ruleName</span></span>|<span data-ttu-id="6a76d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a76d-137">String</span></span>|<span data-ttu-id="6a76d-138">Nome da regra à qual essa ação agendada se aplica.</span><span class="sxs-lookup"><span data-stu-id="6a76d-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="6a76d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a76d-139">Response</span></span>
<span data-ttu-id="6a76d-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a76d-140">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a76d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a76d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a76d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a76d-142">Request</span></span>
<span data-ttu-id="6a76d-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a76d-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="6a76d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a76d-144">Response</span></span>
<span data-ttu-id="6a76d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a76d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




