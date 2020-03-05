---
title: Atualizar targetedManagedAppPolicyAssignment
description: Atualizar as propriedades de um objeto targetedManagedAppPolicyAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b3b0db1368b8726deaa7ff3adcacee0774eebfce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463150"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="31f3f-103">Atualizar targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="31f3f-103">Update targetedManagedAppPolicyAssignment</span></span>

<span data-ttu-id="31f3f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="31f3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31f3f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31f3f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31f3f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31f3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31f3f-107">Atualizar as propriedades de um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31f3f-107">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31f3f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="31f3f-108">Prerequisites</span></span>
<span data-ttu-id="31f3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31f3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31f3f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31f3f-111">Permission type</span></span>|<span data-ttu-id="31f3f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="31f3f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31f3f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31f3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31f3f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31f3f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="31f3f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31f3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31f3f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31f3f-116">Not supported.</span></span>|
|<span data-ttu-id="31f3f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31f3f-117">Application</span></span>|<span data-ttu-id="31f3f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31f3f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31f3f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31f3f-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="31f3f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31f3f-120">Request headers</span></span>
|<span data-ttu-id="31f3f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31f3f-121">Header</span></span>|<span data-ttu-id="31f3f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="31f3f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31f3f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="31f3f-123">Authorization</span></span>|<span data-ttu-id="31f3f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31f3f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31f3f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="31f3f-125">Accept</span></span>|<span data-ttu-id="31f3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31f3f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31f3f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31f3f-127">Request body</span></span>
<span data-ttu-id="31f3f-128">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31f3f-128">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="31f3f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31f3f-129">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="31f3f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31f3f-130">Property</span></span>|<span data-ttu-id="31f3f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="31f3f-131">Type</span></span>|<span data-ttu-id="31f3f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="31f3f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31f3f-133">id</span><span class="sxs-lookup"><span data-stu-id="31f3f-133">id</span></span>|<span data-ttu-id="31f3f-134">String</span><span class="sxs-lookup"><span data-stu-id="31f3f-134">String</span></span>|<span data-ttu-id="31f3f-135">Id</span><span class="sxs-lookup"><span data-stu-id="31f3f-135">Id</span></span>|
|<span data-ttu-id="31f3f-136">destino</span><span class="sxs-lookup"><span data-stu-id="31f3f-136">target</span></span>|[<span data-ttu-id="31f3f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="31f3f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="31f3f-138">Identificador para implantação em um grupo ou aplicativo</span><span class="sxs-lookup"><span data-stu-id="31f3f-138">Identifier for deployment to a group or app</span></span>|
|<span data-ttu-id="31f3f-139">source</span><span class="sxs-lookup"><span data-stu-id="31f3f-139">source</span></span>|[<span data-ttu-id="31f3f-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="31f3f-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="31f3f-141">Tipo de recurso usado para implantação em um grupo, direto ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="31f3f-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="31f3f-142">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="31f3f-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="31f3f-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="31f3f-143">sourceId</span></span>|<span data-ttu-id="31f3f-144">String</span><span class="sxs-lookup"><span data-stu-id="31f3f-144">String</span></span>|<span data-ttu-id="31f3f-145">Identificador para o recurso usado para implantação em um grupo</span><span class="sxs-lookup"><span data-stu-id="31f3f-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="31f3f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="31f3f-146">Response</span></span>
<span data-ttu-id="31f3f-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31f3f-147">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31f3f-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31f3f-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="31f3f-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31f3f-149">Request</span></span>
<span data-ttu-id="31f3f-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31f3f-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="31f3f-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="31f3f-151">Response</span></span>
<span data-ttu-id="31f3f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31f3f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





