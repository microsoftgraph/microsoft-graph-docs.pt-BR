---
title: Listar deviceComplianceScheduledActionForRules
description: Listar propriedades e relações dos objetos deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 95e15206f30cefd0115ae508ce119554ec99fe0d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258398"
---
# <a name="list-devicecompliancescheduledactionforrules"></a><span data-ttu-id="39b6d-103">Listar deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="39b6d-103">List deviceComplianceScheduledActionForRules</span></span>

> <span data-ttu-id="39b6d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39b6d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39b6d-105">Listar propriedades e relações dos objetos [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="39b6d-105">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39b6d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="39b6d-106">Prerequisites</span></span>
<span data-ttu-id="39b6d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="39b6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="39b6d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39b6d-109">Permission type</span></span>|<span data-ttu-id="39b6d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="39b6d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39b6d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39b6d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="39b6d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="39b6d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="39b6d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39b6d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39b6d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39b6d-114">Not supported.</span></span>|
|<span data-ttu-id="39b6d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39b6d-115">Application</span></span>|<span data-ttu-id="39b6d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39b6d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39b6d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39b6d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="39b6d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39b6d-118">Request headers</span></span>
|<span data-ttu-id="39b6d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39b6d-119">Header</span></span>|<span data-ttu-id="39b6d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="39b6d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39b6d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="39b6d-121">Authorization</span></span>|<span data-ttu-id="39b6d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39b6d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39b6d-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="39b6d-123">Accept</span></span>|<span data-ttu-id="39b6d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="39b6d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39b6d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39b6d-125">Request body</span></span>
<span data-ttu-id="39b6d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="39b6d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39b6d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="39b6d-127">Response</span></span>
<span data-ttu-id="39b6d-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39b6d-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39b6d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39b6d-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="39b6d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39b6d-130">Request</span></span>
<span data-ttu-id="39b6d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39b6d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

### <a name="response"></a><span data-ttu-id="39b6d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="39b6d-132">Response</span></span>
<span data-ttu-id="39b6d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39b6d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



