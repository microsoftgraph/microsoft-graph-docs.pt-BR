---
title: Atualizar intuneBrandingProfileAssignment
description: Atualiza as propriedades de um objeto intuneBrandingProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 718a2e538b619a4138ef64987009bd5f6415851a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791206"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="77823-103">Atualizar intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="77823-103">Update intuneBrandingProfileAssignment</span></span>

<span data-ttu-id="77823-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77823-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77823-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="77823-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77823-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77823-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77823-107">Atualiza as propriedades de um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="77823-107">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77823-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77823-108">Prerequisites</span></span>
<span data-ttu-id="77823-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="77823-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="77823-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77823-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77823-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77823-111">Permission type</span></span>|<span data-ttu-id="77823-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="77823-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77823-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77823-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77823-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77823-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="77823-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77823-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77823-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77823-116">Not supported.</span></span>|
|<span data-ttu-id="77823-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77823-117">Application</span></span>|<span data-ttu-id="77823-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77823-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77823-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77823-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="77823-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77823-120">Request headers</span></span>
|<span data-ttu-id="77823-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77823-121">Header</span></span>|<span data-ttu-id="77823-122">Valor</span><span class="sxs-lookup"><span data-stu-id="77823-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77823-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="77823-123">Authorization</span></span>|<span data-ttu-id="77823-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77823-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77823-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="77823-125">Accept</span></span>|<span data-ttu-id="77823-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77823-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77823-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77823-127">Request body</span></span>
<span data-ttu-id="77823-128">No corpo da solicitação, forneça uma representação JSON do objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="77823-128">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="77823-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="77823-129">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="77823-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77823-130">Property</span></span>|<span data-ttu-id="77823-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="77823-131">Type</span></span>|<span data-ttu-id="77823-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="77823-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77823-133">id</span><span class="sxs-lookup"><span data-stu-id="77823-133">id</span></span>|<span data-ttu-id="77823-134">String</span><span class="sxs-lookup"><span data-stu-id="77823-134">String</span></span>|<span data-ttu-id="77823-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="77823-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="77823-136">destino</span><span class="sxs-lookup"><span data-stu-id="77823-136">target</span></span>|[<span data-ttu-id="77823-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="77823-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="77823-138">Destino de atribuição ao qual o perfil de identidade visual está atribuído.</span><span class="sxs-lookup"><span data-stu-id="77823-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="77823-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="77823-139">Response</span></span>
<span data-ttu-id="77823-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77823-140">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77823-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77823-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="77823-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77823-142">Request</span></span>
<span data-ttu-id="77823-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77823-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
Content-type: application/json
Content-length: 326

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="77823-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="77823-144">Response</span></span>
<span data-ttu-id="77823-145">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="77823-145">Here is an example of the response.</span></span> <span data-ttu-id="77823-146">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="77823-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="77823-147">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="77823-147">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 375

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



