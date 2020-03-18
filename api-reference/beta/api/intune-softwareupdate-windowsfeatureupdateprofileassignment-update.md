---
title: Atualizar windowsFeatureUpdateProfileAssignment
description: Atualiza as propriedades de um objeto windowsFeatureUpdateProfileAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 35973927b9eadacc8b9fd4280c33b789c6584a03
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800337"
---
# <a name="update-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="1ca09-103">Atualizar windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="1ca09-103">Update windowsFeatureUpdateProfileAssignment</span></span>

> <span data-ttu-id="1ca09-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ca09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ca09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ca09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ca09-106">Atualiza as propriedades de um objeto [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1ca09-106">Update the properties of a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ca09-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ca09-107">Prerequisites</span></span>
<span data-ttu-id="1ca09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ca09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ca09-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ca09-110">Permission type</span></span>|<span data-ttu-id="1ca09-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ca09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ca09-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ca09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ca09-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ca09-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ca09-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ca09-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ca09-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ca09-115">Not supported.</span></span>|
|<span data-ttu-id="1ca09-116">Application</span><span class="sxs-lookup"><span data-stu-id="1ca09-116">Application</span></span>|<span data-ttu-id="1ca09-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ca09-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ca09-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ca09-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1ca09-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ca09-119">Request headers</span></span>
|<span data-ttu-id="1ca09-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ca09-120">Header</span></span>|<span data-ttu-id="1ca09-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1ca09-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ca09-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ca09-122">Authorization</span></span>|<span data-ttu-id="1ca09-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ca09-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ca09-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ca09-124">Accept</span></span>|<span data-ttu-id="1ca09-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ca09-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ca09-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ca09-126">Request body</span></span>
<span data-ttu-id="1ca09-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1ca09-127">In the request body, supply a JSON representation for the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

<span data-ttu-id="1ca09-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1ca09-128">The following table shows the properties that are required when you create the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).</span></span>

|<span data-ttu-id="1ca09-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ca09-129">Property</span></span>|<span data-ttu-id="1ca09-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ca09-130">Type</span></span>|<span data-ttu-id="1ca09-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ca09-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ca09-132">id</span><span class="sxs-lookup"><span data-stu-id="1ca09-132">id</span></span>|<span data-ttu-id="1ca09-133">String</span><span class="sxs-lookup"><span data-stu-id="1ca09-133">String</span></span>|<span data-ttu-id="1ca09-134">O identificador da entidade</span><span class="sxs-lookup"><span data-stu-id="1ca09-134">The Identifier of the entity</span></span>|
|<span data-ttu-id="1ca09-135">destino</span><span class="sxs-lookup"><span data-stu-id="1ca09-135">target</span></span>|[<span data-ttu-id="1ca09-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1ca09-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1ca09-137">O destino de atribuição ao qual o perfil de atualização de recursos está atribuído.</span><span class="sxs-lookup"><span data-stu-id="1ca09-137">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="1ca09-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ca09-138">Response</span></span>
<span data-ttu-id="1ca09-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ca09-139">If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ca09-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ca09-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ca09-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ca09-141">Request</span></span>
<span data-ttu-id="1ca09-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ca09-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1ca09-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ca09-143">Response</span></span>
<span data-ttu-id="1ca09-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ca09-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




