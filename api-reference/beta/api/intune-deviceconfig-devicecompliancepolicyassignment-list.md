---
title: Listar deviceCompliancePolicyAssignments
description: Listar propriedades e relações dos objetosdeviceCompliancePolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1eca501ef89ddd3badb14ecd58e0f5c692a9c80c
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793028"
---
# <a name="list-devicecompliancepolicyassignments"></a><span data-ttu-id="f6f5b-103">Listar deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="f6f5b-103">List deviceCompliancePolicyAssignments</span></span>

<span data-ttu-id="f6f5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6f5b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6f5b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6f5b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6f5b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6f5b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6f5b-107">Listar propriedades e relações dos objetos[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f6f5b-107">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6f5b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f6f5b-108">Prerequisites</span></span>
<span data-ttu-id="f6f5b-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f6f5b-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f6f5b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6f5b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6f5b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6f5b-111">Permission type</span></span>|<span data-ttu-id="f6f5b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f6f5b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6f5b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6f5b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6f5b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6f5b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f6f5b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6f5b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6f5b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6f5b-116">Not supported.</span></span>|
|<span data-ttu-id="f6f5b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6f5b-117">Application</span></span>|<span data-ttu-id="f6f5b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6f5b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6f5b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6f5b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f6f5b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6f5b-120">Request headers</span></span>
|<span data-ttu-id="f6f5b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6f5b-121">Header</span></span>|<span data-ttu-id="f6f5b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f6f5b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6f5b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6f5b-123">Authorization</span></span>|<span data-ttu-id="f6f5b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6f5b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6f5b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f6f5b-125">Accept</span></span>|<span data-ttu-id="f6f5b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6f5b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6f5b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6f5b-127">Request body</span></span>
<span data-ttu-id="f6f5b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f6f5b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6f5b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6f5b-129">Response</span></span>
<span data-ttu-id="f6f5b-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6f5b-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6f5b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6f5b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6f5b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6f5b-132">Request</span></span>
<span data-ttu-id="f6f5b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6f5b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="f6f5b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6f5b-134">Response</span></span>
<span data-ttu-id="f6f5b-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="f6f5b-135">Here is an example of the response.</span></span> <span data-ttu-id="f6f5b-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f6f5b-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f6f5b-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f6f5b-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 506

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```



