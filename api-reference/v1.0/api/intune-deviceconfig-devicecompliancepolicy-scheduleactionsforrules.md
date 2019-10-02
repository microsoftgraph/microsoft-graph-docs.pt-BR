---
title: Ação scheduleActionsForRules
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dd43861eeba5b4d166dd03c34b83cec69379cec5
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354242"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="ec430-103">ação scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="ec430-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="ec430-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec430-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec430-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ec430-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec430-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ec430-106">Prerequisites</span></span>
<span data-ttu-id="ec430-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec430-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec430-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec430-109">Permission type</span></span>|<span data-ttu-id="ec430-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ec430-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec430-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec430-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ec430-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec430-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ec430-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec430-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec430-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec430-114">Not supported.</span></span>|
|<span data-ttu-id="ec430-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec430-115">Application</span></span>|<span data-ttu-id="ec430-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec430-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec430-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec430-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="ec430-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec430-118">Request headers</span></span>
|<span data-ttu-id="ec430-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec430-119">Header</span></span>|<span data-ttu-id="ec430-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ec430-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec430-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec430-121">Authorization</span></span>|<span data-ttu-id="ec430-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec430-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec430-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ec430-123">Accept</span></span>|<span data-ttu-id="ec430-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ec430-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec430-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec430-125">Request body</span></span>
<span data-ttu-id="ec430-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ec430-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ec430-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ec430-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ec430-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec430-128">Property</span></span>|<span data-ttu-id="ec430-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec430-129">Type</span></span>|<span data-ttu-id="ec430-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec430-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec430-131">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="ec430-131">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="ec430-132">Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="ec430-132">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="ec430-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ec430-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ec430-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec430-134">Response</span></span>
<span data-ttu-id="ec430-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ec430-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ec430-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec430-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec430-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec430-137">Request</span></span>
<span data-ttu-id="ec430-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec430-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules

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

### <a name="response"></a><span data-ttu-id="ec430-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec430-139">Response</span></span>
<span data-ttu-id="ec430-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec430-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




