---
title: Atualizar windowsQualityUpdateProfileAssignment
description: Atualize as propriedades de um objeto windowsQualityUpdateProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76748ca5aa6c3192ebfe417746a6933928e45284
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156104"
---
# <a name="update-windowsqualityupdateprofileassignment"></a><span data-ttu-id="8c251-103">Atualizar windowsQualityUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="8c251-103">Update windowsQualityUpdateProfileAssignment</span></span>

<span data-ttu-id="8c251-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c251-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c251-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8c251-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c251-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c251-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c251-107">Atualize as propriedades de um [objeto windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8c251-107">Update the properties of a [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c251-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c251-108">Prerequisites</span></span>
<span data-ttu-id="8c251-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c251-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c251-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c251-111">Permission type</span></span>|<span data-ttu-id="8c251-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c251-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c251-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c251-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c251-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c251-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c251-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c251-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c251-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c251-116">Not supported.</span></span>|
|<span data-ttu-id="8c251-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c251-117">Application</span></span>|<span data-ttu-id="8c251-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c251-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c251-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c251-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}/assignments/{windowsQualityUpdateProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8c251-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c251-120">Request headers</span></span>
|<span data-ttu-id="8c251-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c251-121">Header</span></span>|<span data-ttu-id="8c251-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8c251-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c251-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c251-123">Authorization</span></span>|<span data-ttu-id="8c251-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c251-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c251-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8c251-125">Accept</span></span>|<span data-ttu-id="8c251-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c251-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c251-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c251-127">Request body</span></span>
<span data-ttu-id="8c251-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8c251-128">In the request body, supply a JSON representation for the [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) object.</span></span>

<span data-ttu-id="8c251-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8c251-129">The following table shows the properties that are required when you create the [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md).</span></span>

|<span data-ttu-id="8c251-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c251-130">Property</span></span>|<span data-ttu-id="8c251-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c251-131">Type</span></span>|<span data-ttu-id="8c251-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c251-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c251-133">id</span><span class="sxs-lookup"><span data-stu-id="8c251-133">id</span></span>|<span data-ttu-id="8c251-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c251-134">String</span></span>|<span data-ttu-id="8c251-135">O Identificador da entidade</span><span class="sxs-lookup"><span data-stu-id="8c251-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="8c251-136">destino</span><span class="sxs-lookup"><span data-stu-id="8c251-136">target</span></span>|[<span data-ttu-id="8c251-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8c251-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8c251-138">O destino de atribuição ao que o perfil de atualização de recursos é atribuído.</span><span class="sxs-lookup"><span data-stu-id="8c251-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="8c251-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c251-139">Response</span></span>
<span data-ttu-id="8c251-140">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c251-140">If successful, this method returns a `200 OK` response code and an updated [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c251-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c251-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c251-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c251-142">Request</span></span>
<span data-ttu-id="8c251-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c251-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}/assignments/{windowsQualityUpdateProfileAssignmentId}
Content-type: application/json
Content-length: 344

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="8c251-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c251-144">Response</span></span>
<span data-ttu-id="8c251-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c251-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 393

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "id": "0c3a8422-8422-0c3a-2284-3a0c22843a0c",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




