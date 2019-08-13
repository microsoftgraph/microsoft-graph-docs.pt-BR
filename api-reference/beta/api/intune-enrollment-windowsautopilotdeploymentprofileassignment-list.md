---
title: Listar windowsAutopilotDeploymentProfileAssignments
description: Listar Propriedades e relações dos objetos windowsAutopilotDeploymentProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b6767337e772efc0a254ed02de0cb7413622e41b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356092"
---
# <a name="list-windowsautopilotdeploymentprofileassignments"></a><span data-ttu-id="2026e-103">Listar windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="2026e-103">List windowsAutopilotDeploymentProfileAssignments</span></span>

> <span data-ttu-id="2026e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2026e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2026e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2026e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2026e-106">Listar Propriedades e relações dos objetos [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2026e-106">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2026e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2026e-107">Prerequisites</span></span>
<span data-ttu-id="2026e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2026e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2026e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2026e-110">Permission type</span></span>|<span data-ttu-id="2026e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2026e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2026e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2026e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2026e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2026e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2026e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2026e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2026e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2026e-115">Not supported.</span></span>|
|<span data-ttu-id="2026e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2026e-116">Application</span></span>|<span data-ttu-id="2026e-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2026e-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2026e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2026e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2026e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2026e-119">Request headers</span></span>
|<span data-ttu-id="2026e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2026e-120">Header</span></span>|<span data-ttu-id="2026e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2026e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2026e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2026e-122">Authorization</span></span>|<span data-ttu-id="2026e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2026e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2026e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2026e-124">Accept</span></span>|<span data-ttu-id="2026e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2026e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2026e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2026e-126">Request body</span></span>
<span data-ttu-id="2026e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2026e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2026e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2026e-128">Response</span></span>
<span data-ttu-id="2026e-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2026e-129">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2026e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2026e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2026e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2026e-131">Request</span></span>
<span data-ttu-id="2026e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2026e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

### <a name="response"></a><span data-ttu-id="2026e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2026e-133">Response</span></span>
<span data-ttu-id="2026e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2026e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
      "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```






