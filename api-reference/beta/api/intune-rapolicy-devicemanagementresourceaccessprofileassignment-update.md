---
title: Atualizar deviceManagementResourceAccessProfileAssignment
description: Atualize as propriedades de um objeto deviceManagementResourceAccessProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efb68d34ac084ca4e4ebdfd03eee793eb5a85c4a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152100"
---
# <a name="update-devicemanagementresourceaccessprofileassignment"></a><span data-ttu-id="ed253-103">Atualizar deviceManagementResourceAccessProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="ed253-103">Update deviceManagementResourceAccessProfileAssignment</span></span>

<span data-ttu-id="ed253-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed253-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed253-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed253-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed253-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed253-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed253-107">Atualize as propriedades de [um objeto deviceManagementResourceAccessProfileAssignment.](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ed253-107">Update the properties of a [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed253-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed253-108">Prerequisites</span></span>
<span data-ttu-id="ed253-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed253-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed253-111">Permission type</span></span>|<span data-ttu-id="ed253-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed253-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed253-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed253-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed253-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed253-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ed253-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed253-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed253-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed253-116">Not supported.</span></span>|
|<span data-ttu-id="ed253-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed253-117">Application</span></span>|<span data-ttu-id="ed253-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed253-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed253-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed253-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments/{deviceManagementResourceAccessProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ed253-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed253-120">Request headers</span></span>
|<span data-ttu-id="ed253-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed253-121">Header</span></span>|<span data-ttu-id="ed253-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ed253-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed253-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed253-123">Authorization</span></span>|<span data-ttu-id="ed253-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed253-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed253-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed253-125">Accept</span></span>|<span data-ttu-id="ed253-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed253-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed253-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed253-127">Request body</span></span>
<span data-ttu-id="ed253-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementResourceAccessProfileAssignment.](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ed253-128">In the request body, supply a JSON representation for the [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.</span></span>

<span data-ttu-id="ed253-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ed253-129">The following table shows the properties that are required when you create the [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md).</span></span>

|<span data-ttu-id="ed253-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed253-130">Property</span></span>|<span data-ttu-id="ed253-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed253-131">Type</span></span>|<span data-ttu-id="ed253-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed253-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed253-133">id</span><span class="sxs-lookup"><span data-stu-id="ed253-133">id</span></span>|<span data-ttu-id="ed253-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed253-134">String</span></span>|<span data-ttu-id="ed253-135">Identificador exclusivo para as atribuições</span><span class="sxs-lookup"><span data-stu-id="ed253-135">Unique identifier for the Assignments</span></span>|
|<span data-ttu-id="ed253-136">finalidade</span><span class="sxs-lookup"><span data-stu-id="ed253-136">intent</span></span>|[<span data-ttu-id="ed253-137">deviceManagementResourceAccessProfileIntent</span><span class="sxs-lookup"><span data-stu-id="ed253-137">deviceManagementResourceAccessProfileIntent</span></span>](../resources/intune-rapolicy-devicemanagementresourceaccessprofileintent.md)|<span data-ttu-id="ed253-138">A intenção de atribuição para o perfil de acesso ao recurso.</span><span class="sxs-lookup"><span data-stu-id="ed253-138">The assignment intent for the resource access profile.</span></span> <span data-ttu-id="ed253-139">Os valores possíveis são: `apply` e `remove`.</span><span class="sxs-lookup"><span data-stu-id="ed253-139">Possible values are: `apply`, `remove`.</span></span>|
|<span data-ttu-id="ed253-140">destino</span><span class="sxs-lookup"><span data-stu-id="ed253-140">target</span></span>|[<span data-ttu-id="ed253-141">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ed253-141">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ed253-142">O destino de atribuição para o perfil de acesso ao recurso.</span><span class="sxs-lookup"><span data-stu-id="ed253-142">The assignment target for the resource access profile.</span></span>|
|<span data-ttu-id="ed253-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="ed253-143">sourceId</span></span>|<span data-ttu-id="ed253-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed253-144">String</span></span>|<span data-ttu-id="ed253-145">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="ed253-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="ed253-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed253-146">Response</span></span>
<span data-ttu-id="ed253-147">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed253-147">If successful, this method returns a `200 OK` response code and an updated [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed253-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed253-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed253-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed253-149">Request</span></span>
<span data-ttu-id="ed253-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed253-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments/{deviceManagementResourceAccessProfileAssignmentId}
Content-type: application/json
Content-length: 463

{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "intent": "remove",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="ed253-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed253-151">Response</span></span>
<span data-ttu-id="ed253-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed253-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "id": "4ebb8d4e-8d4e-4ebb-4e8d-bb4e4e8dbb4e",
  "intent": "remove",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "sourceId": "Source Id value"
}
```




