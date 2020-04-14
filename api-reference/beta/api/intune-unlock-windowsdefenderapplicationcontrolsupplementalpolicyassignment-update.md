---
title: Atualizar windowsDefenderApplicationControlSupplementalPolicyAssignment
description: Atualiza as propriedades de um objeto windowsDefenderApplicationControlSupplementalPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 923d4dd424b25a58380af2f369c0b79d2b524727
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450177"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="cdc3d-103">Atualizar windowsDefenderApplicationControlSupplementalPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="cdc3d-103">Update windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

<span data-ttu-id="cdc3d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdc3d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdc3d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cdc3d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdc3d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cdc3d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdc3d-107">Atualiza as propriedades de um objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="cdc3d-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdc3d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cdc3d-108">Prerequisites</span></span>
<span data-ttu-id="cdc3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdc3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdc3d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdc3d-111">Permission type</span></span>|<span data-ttu-id="cdc3d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cdc3d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdc3d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdc3d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cdc3d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdc3d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cdc3d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdc3d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdc3d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdc3d-116">Not supported.</span></span>|
|<span data-ttu-id="cdc3d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdc3d-117">Application</span></span>|<span data-ttu-id="cdc3d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdc3d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdc3d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc3d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="cdc3d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc3d-120">Request headers</span></span>
|<span data-ttu-id="cdc3d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cdc3d-121">Header</span></span>|<span data-ttu-id="cdc3d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cdc3d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdc3d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdc3d-123">Authorization</span></span>|<span data-ttu-id="cdc3d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdc3d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdc3d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cdc3d-125">Accept</span></span>|<span data-ttu-id="cdc3d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cdc3d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdc3d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc3d-127">Request body</span></span>
<span data-ttu-id="cdc3d-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="cdc3d-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

<span data-ttu-id="cdc3d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cdc3d-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span></span>

|<span data-ttu-id="cdc3d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cdc3d-130">Property</span></span>|<span data-ttu-id="cdc3d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdc3d-131">Type</span></span>|<span data-ttu-id="cdc3d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdc3d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdc3d-133">id</span><span class="sxs-lookup"><span data-stu-id="cdc3d-133">id</span></span>|<span data-ttu-id="cdc3d-134">String</span><span class="sxs-lookup"><span data-stu-id="cdc3d-134">String</span></span>|<span data-ttu-id="cdc3d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cdc3d-135">Key of the entity.</span></span>|
|<span data-ttu-id="cdc3d-136">destino</span><span class="sxs-lookup"><span data-stu-id="cdc3d-136">target</span></span>|[<span data-ttu-id="cdc3d-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cdc3d-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cdc3d-138">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="cdc3d-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="cdc3d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdc3d-139">Response</span></span>
<span data-ttu-id="cdc3d-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdc3d-140">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdc3d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdc3d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdc3d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc3d-142">Request</span></span>
<span data-ttu-id="cdc3d-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdc3d-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
Content-type: application/json
Content-length: 201

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="cdc3d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdc3d-144">Response</span></span>
<span data-ttu-id="cdc3d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cdc3d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



