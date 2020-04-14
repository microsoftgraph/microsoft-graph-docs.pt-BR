---
title: Atualizar windowsFeatureUpdateProfileAssignment
description: Atualiza as propriedades de um objeto windowsFeatureUpdateProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3b808fea3a16da8d02d8e7cb54dae112c1aef09c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457574"
---
# <a name="update-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="90756-103">Atualizar windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="90756-103">Update windowsFeatureUpdateProfileAssignment</span></span>

<span data-ttu-id="90756-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90756-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90756-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="90756-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90756-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90756-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90756-107">Atualiza as propriedades de um objeto [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="90756-107">Update the properties of a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90756-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90756-108">Prerequisites</span></span>
<span data-ttu-id="90756-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90756-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90756-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90756-111">Permission type</span></span>|<span data-ttu-id="90756-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90756-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90756-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90756-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90756-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90756-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90756-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90756-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90756-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90756-116">Not supported.</span></span>|
|<span data-ttu-id="90756-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90756-117">Application</span></span>|<span data-ttu-id="90756-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90756-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90756-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90756-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="90756-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90756-120">Request headers</span></span>
|<span data-ttu-id="90756-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90756-121">Header</span></span>|<span data-ttu-id="90756-122">Valor</span><span class="sxs-lookup"><span data-stu-id="90756-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90756-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="90756-123">Authorization</span></span>|<span data-ttu-id="90756-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90756-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90756-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90756-125">Accept</span></span>|<span data-ttu-id="90756-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90756-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90756-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90756-127">Request body</span></span>
<span data-ttu-id="90756-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="90756-128">In the request body, supply a JSON representation for the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

<span data-ttu-id="90756-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="90756-129">The following table shows the properties that are required when you create the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).</span></span>

|<span data-ttu-id="90756-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90756-130">Property</span></span>|<span data-ttu-id="90756-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="90756-131">Type</span></span>|<span data-ttu-id="90756-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="90756-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90756-133">id</span><span class="sxs-lookup"><span data-stu-id="90756-133">id</span></span>|<span data-ttu-id="90756-134">String</span><span class="sxs-lookup"><span data-stu-id="90756-134">String</span></span>|<span data-ttu-id="90756-135">O identificador da entidade</span><span class="sxs-lookup"><span data-stu-id="90756-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="90756-136">destino</span><span class="sxs-lookup"><span data-stu-id="90756-136">target</span></span>|[<span data-ttu-id="90756-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="90756-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="90756-138">O destino de atribuição ao qual o perfil de atualização de recursos está atribuído.</span><span class="sxs-lookup"><span data-stu-id="90756-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="90756-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="90756-139">Response</span></span>
<span data-ttu-id="90756-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90756-140">If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90756-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90756-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="90756-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90756-142">Request</span></span>
<span data-ttu-id="90756-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90756-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
Content-type: application/json
Content-length: 177

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="90756-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="90756-144">Response</span></span>
<span data-ttu-id="90756-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90756-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 226

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "id": "567a744f-744f-567a-4f74-7a564f747a56",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



