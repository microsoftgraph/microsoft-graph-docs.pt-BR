---
title: Ação scheduleActionsForRules
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 60499e19016b7bd8fa6c18d0a22bb59865a540fc
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086169"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="82a6d-103">ação scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="82a6d-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="82a6d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="82a6d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82a6d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82a6d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82a6d-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82a6d-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82a6d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82a6d-107">Prerequisites</span></span>
<span data-ttu-id="82a6d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82a6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82a6d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82a6d-110">Permission type</span></span>|<span data-ttu-id="82a6d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="82a6d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82a6d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82a6d-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="82a6d-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="82a6d-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="82a6d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82a6d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82a6d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82a6d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82a6d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82a6d-116">Not supported.</span></span>|
|<span data-ttu-id="82a6d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82a6d-117">Application</span></span>||
| <span data-ttu-id="82a6d-118">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="82a6d-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="82a6d-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82a6d-119">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82a6d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82a6d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="82a6d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82a6d-121">Request headers</span></span>
|<span data-ttu-id="82a6d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82a6d-122">Header</span></span>|<span data-ttu-id="82a6d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="82a6d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82a6d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="82a6d-124">Authorization</span></span>|<span data-ttu-id="82a6d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82a6d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82a6d-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="82a6d-126">Accept</span></span>|<span data-ttu-id="82a6d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="82a6d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82a6d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82a6d-128">Request body</span></span>
<span data-ttu-id="82a6d-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="82a6d-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="82a6d-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="82a6d-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="82a6d-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82a6d-131">Property</span></span>|<span data-ttu-id="82a6d-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="82a6d-132">Type</span></span>|<span data-ttu-id="82a6d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="82a6d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82a6d-134">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="82a6d-134">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="82a6d-135">Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="82a6d-135">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="82a6d-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82a6d-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="82a6d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="82a6d-137">Response</span></span>
<span data-ttu-id="82a6d-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="82a6d-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="82a6d-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82a6d-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="82a6d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82a6d-140">Request</span></span>
<span data-ttu-id="82a6d-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82a6d-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82a6d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="82a6d-142">Response</span></span>
<span data-ttu-id="82a6d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82a6d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









