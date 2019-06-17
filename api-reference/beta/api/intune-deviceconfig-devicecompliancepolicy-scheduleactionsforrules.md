---
title: Ação scheduleActionsForRules
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5cc42f774f4a59af637277d38350627a20ac9248
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968424"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="24da8-103">ação scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="24da8-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="24da8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="24da8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24da8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="24da8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24da8-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="24da8-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24da8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="24da8-107">Prerequisites</span></span>
<span data-ttu-id="24da8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24da8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24da8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24da8-110">Permission type</span></span>|<span data-ttu-id="24da8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="24da8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24da8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24da8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24da8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24da8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24da8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24da8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24da8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24da8-115">Not supported.</span></span>|
|<span data-ttu-id="24da8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24da8-116">Application</span></span>|<span data-ttu-id="24da8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24da8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24da8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24da8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="24da8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24da8-119">Request headers</span></span>
|<span data-ttu-id="24da8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24da8-120">Header</span></span>|<span data-ttu-id="24da8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="24da8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24da8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="24da8-122">Authorization</span></span>|<span data-ttu-id="24da8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24da8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24da8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="24da8-124">Accept</span></span>|<span data-ttu-id="24da8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24da8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24da8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24da8-126">Request body</span></span>
<span data-ttu-id="24da8-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="24da8-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="24da8-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="24da8-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="24da8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24da8-129">Property</span></span>|<span data-ttu-id="24da8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="24da8-130">Type</span></span>|<span data-ttu-id="24da8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="24da8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24da8-132">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="24da8-132">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="24da8-133">Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="24da8-133">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="24da8-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="24da8-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="24da8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="24da8-135">Response</span></span>
<span data-ttu-id="24da8-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="24da8-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="24da8-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24da8-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="24da8-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24da8-138">Request</span></span>
<span data-ttu-id="24da8-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24da8-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="24da8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="24da8-140">Response</span></span>
<span data-ttu-id="24da8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24da8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





