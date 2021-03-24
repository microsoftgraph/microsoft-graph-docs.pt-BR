---
title: Atualizar windowsDefenderApplicationControlSupplementalPolicyAssignment
description: Atualize as propriedades de um objeto windowsDefenderApplicationControlSupplementalPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f161877e4f4f78479be7cf5aac82ee0f74d340e4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133959"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="92636-103">Atualizar windowsDefenderApplicationControlSupplementalPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="92636-103">Update windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

<span data-ttu-id="92636-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92636-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92636-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92636-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92636-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92636-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92636-107">Atualize as propriedades de [um objeto windowsDefenderApplicationControlSupplementalPolicyAssignment.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="92636-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92636-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92636-108">Prerequisites</span></span>
<span data-ttu-id="92636-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92636-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92636-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92636-111">Permission type</span></span>|<span data-ttu-id="92636-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92636-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92636-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92636-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92636-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92636-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="92636-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92636-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92636-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92636-116">Not supported.</span></span>|
|<span data-ttu-id="92636-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92636-117">Application</span></span>|<span data-ttu-id="92636-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92636-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92636-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92636-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="92636-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92636-120">Request headers</span></span>
|<span data-ttu-id="92636-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92636-121">Header</span></span>|<span data-ttu-id="92636-122">Valor</span><span class="sxs-lookup"><span data-stu-id="92636-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92636-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92636-123">Authorization</span></span>|<span data-ttu-id="92636-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92636-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92636-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92636-125">Accept</span></span>|<span data-ttu-id="92636-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92636-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92636-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92636-127">Request body</span></span>
<span data-ttu-id="92636-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsDefenderApplicationControlSupplementalPolicyAssignment.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="92636-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

<span data-ttu-id="92636-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="92636-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span></span>

|<span data-ttu-id="92636-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92636-130">Property</span></span>|<span data-ttu-id="92636-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="92636-131">Type</span></span>|<span data-ttu-id="92636-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="92636-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92636-133">id</span><span class="sxs-lookup"><span data-stu-id="92636-133">id</span></span>|<span data-ttu-id="92636-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92636-134">String</span></span>|<span data-ttu-id="92636-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="92636-135">Key of the entity.</span></span>|
|<span data-ttu-id="92636-136">destino</span><span class="sxs-lookup"><span data-stu-id="92636-136">target</span></span>|[<span data-ttu-id="92636-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="92636-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="92636-138">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="92636-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="92636-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="92636-139">Response</span></span>
<span data-ttu-id="92636-140">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92636-140">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92636-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92636-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="92636-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92636-142">Request</span></span>
<span data-ttu-id="92636-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92636-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="92636-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="92636-144">Response</span></span>
<span data-ttu-id="92636-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92636-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




