---
title: Ação scheduleActionsForRules
description: Ainda não documentado
ms.openlocfilehash: 7df79c4428834cda8a739a9afb1919282c9e1dbb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006819"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="52941-103">Ação scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="52941-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="52941-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="52941-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52941-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="52941-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="52941-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52941-106">Prerequisites</span></span>
<span data-ttu-id="52941-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52941-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52941-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52941-109">Permission type</span></span>|<span data-ttu-id="52941-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52941-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52941-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52941-111">Delegated (work or school account)</span></span>|<span data-ttu-id="52941-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52941-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="52941-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52941-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52941-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52941-114">Not supported.</span></span>|
|<span data-ttu-id="52941-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52941-115">Application</span></span>|<span data-ttu-id="52941-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52941-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52941-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52941-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="52941-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52941-118">Request headers</span></span>
|<span data-ttu-id="52941-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52941-119">Header</span></span>|<span data-ttu-id="52941-120">Valor</span><span class="sxs-lookup"><span data-stu-id="52941-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52941-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="52941-121">Authorization</span></span>|<span data-ttu-id="52941-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52941-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52941-123">Accept</span><span class="sxs-lookup"><span data-stu-id="52941-123">Accept</span></span>|<span data-ttu-id="52941-124">application/json</span><span class="sxs-lookup"><span data-stu-id="52941-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52941-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52941-125">Request body</span></span>
<span data-ttu-id="52941-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="52941-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="52941-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="52941-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="52941-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52941-128">Property</span></span>|<span data-ttu-id="52941-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="52941-129">Type</span></span>|<span data-ttu-id="52941-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="52941-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52941-131">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="52941-131">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="52941-132">Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="52941-132">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="52941-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="52941-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="52941-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="52941-134">Response</span></span>
<span data-ttu-id="52941-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="52941-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="52941-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52941-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="52941-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52941-137">Request</span></span>
<span data-ttu-id="52941-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52941-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="52941-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="52941-139">Response</span></span>
<span data-ttu-id="52941-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52941-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



