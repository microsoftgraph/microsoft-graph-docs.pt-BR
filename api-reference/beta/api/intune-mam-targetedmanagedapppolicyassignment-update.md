---
title: Atualizar targetedManagedAppPolicyAssignment
description: Atualizar as propriedades de um objeto targetedManagedAppPolicyAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 525bf6c1b8d07adbb2a25f7ec3273b3d05c2994a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803411"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="398ff-103">Atualizar targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="398ff-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="398ff-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="398ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="398ff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="398ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="398ff-106">Atualizar as propriedades de um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="398ff-106">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="398ff-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="398ff-107">Prerequisites</span></span>
<span data-ttu-id="398ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="398ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="398ff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="398ff-110">Permission type</span></span>|<span data-ttu-id="398ff-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="398ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="398ff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="398ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="398ff-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="398ff-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="398ff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="398ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="398ff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="398ff-115">Not supported.</span></span>|
|<span data-ttu-id="398ff-116">Application</span><span class="sxs-lookup"><span data-stu-id="398ff-116">Application</span></span>|<span data-ttu-id="398ff-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="398ff-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="398ff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="398ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="398ff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="398ff-119">Request headers</span></span>
|<span data-ttu-id="398ff-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="398ff-120">Header</span></span>|<span data-ttu-id="398ff-121">Valor</span><span class="sxs-lookup"><span data-stu-id="398ff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="398ff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="398ff-122">Authorization</span></span>|<span data-ttu-id="398ff-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="398ff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="398ff-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="398ff-124">Accept</span></span>|<span data-ttu-id="398ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="398ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="398ff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="398ff-126">Request body</span></span>
<span data-ttu-id="398ff-127">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="398ff-127">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="398ff-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="398ff-128">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="398ff-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="398ff-129">Property</span></span>|<span data-ttu-id="398ff-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="398ff-130">Type</span></span>|<span data-ttu-id="398ff-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="398ff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="398ff-132">id</span><span class="sxs-lookup"><span data-stu-id="398ff-132">id</span></span>|<span data-ttu-id="398ff-133">String</span><span class="sxs-lookup"><span data-stu-id="398ff-133">String</span></span>|<span data-ttu-id="398ff-134">Id</span><span class="sxs-lookup"><span data-stu-id="398ff-134">Id</span></span>|
|<span data-ttu-id="398ff-135">destino</span><span class="sxs-lookup"><span data-stu-id="398ff-135">target</span></span>|[<span data-ttu-id="398ff-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="398ff-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="398ff-137">Identificador para implantação em um grupo ou aplicativo</span><span class="sxs-lookup"><span data-stu-id="398ff-137">Identifier for deployment to a group or app</span></span>|
|<span data-ttu-id="398ff-138">source</span><span class="sxs-lookup"><span data-stu-id="398ff-138">source</span></span>|[<span data-ttu-id="398ff-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="398ff-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="398ff-140">Tipo de recurso usado para implantação em um grupo, direto ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="398ff-140">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="398ff-141">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="398ff-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="398ff-142">sourceId</span><span class="sxs-lookup"><span data-stu-id="398ff-142">sourceId</span></span>|<span data-ttu-id="398ff-143">String</span><span class="sxs-lookup"><span data-stu-id="398ff-143">String</span></span>|<span data-ttu-id="398ff-144">Identificador para o recurso usado para implantação em um grupo</span><span class="sxs-lookup"><span data-stu-id="398ff-144">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="398ff-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="398ff-145">Response</span></span>
<span data-ttu-id="398ff-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="398ff-146">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="398ff-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="398ff-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="398ff-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="398ff-148">Request</span></span>
<span data-ttu-id="398ff-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="398ff-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="398ff-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="398ff-150">Response</span></span>
<span data-ttu-id="398ff-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="398ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




