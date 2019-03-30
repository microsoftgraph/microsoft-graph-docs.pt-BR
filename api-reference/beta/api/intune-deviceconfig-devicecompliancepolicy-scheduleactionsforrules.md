---
title: Ação scheduleActionsForRules
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 759d6a6f9f786e52d2d3966a62c62792b6387c76
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987150"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="50187-103">ação scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="50187-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="50187-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50187-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50187-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50187-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50187-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="50187-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50187-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50187-107">Prerequisites</span></span>
<span data-ttu-id="50187-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50187-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50187-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50187-110">Permission type</span></span>|<span data-ttu-id="50187-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50187-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50187-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50187-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50187-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50187-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50187-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50187-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50187-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50187-115">Not supported.</span></span>|
|<span data-ttu-id="50187-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50187-116">Application</span></span>|<span data-ttu-id="50187-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50187-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50187-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50187-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="50187-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50187-119">Request headers</span></span>
|<span data-ttu-id="50187-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50187-120">Header</span></span>|<span data-ttu-id="50187-121">Valor</span><span class="sxs-lookup"><span data-stu-id="50187-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50187-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="50187-122">Authorization</span></span>|<span data-ttu-id="50187-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50187-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50187-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50187-124">Accept</span></span>|<span data-ttu-id="50187-125">application/json</span><span class="sxs-lookup"><span data-stu-id="50187-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50187-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50187-126">Request body</span></span>
<span data-ttu-id="50187-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="50187-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="50187-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="50187-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="50187-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50187-129">Property</span></span>|<span data-ttu-id="50187-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="50187-130">Type</span></span>|<span data-ttu-id="50187-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="50187-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50187-132">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="50187-132">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="50187-133">Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="50187-133">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="50187-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="50187-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="50187-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="50187-135">Response</span></span>
<span data-ttu-id="50187-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="50187-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="50187-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50187-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="50187-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50187-138">Request</span></span>
<span data-ttu-id="50187-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50187-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules

Content-type: application/json
Content-length: 242

{
  "deviceComplianceScheduledActionForRules": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
      "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
      "ruleName": "Rule Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="50187-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="50187-140">Response</span></span>
<span data-ttu-id="50187-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50187-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




