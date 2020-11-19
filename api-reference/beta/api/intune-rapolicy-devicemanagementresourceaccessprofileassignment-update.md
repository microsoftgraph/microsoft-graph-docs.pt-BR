---
title: Atualizar deviceManagementResourceAccessProfileAssignment
description: Atualiza as propriedades de um objeto deviceManagementResourceAccessProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32f2a64c0e6b4db08182919514bf5eb14755fd3e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301617"
---
# <a name="update-devicemanagementresourceaccessprofileassignment"></a><span data-ttu-id="7d0c1-103">Atualizar deviceManagementResourceAccessProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="7d0c1-103">Update deviceManagementResourceAccessProfileAssignment</span></span>

<span data-ttu-id="7d0c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d0c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d0c1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7d0c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d0c1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d0c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d0c1-107">Atualiza as propriedades de um objeto [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7d0c1-107">Update the properties of a [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d0c1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d0c1-108">Prerequisites</span></span>
<span data-ttu-id="7d0c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d0c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d0c1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d0c1-111">Permission type</span></span>|<span data-ttu-id="7d0c1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d0c1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d0c1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d0c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d0c1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d0c1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7d0c1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d0c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d0c1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d0c1-116">Not supported.</span></span>|
|<span data-ttu-id="7d0c1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d0c1-117">Application</span></span>|<span data-ttu-id="7d0c1-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d0c1-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d0c1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d0c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments/{deviceManagementResourceAccessProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7d0c1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d0c1-120">Request headers</span></span>
|<span data-ttu-id="7d0c1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d0c1-121">Header</span></span>|<span data-ttu-id="7d0c1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7d0c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d0c1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d0c1-123">Authorization</span></span>|<span data-ttu-id="7d0c1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d0c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d0c1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d0c1-125">Accept</span></span>|<span data-ttu-id="7d0c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d0c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d0c1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d0c1-127">Request body</span></span>
<span data-ttu-id="7d0c1-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7d0c1-128">In the request body, supply a JSON representation for the [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.</span></span>

<span data-ttu-id="7d0c1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7d0c1-129">The following table shows the properties that are required when you create the [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md).</span></span>

|<span data-ttu-id="7d0c1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d0c1-130">Property</span></span>|<span data-ttu-id="7d0c1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d0c1-131">Type</span></span>|<span data-ttu-id="7d0c1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d0c1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d0c1-133">id</span><span class="sxs-lookup"><span data-stu-id="7d0c1-133">id</span></span>|<span data-ttu-id="7d0c1-134">String</span><span class="sxs-lookup"><span data-stu-id="7d0c1-134">String</span></span>|<span data-ttu-id="7d0c1-135">Identificador exclusivo das atribuições</span><span class="sxs-lookup"><span data-stu-id="7d0c1-135">Unique identifier for the Assignments</span></span>|
|<span data-ttu-id="7d0c1-136">finalidade</span><span class="sxs-lookup"><span data-stu-id="7d0c1-136">intent</span></span>|[<span data-ttu-id="7d0c1-137">deviceManagementResourceAccessProfileIntent</span><span class="sxs-lookup"><span data-stu-id="7d0c1-137">deviceManagementResourceAccessProfileIntent</span></span>](../resources/intune-rapolicy-devicemanagementresourceaccessprofileintent.md)|<span data-ttu-id="7d0c1-138">A intenção de atribuição para o perfil de acesso do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d0c1-138">The assignment intent for the resource access profile.</span></span> <span data-ttu-id="7d0c1-139">Os valores possíveis são: `apply` e `remove`.</span><span class="sxs-lookup"><span data-stu-id="7d0c1-139">Possible values are: `apply`, `remove`.</span></span>|
|<span data-ttu-id="7d0c1-140">destino</span><span class="sxs-lookup"><span data-stu-id="7d0c1-140">target</span></span>|[<span data-ttu-id="7d0c1-141">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7d0c1-141">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7d0c1-142">O destino da atribuição para o perfil de acesso do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d0c1-142">The assignment target for the resource access profile.</span></span>|
|<span data-ttu-id="7d0c1-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="7d0c1-143">sourceId</span></span>|<span data-ttu-id="7d0c1-144">String</span><span class="sxs-lookup"><span data-stu-id="7d0c1-144">String</span></span>|<span data-ttu-id="7d0c1-145">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="7d0c1-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="7d0c1-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d0c1-146">Response</span></span>
<span data-ttu-id="7d0c1-147">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d0c1-147">If successful, this method returns a `200 OK` response code and an updated [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d0c1-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d0c1-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d0c1-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d0c1-149">Request</span></span>
<span data-ttu-id="7d0c1-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d0c1-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments/{deviceManagementResourceAccessProfileAssignmentId}
Content-type: application/json
Content-length: 399

{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "intent": "remove",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="7d0c1-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d0c1-151">Response</span></span>
<span data-ttu-id="7d0c1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d0c1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 448

{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "id": "4ebb8d4e-8d4e-4ebb-4e8d-bb4e4e8dbb4e",
  "intent": "remove",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "sourceId": "Source Id value"
}
```




