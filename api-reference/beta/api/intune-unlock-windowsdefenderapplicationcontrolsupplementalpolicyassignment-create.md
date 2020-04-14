---
title: Criar windowsDefenderApplicationControlSupplementalPolicyAssignment
description: Criar um novo objeto windowsDefenderApplicationControlSupplementalPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 008bc6715ef60d21e468a8078d67076c91e66c6d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457232"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="02698-103">Criar windowsDefenderApplicationControlSupplementalPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="02698-103">Create windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

<span data-ttu-id="02698-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02698-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02698-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02698-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02698-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02698-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02698-107">Criar um novo objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="02698-107">Create a new [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02698-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02698-108">Prerequisites</span></span>
<span data-ttu-id="02698-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02698-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02698-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02698-111">Permission type</span></span>|<span data-ttu-id="02698-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02698-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02698-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02698-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02698-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02698-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="02698-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02698-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02698-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02698-116">Not supported.</span></span>|
|<span data-ttu-id="02698-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02698-117">Application</span></span>|<span data-ttu-id="02698-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02698-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02698-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02698-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="02698-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02698-120">Request headers</span></span>
|<span data-ttu-id="02698-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02698-121">Header</span></span>|<span data-ttu-id="02698-122">Valor</span><span class="sxs-lookup"><span data-stu-id="02698-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02698-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02698-123">Authorization</span></span>|<span data-ttu-id="02698-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02698-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02698-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02698-125">Accept</span></span>|<span data-ttu-id="02698-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02698-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02698-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02698-127">Request body</span></span>
<span data-ttu-id="02698-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderApplicationControlSupplementalPolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="02698-128">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicyAssignment object.</span></span>

<span data-ttu-id="02698-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderApplicationControlSupplementalPolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="02698-129">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicyAssignment.</span></span>

|<span data-ttu-id="02698-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02698-130">Property</span></span>|<span data-ttu-id="02698-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="02698-131">Type</span></span>|<span data-ttu-id="02698-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="02698-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02698-133">id</span><span class="sxs-lookup"><span data-stu-id="02698-133">id</span></span>|<span data-ttu-id="02698-134">String</span><span class="sxs-lookup"><span data-stu-id="02698-134">String</span></span>|<span data-ttu-id="02698-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="02698-135">Key of the entity.</span></span>|
|<span data-ttu-id="02698-136">destino</span><span class="sxs-lookup"><span data-stu-id="02698-136">target</span></span>|[<span data-ttu-id="02698-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="02698-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="02698-138">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="02698-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="02698-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="02698-139">Response</span></span>
<span data-ttu-id="02698-140">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02698-140">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02698-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02698-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="02698-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02698-142">Request</span></span>
<span data-ttu-id="02698-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02698-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments
Content-type: application/json
Content-length: 201

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="02698-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="02698-144">Response</span></span>
<span data-ttu-id="02698-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02698-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



