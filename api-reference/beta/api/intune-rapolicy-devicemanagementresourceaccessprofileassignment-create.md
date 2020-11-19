---
title: Criar deviceManagementResourceAccessProfileAssignment
description: Criar um novo objeto deviceManagementResourceAccessProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1053da56d274206d7f050797350d8948d55fa7b3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301423"
---
# <a name="create-devicemanagementresourceaccessprofileassignment"></a><span data-ttu-id="04add-103">Criar deviceManagementResourceAccessProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="04add-103">Create deviceManagementResourceAccessProfileAssignment</span></span>

<span data-ttu-id="04add-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04add-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04add-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04add-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04add-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04add-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04add-107">Criar um novo objeto [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="04add-107">Create a new [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04add-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04add-108">Prerequisites</span></span>
<span data-ttu-id="04add-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04add-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04add-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04add-111">Permission type</span></span>|<span data-ttu-id="04add-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04add-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04add-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04add-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04add-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04add-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="04add-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04add-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04add-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04add-116">Not supported.</span></span>|
|<span data-ttu-id="04add-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04add-117">Application</span></span>|<span data-ttu-id="04add-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04add-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04add-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04add-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="04add-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04add-120">Request headers</span></span>
|<span data-ttu-id="04add-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04add-121">Header</span></span>|<span data-ttu-id="04add-122">Valor</span><span class="sxs-lookup"><span data-stu-id="04add-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04add-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="04add-123">Authorization</span></span>|<span data-ttu-id="04add-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04add-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04add-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04add-125">Accept</span></span>|<span data-ttu-id="04add-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04add-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04add-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04add-127">Request body</span></span>
<span data-ttu-id="04add-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementResourceAccessProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="04add-128">In the request body, supply a JSON representation for the deviceManagementResourceAccessProfileAssignment object.</span></span>

<span data-ttu-id="04add-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementResourceAccessProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="04add-129">The following table shows the properties that are required when you create the deviceManagementResourceAccessProfileAssignment.</span></span>

|<span data-ttu-id="04add-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04add-130">Property</span></span>|<span data-ttu-id="04add-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="04add-131">Type</span></span>|<span data-ttu-id="04add-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="04add-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04add-133">id</span><span class="sxs-lookup"><span data-stu-id="04add-133">id</span></span>|<span data-ttu-id="04add-134">String</span><span class="sxs-lookup"><span data-stu-id="04add-134">String</span></span>|<span data-ttu-id="04add-135">Identificador exclusivo das atribuições</span><span class="sxs-lookup"><span data-stu-id="04add-135">Unique identifier for the Assignments</span></span>|
|<span data-ttu-id="04add-136">finalidade</span><span class="sxs-lookup"><span data-stu-id="04add-136">intent</span></span>|[<span data-ttu-id="04add-137">deviceManagementResourceAccessProfileIntent</span><span class="sxs-lookup"><span data-stu-id="04add-137">deviceManagementResourceAccessProfileIntent</span></span>](../resources/intune-rapolicy-devicemanagementresourceaccessprofileintent.md)|<span data-ttu-id="04add-138">A intenção de atribuição para o perfil de acesso do recurso.</span><span class="sxs-lookup"><span data-stu-id="04add-138">The assignment intent for the resource access profile.</span></span> <span data-ttu-id="04add-139">Os valores possíveis são: `apply` e `remove`.</span><span class="sxs-lookup"><span data-stu-id="04add-139">Possible values are: `apply`, `remove`.</span></span>|
|<span data-ttu-id="04add-140">destino</span><span class="sxs-lookup"><span data-stu-id="04add-140">target</span></span>|[<span data-ttu-id="04add-141">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="04add-141">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="04add-142">O destino da atribuição para o perfil de acesso do recurso.</span><span class="sxs-lookup"><span data-stu-id="04add-142">The assignment target for the resource access profile.</span></span>|
|<span data-ttu-id="04add-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="04add-143">sourceId</span></span>|<span data-ttu-id="04add-144">String</span><span class="sxs-lookup"><span data-stu-id="04add-144">String</span></span>|<span data-ttu-id="04add-145">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="04add-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="04add-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="04add-146">Response</span></span>
<span data-ttu-id="04add-147">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04add-147">If successful, this method returns a `201 Created` response code and a [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04add-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04add-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="04add-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04add-149">Request</span></span>
<span data-ttu-id="04add-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04add-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments
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

### <a name="response"></a><span data-ttu-id="04add-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="04add-151">Response</span></span>
<span data-ttu-id="04add-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04add-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




