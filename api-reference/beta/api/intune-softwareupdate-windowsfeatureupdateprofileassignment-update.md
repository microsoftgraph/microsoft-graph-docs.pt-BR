---
title: Atualizar windowsFeatureUpdateProfileAssignment
description: Atualize as propriedades de um objeto windowsFeatureUpdateProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d54fd27c2f106e72cfa9ab8a11a13715693190f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156321"
---
# <a name="update-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="4b386-103">Atualizar windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="4b386-103">Update windowsFeatureUpdateProfileAssignment</span></span>

<span data-ttu-id="4b386-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b386-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b386-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b386-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b386-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b386-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b386-107">Atualize as propriedades de um [objeto windowsFeatureUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4b386-107">Update the properties of a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b386-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b386-108">Prerequisites</span></span>
<span data-ttu-id="4b386-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b386-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b386-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b386-111">Permission type</span></span>|<span data-ttu-id="4b386-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b386-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b386-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b386-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b386-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b386-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b386-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b386-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b386-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b386-116">Not supported.</span></span>|
|<span data-ttu-id="4b386-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b386-117">Application</span></span>|<span data-ttu-id="4b386-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b386-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b386-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b386-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4b386-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b386-120">Request headers</span></span>
|<span data-ttu-id="4b386-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b386-121">Header</span></span>|<span data-ttu-id="4b386-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4b386-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b386-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b386-123">Authorization</span></span>|<span data-ttu-id="4b386-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b386-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b386-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b386-125">Accept</span></span>|<span data-ttu-id="4b386-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b386-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b386-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b386-127">Request body</span></span>
<span data-ttu-id="4b386-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsFeatureUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4b386-128">In the request body, supply a JSON representation for the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

<span data-ttu-id="4b386-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4b386-129">The following table shows the properties that are required when you create the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).</span></span>

|<span data-ttu-id="4b386-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b386-130">Property</span></span>|<span data-ttu-id="4b386-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b386-131">Type</span></span>|<span data-ttu-id="4b386-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b386-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b386-133">id</span><span class="sxs-lookup"><span data-stu-id="4b386-133">id</span></span>|<span data-ttu-id="4b386-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b386-134">String</span></span>|<span data-ttu-id="4b386-135">O Identificador da entidade</span><span class="sxs-lookup"><span data-stu-id="4b386-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="4b386-136">destino</span><span class="sxs-lookup"><span data-stu-id="4b386-136">target</span></span>|[<span data-ttu-id="4b386-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4b386-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4b386-138">O destino de atribuição ao que o perfil de atualização de recursos é atribuído.</span><span class="sxs-lookup"><span data-stu-id="4b386-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="4b386-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b386-139">Response</span></span>
<span data-ttu-id="4b386-140">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b386-140">If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b386-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b386-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b386-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b386-142">Request</span></span>
<span data-ttu-id="4b386-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b386-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
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

### <a name="response"></a><span data-ttu-id="4b386-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b386-144">Response</span></span>
<span data-ttu-id="4b386-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b386-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




