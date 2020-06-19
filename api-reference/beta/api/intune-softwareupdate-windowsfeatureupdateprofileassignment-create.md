---
title: Criar windowsFeatureUpdateProfileAssignment
description: Criar um novo objeto windowsFeatureUpdateProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 978a0e7b9c1c0b167bcf08c63d32fad8dc24b57c
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791297"
---
# <a name="create-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="41c0b-103">Criar windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="41c0b-103">Create windowsFeatureUpdateProfileAssignment</span></span>

<span data-ttu-id="41c0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41c0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41c0b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41c0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41c0b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41c0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41c0b-107">Criar um novo objeto [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="41c0b-107">Create a new [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41c0b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41c0b-108">Prerequisites</span></span>
<span data-ttu-id="41c0b-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="41c0b-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="41c0b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41c0b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41c0b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41c0b-111">Permission type</span></span>|<span data-ttu-id="41c0b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41c0b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41c0b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41c0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41c0b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41c0b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41c0b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41c0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41c0b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41c0b-116">Not supported.</span></span>|
|<span data-ttu-id="41c0b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41c0b-117">Application</span></span>|<span data-ttu-id="41c0b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41c0b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41c0b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41c0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="41c0b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41c0b-120">Request headers</span></span>
|<span data-ttu-id="41c0b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41c0b-121">Header</span></span>|<span data-ttu-id="41c0b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="41c0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41c0b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="41c0b-123">Authorization</span></span>|<span data-ttu-id="41c0b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41c0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41c0b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41c0b-125">Accept</span></span>|<span data-ttu-id="41c0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41c0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41c0b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41c0b-127">Request body</span></span>
<span data-ttu-id="41c0b-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsFeatureUpdateProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="41c0b-128">In the request body, supply a JSON representation for the windowsFeatureUpdateProfileAssignment object.</span></span>

<span data-ttu-id="41c0b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsFeatureUpdateProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="41c0b-129">The following table shows the properties that are required when you create the windowsFeatureUpdateProfileAssignment.</span></span>

|<span data-ttu-id="41c0b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41c0b-130">Property</span></span>|<span data-ttu-id="41c0b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="41c0b-131">Type</span></span>|<span data-ttu-id="41c0b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="41c0b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41c0b-133">id</span><span class="sxs-lookup"><span data-stu-id="41c0b-133">id</span></span>|<span data-ttu-id="41c0b-134">String</span><span class="sxs-lookup"><span data-stu-id="41c0b-134">String</span></span>|<span data-ttu-id="41c0b-135">O identificador da entidade</span><span class="sxs-lookup"><span data-stu-id="41c0b-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="41c0b-136">destino</span><span class="sxs-lookup"><span data-stu-id="41c0b-136">target</span></span>|[<span data-ttu-id="41c0b-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="41c0b-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="41c0b-138">O destino de atribuição ao qual o perfil de atualização de recursos está atribuído.</span><span class="sxs-lookup"><span data-stu-id="41c0b-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="41c0b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="41c0b-139">Response</span></span>
<span data-ttu-id="41c0b-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41c0b-140">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41c0b-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41c0b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="41c0b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41c0b-142">Request</span></span>
<span data-ttu-id="41c0b-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41c0b-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
Content-type: application/json
Content-length: 344

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="41c0b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="41c0b-144">Response</span></span>
<span data-ttu-id="41c0b-145">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="41c0b-145">Here is an example of the response.</span></span> <span data-ttu-id="41c0b-146">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="41c0b-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="41c0b-147">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="41c0b-147">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 393

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "id": "567a744f-744f-567a-4f74-7a564f747a56",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



