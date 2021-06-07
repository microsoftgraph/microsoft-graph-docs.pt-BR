---
title: Listar deviceComplianceScheduledActionForRules
description: Listar propriedades e relações dos objetos deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6dba306e8a83c9cc3f2f066b96fcfab0a3ae1e84
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756600"
---
# <a name="list-devicecompliancescheduledactionforrules"></a><span data-ttu-id="1ec5d-103">Listar deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="1ec5d-103">List deviceComplianceScheduledActionForRules</span></span>

<span data-ttu-id="1ec5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ec5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ec5d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ec5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ec5d-106">Listar propriedades e relações dos objetos [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="1ec5d-106">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ec5d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ec5d-107">Prerequisites</span></span>
<span data-ttu-id="1ec5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ec5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ec5d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ec5d-110">Permission type</span></span>|<span data-ttu-id="1ec5d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1ec5d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ec5d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ec5d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ec5d-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ec5d-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ec5d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ec5d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ec5d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ec5d-115">Not supported.</span></span>|
|<span data-ttu-id="1ec5d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ec5d-116">Application</span></span>|<span data-ttu-id="1ec5d-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ec5d-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ec5d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ec5d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="1ec5d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ec5d-119">Request headers</span></span>
|<span data-ttu-id="1ec5d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ec5d-120">Header</span></span>|<span data-ttu-id="1ec5d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1ec5d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ec5d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ec5d-122">Authorization</span></span>|<span data-ttu-id="1ec5d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ec5d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ec5d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ec5d-124">Accept</span></span>|<span data-ttu-id="1ec5d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ec5d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ec5d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ec5d-126">Request body</span></span>
<span data-ttu-id="1ec5d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1ec5d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ec5d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ec5d-128">Response</span></span>
<span data-ttu-id="1ec5d-129">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ec5d-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ec5d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ec5d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ec5d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ec5d-131">Request</span></span>
<span data-ttu-id="1ec5d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ec5d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

### <a name="response"></a><span data-ttu-id="1ec5d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ec5d-133">Response</span></span>
<span data-ttu-id="1ec5d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ec5d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




