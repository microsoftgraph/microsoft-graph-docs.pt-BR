---
title: Criar intuneBrandingProfileAssignment
description: Criar um novo objeto intuneBrandingProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 64aa7d8e1ca3a1ad33e69921a67258f820348704
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157740"
---
# <a name="create-intunebrandingprofileassignment"></a><span data-ttu-id="27065-103">Criar intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="27065-103">Create intuneBrandingProfileAssignment</span></span>

<span data-ttu-id="27065-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27065-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27065-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27065-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27065-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27065-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27065-107">Criar um novo [objeto intuneBrandingProfileAssignment.](../resources/intune-wip-intunebrandingprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="27065-107">Create a new [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27065-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27065-108">Prerequisites</span></span>
<span data-ttu-id="27065-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27065-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27065-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27065-111">Permission type</span></span>|<span data-ttu-id="27065-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27065-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27065-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27065-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27065-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27065-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="27065-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27065-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27065-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27065-116">Not supported.</span></span>|
|<span data-ttu-id="27065-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27065-117">Application</span></span>|<span data-ttu-id="27065-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27065-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27065-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27065-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="27065-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27065-120">Request headers</span></span>
|<span data-ttu-id="27065-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27065-121">Header</span></span>|<span data-ttu-id="27065-122">Valor</span><span class="sxs-lookup"><span data-stu-id="27065-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27065-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="27065-123">Authorization</span></span>|<span data-ttu-id="27065-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27065-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27065-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27065-125">Accept</span></span>|<span data-ttu-id="27065-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27065-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27065-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27065-127">Request body</span></span>
<span data-ttu-id="27065-128">No corpo da solicitação, fornece uma representação JSON do objeto intuneBrandingProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="27065-128">In the request body, supply a JSON representation for the intuneBrandingProfileAssignment object.</span></span>

<span data-ttu-id="27065-129">A tabela a seguir mostra as propriedades que são necessárias ao criar intuneBrandingProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="27065-129">The following table shows the properties that are required when you create the intuneBrandingProfileAssignment.</span></span>

|<span data-ttu-id="27065-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27065-130">Property</span></span>|<span data-ttu-id="27065-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="27065-131">Type</span></span>|<span data-ttu-id="27065-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="27065-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27065-133">id</span><span class="sxs-lookup"><span data-stu-id="27065-133">id</span></span>|<span data-ttu-id="27065-134">String</span><span class="sxs-lookup"><span data-stu-id="27065-134">String</span></span>|<span data-ttu-id="27065-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="27065-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="27065-136">destino</span><span class="sxs-lookup"><span data-stu-id="27065-136">target</span></span>|[<span data-ttu-id="27065-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="27065-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="27065-138">Destino de atribuição ao que o perfil de identidade visual está atribuído.</span><span class="sxs-lookup"><span data-stu-id="27065-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="27065-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="27065-139">Response</span></span>
<span data-ttu-id="27065-140">Se bem-sucedido, este método retorna um código de resposta e um objeto `201 Created` [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27065-140">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27065-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27065-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="27065-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27065-142">Request</span></span>
<span data-ttu-id="27065-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27065-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
Content-type: application/json
Content-length: 390

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="27065-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="27065-144">Response</span></span>
<span data-ttu-id="27065-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27065-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




