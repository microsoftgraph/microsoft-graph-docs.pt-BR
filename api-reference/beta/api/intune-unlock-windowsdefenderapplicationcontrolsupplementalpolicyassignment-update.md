---
title: Atualizar windowsDefenderApplicationControlSupplementalPolicyAssignment
description: Atualiza as propriedades de um objeto windowsDefenderApplicationControlSupplementalPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 89e958ee31dc09112f9279e7ad170f144c088d5f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791248"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="aee4b-103">Atualizar windowsDefenderApplicationControlSupplementalPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="aee4b-103">Update windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

<span data-ttu-id="aee4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aee4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aee4b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aee4b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aee4b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aee4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aee4b-107">Atualiza as propriedades de um objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="aee4b-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aee4b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aee4b-108">Prerequisites</span></span>
<span data-ttu-id="aee4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aee4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aee4b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aee4b-111">Permission type</span></span>|<span data-ttu-id="aee4b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aee4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aee4b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aee4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aee4b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aee4b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aee4b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aee4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aee4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aee4b-116">Not supported.</span></span>|
|<span data-ttu-id="aee4b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aee4b-117">Application</span></span>|<span data-ttu-id="aee4b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aee4b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aee4b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aee4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="aee4b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aee4b-120">Request headers</span></span>
|<span data-ttu-id="aee4b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aee4b-121">Header</span></span>|<span data-ttu-id="aee4b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aee4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aee4b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aee4b-123">Authorization</span></span>|<span data-ttu-id="aee4b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aee4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aee4b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aee4b-125">Accept</span></span>|<span data-ttu-id="aee4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aee4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aee4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aee4b-127">Request body</span></span>
<span data-ttu-id="aee4b-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="aee4b-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

<span data-ttu-id="aee4b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="aee4b-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span></span>

|<span data-ttu-id="aee4b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aee4b-130">Property</span></span>|<span data-ttu-id="aee4b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aee4b-131">Type</span></span>|<span data-ttu-id="aee4b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aee4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aee4b-133">id</span><span class="sxs-lookup"><span data-stu-id="aee4b-133">id</span></span>|<span data-ttu-id="aee4b-134">String</span><span class="sxs-lookup"><span data-stu-id="aee4b-134">String</span></span>|<span data-ttu-id="aee4b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aee4b-135">Key of the entity.</span></span>|
|<span data-ttu-id="aee4b-136">destino</span><span class="sxs-lookup"><span data-stu-id="aee4b-136">target</span></span>|[<span data-ttu-id="aee4b-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="aee4b-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="aee4b-138">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="aee4b-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="aee4b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="aee4b-139">Response</span></span>
<span data-ttu-id="aee4b-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aee4b-140">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aee4b-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aee4b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="aee4b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aee4b-142">Request</span></span>
<span data-ttu-id="aee4b-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aee4b-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
Content-type: application/json
Content-length: 368

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="aee4b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="aee4b-144">Response</span></span>
<span data-ttu-id="aee4b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aee4b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 417

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



