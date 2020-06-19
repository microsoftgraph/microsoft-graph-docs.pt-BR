---
title: Listar windowsAutopilotDeploymentProfileAssignments
description: Listar Propriedades e relações dos objetos windowsAutopilotDeploymentProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7069764bc372ce1a7da396f099f478ed50244aae
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792040"
---
# <a name="list-windowsautopilotdeploymentprofileassignments"></a><span data-ttu-id="2f6d5-103">Listar windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="2f6d5-103">List windowsAutopilotDeploymentProfileAssignments</span></span>

<span data-ttu-id="2f6d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f6d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f6d5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f6d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f6d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f6d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f6d5-107">Listar Propriedades e relações dos objetos [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2f6d5-107">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f6d5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f6d5-108">Prerequisites</span></span>
<span data-ttu-id="2f6d5-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="2f6d5-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2f6d5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f6d5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f6d5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f6d5-111">Permission type</span></span>|<span data-ttu-id="2f6d5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f6d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f6d5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f6d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f6d5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f6d5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2f6d5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f6d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f6d5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f6d5-116">Not supported.</span></span>|
|<span data-ttu-id="2f6d5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f6d5-117">Application</span></span>|<span data-ttu-id="2f6d5-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f6d5-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f6d5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f6d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2f6d5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f6d5-120">Request headers</span></span>
|<span data-ttu-id="2f6d5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f6d5-121">Header</span></span>|<span data-ttu-id="2f6d5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2f6d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f6d5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f6d5-123">Authorization</span></span>|<span data-ttu-id="2f6d5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f6d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f6d5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f6d5-125">Accept</span></span>|<span data-ttu-id="2f6d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f6d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f6d5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f6d5-127">Request body</span></span>
<span data-ttu-id="2f6d5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f6d5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f6d5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f6d5-129">Response</span></span>
<span data-ttu-id="2f6d5-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f6d5-130">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f6d5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f6d5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f6d5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f6d5-132">Request</span></span>
<span data-ttu-id="2f6d5-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f6d5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

### <a name="response"></a><span data-ttu-id="2f6d5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f6d5-134">Response</span></span>
<span data-ttu-id="2f6d5-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="2f6d5-135">Here is an example of the response.</span></span> <span data-ttu-id="2f6d5-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="2f6d5-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2f6d5-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="2f6d5-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
      "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```



