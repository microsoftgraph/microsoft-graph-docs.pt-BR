---
title: Criar windowsFeatureUpdateProfileAssignment
description: Criar um novo objeto windowsFeatureUpdateProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dc08579bd23a73d6786555943dd2167284b19427
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082319"
---
# <a name="create-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="a6ee3-103">Criar windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="a6ee3-103">Create windowsFeatureUpdateProfileAssignment</span></span>

<span data-ttu-id="a6ee3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6ee3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6ee3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6ee3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6ee3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6ee3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6ee3-107">Criar um novo objeto [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a6ee3-107">Create a new [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6ee3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6ee3-108">Prerequisites</span></span>
<span data-ttu-id="a6ee3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6ee3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6ee3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6ee3-111">Permission type</span></span>|<span data-ttu-id="a6ee3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6ee3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6ee3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6ee3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6ee3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6ee3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6ee3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6ee3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6ee3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6ee3-116">Not supported.</span></span>|
|<span data-ttu-id="a6ee3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6ee3-117">Application</span></span>|<span data-ttu-id="a6ee3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6ee3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6ee3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6ee3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a6ee3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ee3-120">Request headers</span></span>
|<span data-ttu-id="a6ee3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6ee3-121">Header</span></span>|<span data-ttu-id="a6ee3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a6ee3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6ee3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6ee3-123">Authorization</span></span>|<span data-ttu-id="a6ee3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6ee3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6ee3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6ee3-125">Accept</span></span>|<span data-ttu-id="a6ee3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6ee3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6ee3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ee3-127">Request body</span></span>
<span data-ttu-id="a6ee3-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsFeatureUpdateProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="a6ee3-128">In the request body, supply a JSON representation for the windowsFeatureUpdateProfileAssignment object.</span></span>

<span data-ttu-id="a6ee3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsFeatureUpdateProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="a6ee3-129">The following table shows the properties that are required when you create the windowsFeatureUpdateProfileAssignment.</span></span>

|<span data-ttu-id="a6ee3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6ee3-130">Property</span></span>|<span data-ttu-id="a6ee3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6ee3-131">Type</span></span>|<span data-ttu-id="a6ee3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6ee3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6ee3-133">id</span><span class="sxs-lookup"><span data-stu-id="a6ee3-133">id</span></span>|<span data-ttu-id="a6ee3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6ee3-134">String</span></span>|<span data-ttu-id="a6ee3-135">O identificador da entidade</span><span class="sxs-lookup"><span data-stu-id="a6ee3-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="a6ee3-136">destino</span><span class="sxs-lookup"><span data-stu-id="a6ee3-136">target</span></span>|[<span data-ttu-id="a6ee3-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a6ee3-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a6ee3-138">O destino de atribuição ao qual o perfil de atualização de recursos está atribuído.</span><span class="sxs-lookup"><span data-stu-id="a6ee3-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="a6ee3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6ee3-139">Response</span></span>
<span data-ttu-id="a6ee3-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6ee3-140">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6ee3-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6ee3-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6ee3-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ee3-142">Request</span></span>
<span data-ttu-id="a6ee3-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6ee3-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a6ee3-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6ee3-144">Response</span></span>
<span data-ttu-id="a6ee3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6ee3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






