---
title: Atualizar intuneBrandingProfileAssignment
description: Atualiza as propriedades de um objeto intuneBrandingProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a08c5cccd8837ae7b22cc9e333f783f259871da8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350122"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="fbda5-103">Atualizar intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="fbda5-103">Update intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="fbda5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fbda5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbda5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbda5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbda5-106">Atualiza as propriedades de um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="fbda5-106">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbda5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbda5-107">Prerequisites</span></span>
<span data-ttu-id="fbda5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbda5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbda5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbda5-110">Permission type</span></span>|<span data-ttu-id="fbda5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbda5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbda5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbda5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fbda5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbda5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fbda5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbda5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbda5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbda5-115">Not supported.</span></span>|
|<span data-ttu-id="fbda5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbda5-116">Application</span></span>|<span data-ttu-id="fbda5-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbda5-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbda5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbda5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="fbda5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbda5-119">Request headers</span></span>
|<span data-ttu-id="fbda5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbda5-120">Header</span></span>|<span data-ttu-id="fbda5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fbda5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbda5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbda5-122">Authorization</span></span>|<span data-ttu-id="fbda5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbda5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbda5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fbda5-124">Accept</span></span>|<span data-ttu-id="fbda5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fbda5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbda5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbda5-126">Request body</span></span>
<span data-ttu-id="fbda5-127">No corpo da solicitação, forneça uma representação JSON do objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="fbda5-127">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="fbda5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fbda5-128">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="fbda5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbda5-129">Property</span></span>|<span data-ttu-id="fbda5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbda5-130">Type</span></span>|<span data-ttu-id="fbda5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbda5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbda5-132">id</span><span class="sxs-lookup"><span data-stu-id="fbda5-132">id</span></span>|<span data-ttu-id="fbda5-133">String</span><span class="sxs-lookup"><span data-stu-id="fbda5-133">String</span></span>|<span data-ttu-id="fbda5-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="fbda5-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="fbda5-135">destino</span><span class="sxs-lookup"><span data-stu-id="fbda5-135">target</span></span>|[<span data-ttu-id="fbda5-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fbda5-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fbda5-137">Destino de atribuição ao qual o perfil de identidade visual está atribuído.</span><span class="sxs-lookup"><span data-stu-id="fbda5-137">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="fbda5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbda5-138">Response</span></span>
<span data-ttu-id="fbda5-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbda5-139">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbda5-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbda5-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbda5-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbda5-141">Request</span></span>
<span data-ttu-id="fbda5-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbda5-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fbda5-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbda5-143">Response</span></span>
<span data-ttu-id="fbda5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbda5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






