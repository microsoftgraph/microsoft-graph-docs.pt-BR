---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 47866d69a293869c6b4c024c8f79c826a378e7e9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134078"
---
# <a name="assign-action"></a><span data-ttu-id="95336-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="95336-103">assign action</span></span>

<span data-ttu-id="95336-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95336-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95336-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="95336-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95336-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95336-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95336-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="95336-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95336-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="95336-108">Prerequisites</span></span>
<span data-ttu-id="95336-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95336-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95336-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95336-111">Permission type</span></span>|<span data-ttu-id="95336-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95336-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95336-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95336-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95336-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95336-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95336-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95336-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95336-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95336-116">Not supported.</span></span>|
|<span data-ttu-id="95336-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95336-117">Application</span></span>|<span data-ttu-id="95336-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95336-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95336-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95336-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assign
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}/policy/assign
```

## <a name="request-headers"></a><span data-ttu-id="95336-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95336-120">Request headers</span></span>
|<span data-ttu-id="95336-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95336-121">Header</span></span>|<span data-ttu-id="95336-122">Valor</span><span class="sxs-lookup"><span data-stu-id="95336-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95336-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="95336-123">Authorization</span></span>|<span data-ttu-id="95336-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95336-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95336-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="95336-125">Accept</span></span>|<span data-ttu-id="95336-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95336-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95336-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95336-127">Request body</span></span>
<span data-ttu-id="95336-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="95336-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="95336-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="95336-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="95336-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95336-130">Property</span></span>|<span data-ttu-id="95336-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="95336-131">Type</span></span>|<span data-ttu-id="95336-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="95336-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95336-133">wdacPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="95336-133">wdacPolicyAssignments</span></span>|<span data-ttu-id="95336-134">[coleção windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="95336-134">[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) collection</span></span>|<span data-ttu-id="95336-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="95336-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="95336-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="95336-136">Response</span></span>
<span data-ttu-id="95336-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="95336-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="95336-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95336-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="95336-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95336-139">Request</span></span>
<span data-ttu-id="95336-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95336-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="95336-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="95336-141">Response</span></span>
<span data-ttu-id="95336-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95336-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




