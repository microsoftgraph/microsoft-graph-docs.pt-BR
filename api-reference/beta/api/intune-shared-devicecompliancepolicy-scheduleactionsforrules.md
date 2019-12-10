---
title: Ação scheduleActionsForRules
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f01770280fe5c1d588d4cfeb5b9ce240fb0dfe16
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940093"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="c1a1f-103">ação scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="c1a1f-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="c1a1f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c1a1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1a1f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c1a1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1a1f-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c1a1f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1a1f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c1a1f-107">Prerequisites</span></span>
<span data-ttu-id="c1a1f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1a1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1a1f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1a1f-110">Permission type</span></span>|<span data-ttu-id="c1a1f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c1a1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1a1f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1a1f-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c1a1f-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c1a1f-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c1a1f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1a1f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1a1f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1a1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1a1f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1a1f-116">Not supported.</span></span>|
|<span data-ttu-id="c1a1f-117">Application</span><span class="sxs-lookup"><span data-stu-id="c1a1f-117">Application</span></span>||
| <span data-ttu-id="c1a1f-118">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c1a1f-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c1a1f-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1a1f-119">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1a1f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1a1f-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="c1a1f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1a1f-121">Request headers</span></span>
|<span data-ttu-id="c1a1f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c1a1f-122">Header</span></span>|<span data-ttu-id="c1a1f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c1a1f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1a1f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1a1f-124">Authorization</span></span>|<span data-ttu-id="c1a1f-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1a1f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1a1f-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c1a1f-126">Accept</span></span>|<span data-ttu-id="c1a1f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c1a1f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1a1f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1a1f-128">Request body</span></span>
<span data-ttu-id="c1a1f-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c1a1f-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c1a1f-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c1a1f-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c1a1f-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1a1f-131">Property</span></span>|<span data-ttu-id="c1a1f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1a1f-132">Type</span></span>|<span data-ttu-id="c1a1f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1a1f-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1a1f-134">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="c1a1f-134">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="c1a1f-135">Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="c1a1f-135">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="c1a1f-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c1a1f-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c1a1f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1a1f-137">Response</span></span>
<span data-ttu-id="c1a1f-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c1a1f-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c1a1f-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1a1f-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1a1f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1a1f-140">Request</span></span>
<span data-ttu-id="c1a1f-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1a1f-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1a1f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1a1f-142">Response</span></span>
<span data-ttu-id="c1a1f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1a1f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








