---
title: Atualizar windowsDefenderApplicationControlSupplementalPolicyAssignment
description: Atualiza as propriedades de um objeto windowsDefenderApplicationControlSupplementalPolicyAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 31191b31a0717896263192ba85ec778f3d5a94d7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799798"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="fb020-103">Atualizar windowsDefenderApplicationControlSupplementalPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="fb020-103">Update windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

> <span data-ttu-id="fb020-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb020-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb020-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb020-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb020-106">Atualiza as propriedades de um objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="fb020-106">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb020-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb020-107">Prerequisites</span></span>
<span data-ttu-id="fb020-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb020-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb020-110">Permission type</span></span>|<span data-ttu-id="fb020-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb020-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb020-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb020-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb020-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb020-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fb020-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb020-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb020-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb020-115">Not supported.</span></span>|
|<span data-ttu-id="fb020-116">Application</span><span class="sxs-lookup"><span data-stu-id="fb020-116">Application</span></span>|<span data-ttu-id="fb020-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb020-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb020-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb020-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="fb020-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb020-119">Request headers</span></span>
|<span data-ttu-id="fb020-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb020-120">Header</span></span>|<span data-ttu-id="fb020-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fb020-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb020-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb020-122">Authorization</span></span>|<span data-ttu-id="fb020-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb020-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb020-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb020-124">Accept</span></span>|<span data-ttu-id="fb020-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb020-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb020-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb020-126">Request body</span></span>
<span data-ttu-id="fb020-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="fb020-127">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

<span data-ttu-id="fb020-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fb020-128">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span></span>

|<span data-ttu-id="fb020-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb020-129">Property</span></span>|<span data-ttu-id="fb020-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb020-130">Type</span></span>|<span data-ttu-id="fb020-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb020-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb020-132">id</span><span class="sxs-lookup"><span data-stu-id="fb020-132">id</span></span>|<span data-ttu-id="fb020-133">String</span><span class="sxs-lookup"><span data-stu-id="fb020-133">String</span></span>|<span data-ttu-id="fb020-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fb020-134">Key of the entity.</span></span>|
|<span data-ttu-id="fb020-135">destino</span><span class="sxs-lookup"><span data-stu-id="fb020-135">target</span></span>|[<span data-ttu-id="fb020-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fb020-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fb020-137">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="fb020-137">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="fb020-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb020-138">Response</span></span>
<span data-ttu-id="fb020-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb020-139">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb020-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb020-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb020-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb020-141">Request</span></span>
<span data-ttu-id="fb020-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb020-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fb020-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb020-143">Response</span></span>
<span data-ttu-id="fb020-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb020-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




