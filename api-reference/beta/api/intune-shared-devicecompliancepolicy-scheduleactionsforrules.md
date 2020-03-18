---
title: Ação scheduleActionsForRules
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07af9d9f21891c0ff3547dcb10ca080584bc6617
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801170"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="d3389-103">ação scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="d3389-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="d3389-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3389-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3389-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3389-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3389-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d3389-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3389-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3389-107">Prerequisites</span></span>
<span data-ttu-id="d3389-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3389-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3389-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3389-110">Permission type</span></span>|<span data-ttu-id="d3389-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3389-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3389-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3389-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d3389-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d3389-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d3389-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3389-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3389-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3389-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3389-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3389-116">Not supported.</span></span>|
|<span data-ttu-id="d3389-117">Application</span><span class="sxs-lookup"><span data-stu-id="d3389-117">Application</span></span>||
| <span data-ttu-id="d3389-118">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d3389-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d3389-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3389-119">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3389-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3389-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="d3389-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3389-121">Request headers</span></span>
|<span data-ttu-id="d3389-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3389-122">Header</span></span>|<span data-ttu-id="d3389-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d3389-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3389-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3389-124">Authorization</span></span>|<span data-ttu-id="d3389-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3389-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3389-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3389-126">Accept</span></span>|<span data-ttu-id="d3389-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d3389-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3389-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3389-128">Request body</span></span>
<span data-ttu-id="d3389-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d3389-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d3389-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d3389-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d3389-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3389-131">Property</span></span>|<span data-ttu-id="d3389-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3389-132">Type</span></span>|<span data-ttu-id="d3389-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3389-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3389-134">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="d3389-134">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="d3389-135">Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="d3389-135">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="d3389-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d3389-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d3389-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3389-137">Response</span></span>
<span data-ttu-id="d3389-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d3389-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d3389-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3389-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3389-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3389-140">Request</span></span>
<span data-ttu-id="d3389-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3389-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d3389-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3389-142">Response</span></span>
<span data-ttu-id="d3389-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3389-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







