---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 142fb4168d37184c30c0c3d5c7eeaa01cd9fa23f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791269"
---
# <a name="assign-action"></a><span data-ttu-id="c68e9-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="c68e9-103">assign action</span></span>

<span data-ttu-id="c68e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c68e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c68e9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c68e9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c68e9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c68e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c68e9-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c68e9-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c68e9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c68e9-108">Prerequisites</span></span>
<span data-ttu-id="c68e9-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c68e9-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c68e9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c68e9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c68e9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c68e9-111">Permission type</span></span>|<span data-ttu-id="c68e9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c68e9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c68e9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c68e9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c68e9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c68e9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c68e9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c68e9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c68e9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c68e9-116">Not supported.</span></span>|
|<span data-ttu-id="c68e9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c68e9-117">Application</span></span>|<span data-ttu-id="c68e9-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c68e9-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c68e9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c68e9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assign
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}/policy/assign
```

## <a name="request-headers"></a><span data-ttu-id="c68e9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c68e9-120">Request headers</span></span>
|<span data-ttu-id="c68e9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c68e9-121">Header</span></span>|<span data-ttu-id="c68e9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c68e9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c68e9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c68e9-123">Authorization</span></span>|<span data-ttu-id="c68e9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c68e9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c68e9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c68e9-125">Accept</span></span>|<span data-ttu-id="c68e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c68e9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c68e9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c68e9-127">Request body</span></span>
<span data-ttu-id="c68e9-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c68e9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c68e9-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c68e9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c68e9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c68e9-130">Property</span></span>|<span data-ttu-id="c68e9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c68e9-131">Type</span></span>|<span data-ttu-id="c68e9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c68e9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c68e9-133">wdacPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="c68e9-133">wdacPolicyAssignments</span></span>|<span data-ttu-id="c68e9-134">coleção [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c68e9-134">[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) collection</span></span>|<span data-ttu-id="c68e9-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c68e9-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c68e9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c68e9-136">Response</span></span>
<span data-ttu-id="c68e9-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c68e9-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c68e9-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c68e9-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c68e9-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c68e9-139">Request</span></span>
<span data-ttu-id="c68e9-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c68e9-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assign

Content-type: application/json
Content-length: 494

{
  "wdacPolicyAssignments": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
      "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c68e9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c68e9-141">Response</span></span>
<span data-ttu-id="c68e9-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="c68e9-142">Here is an example of the response.</span></span> <span data-ttu-id="c68e9-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="c68e9-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c68e9-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c68e9-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



