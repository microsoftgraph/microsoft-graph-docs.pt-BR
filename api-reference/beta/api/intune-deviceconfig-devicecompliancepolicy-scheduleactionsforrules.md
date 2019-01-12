---
title: Ação scheduleActionsForRules
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 63b244d1c3a2d4c2099eca6e4edcbfdf54e50410
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967781"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="ff4ff-103">Ação scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="ff4ff-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="ff4ff-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff4ff-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff4ff-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff4ff-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ff4ff-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff4ff-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff4ff-108">Prerequisites</span></span>
<span data-ttu-id="ff4ff-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff4ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff4ff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff4ff-111">Permission type</span></span>|<span data-ttu-id="ff4ff-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff4ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff4ff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff4ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff4ff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff4ff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff4ff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff4ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff4ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-116">Not supported.</span></span>|
|<span data-ttu-id="ff4ff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff4ff-117">Application</span></span>|<span data-ttu-id="ff4ff-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff4ff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff4ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="ff4ff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff4ff-120">Request headers</span></span>
|<span data-ttu-id="ff4ff-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff4ff-121">Header</span></span>|<span data-ttu-id="ff4ff-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ff4ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff4ff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff4ff-123">Authorization</span></span>|<span data-ttu-id="ff4ff-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff4ff-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff4ff-125">Accept</span></span>|<span data-ttu-id="ff4ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff4ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff4ff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff4ff-127">Request body</span></span>
<span data-ttu-id="ff4ff-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ff4ff-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ff4ff-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff4ff-130">Property</span></span>|<span data-ttu-id="ff4ff-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff4ff-131">Type</span></span>|<span data-ttu-id="ff4ff-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff4ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff4ff-133">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="ff4ff-133">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="ff4ff-134">Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="ff4ff-134">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="ff4ff-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ff4ff-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ff4ff-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff4ff-136">Response</span></span>
<span data-ttu-id="ff4ff-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ff4ff-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff4ff-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff4ff-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff4ff-139">Request</span></span>
<span data-ttu-id="ff4ff-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ff4ff-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff4ff-141">Response</span></span>
<span data-ttu-id="ff4ff-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





