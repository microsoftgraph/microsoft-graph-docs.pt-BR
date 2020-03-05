---
title: Atualizar intuneBrandingProfileAssignment
description: Atualiza as propriedades de um objeto intuneBrandingProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 149b212a8e859671bcf6dc4f50615b31408a704e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457388"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="2f9ee-103">Atualizar intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="2f9ee-103">Update intuneBrandingProfileAssignment</span></span>

<span data-ttu-id="2f9ee-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2f9ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f9ee-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f9ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f9ee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f9ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f9ee-107">Atualiza as propriedades de um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2f9ee-107">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f9ee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f9ee-108">Prerequisites</span></span>
<span data-ttu-id="2f9ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f9ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f9ee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f9ee-111">Permission type</span></span>|<span data-ttu-id="2f9ee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f9ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f9ee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f9ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f9ee-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f9ee-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2f9ee-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f9ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f9ee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f9ee-116">Not supported.</span></span>|
|<span data-ttu-id="2f9ee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f9ee-117">Application</span></span>|<span data-ttu-id="2f9ee-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f9ee-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f9ee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f9ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2f9ee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f9ee-120">Request headers</span></span>
|<span data-ttu-id="2f9ee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f9ee-121">Header</span></span>|<span data-ttu-id="2f9ee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2f9ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f9ee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f9ee-123">Authorization</span></span>|<span data-ttu-id="2f9ee-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f9ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f9ee-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f9ee-125">Accept</span></span>|<span data-ttu-id="2f9ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f9ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f9ee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f9ee-127">Request body</span></span>
<span data-ttu-id="2f9ee-128">No corpo da solicitação, forneça uma representação JSON do objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2f9ee-128">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="2f9ee-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2f9ee-129">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="2f9ee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f9ee-130">Property</span></span>|<span data-ttu-id="2f9ee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f9ee-131">Type</span></span>|<span data-ttu-id="2f9ee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f9ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f9ee-133">id</span><span class="sxs-lookup"><span data-stu-id="2f9ee-133">id</span></span>|<span data-ttu-id="2f9ee-134">String</span><span class="sxs-lookup"><span data-stu-id="2f9ee-134">String</span></span>|<span data-ttu-id="2f9ee-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f9ee-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="2f9ee-136">destino</span><span class="sxs-lookup"><span data-stu-id="2f9ee-136">target</span></span>|[<span data-ttu-id="2f9ee-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2f9ee-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2f9ee-138">Destino de atribuição ao qual o perfil de identidade visual está atribuído.</span><span class="sxs-lookup"><span data-stu-id="2f9ee-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="2f9ee-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f9ee-139">Response</span></span>
<span data-ttu-id="2f9ee-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f9ee-140">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f9ee-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f9ee-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f9ee-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f9ee-142">Request</span></span>
<span data-ttu-id="2f9ee-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f9ee-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
Content-type: application/json
Content-length: 171

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="2f9ee-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f9ee-144">Response</span></span>
<span data-ttu-id="2f9ee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f9ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 220

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





