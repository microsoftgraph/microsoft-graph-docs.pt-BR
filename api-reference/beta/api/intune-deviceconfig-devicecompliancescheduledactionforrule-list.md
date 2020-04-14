---
title: Listar deviceComplianceScheduledActionForRules
description: Listar propriedades e relações dos objetos deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d34a838515c55ed4c54cd408af4046baedbb1193
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433873"
---
# <a name="list-devicecompliancescheduledactionforrules"></a><span data-ttu-id="e5231-103">Listar deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="e5231-103">List deviceComplianceScheduledActionForRules</span></span>

<span data-ttu-id="e5231-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5231-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5231-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5231-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5231-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5231-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5231-107">Listar propriedades e relações dos objetos [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="e5231-107">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5231-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e5231-108">Prerequisites</span></span>
<span data-ttu-id="e5231-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5231-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5231-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5231-111">Permission type</span></span>|<span data-ttu-id="e5231-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e5231-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5231-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5231-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5231-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5231-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e5231-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5231-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5231-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5231-116">Not supported.</span></span>|
|<span data-ttu-id="e5231-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5231-117">Application</span></span>|<span data-ttu-id="e5231-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5231-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5231-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5231-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="e5231-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5231-120">Request headers</span></span>
|<span data-ttu-id="e5231-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5231-121">Header</span></span>|<span data-ttu-id="e5231-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e5231-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5231-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5231-123">Authorization</span></span>|<span data-ttu-id="e5231-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5231-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5231-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e5231-125">Accept</span></span>|<span data-ttu-id="e5231-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5231-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5231-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5231-127">Request body</span></span>
<span data-ttu-id="e5231-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5231-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5231-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5231-129">Response</span></span>
<span data-ttu-id="e5231-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5231-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5231-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5231-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5231-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5231-132">Request</span></span>
<span data-ttu-id="e5231-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5231-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

### <a name="response"></a><span data-ttu-id="e5231-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5231-134">Response</span></span>
<span data-ttu-id="e5231-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5231-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 208

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
      "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
      "ruleName": "Rule Name value"
    }
  ]
}
```



