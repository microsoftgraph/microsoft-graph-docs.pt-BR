---
title: Atualizar targetedManagedAppPolicyAssignment
description: Atualizar as propriedades de um objeto targetedManagedAppPolicyAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: adcc1fc1fa088e3a9517302f0efe342a7b53da1e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942223"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="1aada-103">Atualizar targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="1aada-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="1aada-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1aada-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1aada-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1aada-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1aada-106">Atualizar as propriedades de um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1aada-106">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1aada-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1aada-107">Prerequisites</span></span>
<span data-ttu-id="1aada-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1aada-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1aada-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1aada-110">Permission type</span></span>|<span data-ttu-id="1aada-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1aada-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1aada-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1aada-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1aada-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aada-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1aada-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1aada-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1aada-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1aada-115">Not supported.</span></span>|
|<span data-ttu-id="1aada-116">Application</span><span class="sxs-lookup"><span data-stu-id="1aada-116">Application</span></span>|<span data-ttu-id="1aada-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aada-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1aada-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1aada-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1aada-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1aada-119">Request headers</span></span>
|<span data-ttu-id="1aada-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1aada-120">Header</span></span>|<span data-ttu-id="1aada-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1aada-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1aada-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1aada-122">Authorization</span></span>|<span data-ttu-id="1aada-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1aada-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1aada-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1aada-124">Accept</span></span>|<span data-ttu-id="1aada-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1aada-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1aada-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1aada-126">Request body</span></span>
<span data-ttu-id="1aada-127">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1aada-127">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="1aada-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1aada-128">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="1aada-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1aada-129">Property</span></span>|<span data-ttu-id="1aada-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1aada-130">Type</span></span>|<span data-ttu-id="1aada-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1aada-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aada-132">id</span><span class="sxs-lookup"><span data-stu-id="1aada-132">id</span></span>|<span data-ttu-id="1aada-133">String</span><span class="sxs-lookup"><span data-stu-id="1aada-133">String</span></span>|<span data-ttu-id="1aada-134">Id</span><span class="sxs-lookup"><span data-stu-id="1aada-134">Id</span></span>|
|<span data-ttu-id="1aada-135">destino</span><span class="sxs-lookup"><span data-stu-id="1aada-135">target</span></span>|[<span data-ttu-id="1aada-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1aada-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1aada-137">Identificador para implantação em um grupo ou aplicativo</span><span class="sxs-lookup"><span data-stu-id="1aada-137">Identifier for deployment to a group or app</span></span>|
|<span data-ttu-id="1aada-138">source</span><span class="sxs-lookup"><span data-stu-id="1aada-138">source</span></span>|[<span data-ttu-id="1aada-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="1aada-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="1aada-140">Tipo de recurso usado para implantação em um grupo, direto ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="1aada-140">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="1aada-141">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="1aada-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="1aada-142">sourceId</span><span class="sxs-lookup"><span data-stu-id="1aada-142">sourceId</span></span>|<span data-ttu-id="1aada-143">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="1aada-143">String</span></span>|<span data-ttu-id="1aada-144">Identificador para o recurso usado para implantação em um grupo</span><span class="sxs-lookup"><span data-stu-id="1aada-144">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="1aada-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1aada-145">Response</span></span>
<span data-ttu-id="1aada-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1aada-146">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1aada-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1aada-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="1aada-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1aada-148">Request</span></span>
<span data-ttu-id="1aada-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1aada-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1aada-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="1aada-150">Response</span></span>
<span data-ttu-id="1aada-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1aada-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





