---
title: Atualizar intuneBrandingProfileAssignment
description: Atualiza as propriedades de um objeto intuneBrandingProfileAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3743fd5148f46f5be3ea2447c1b52c1f63d0d2eb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799671"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="c9191-103">Atualizar intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="c9191-103">Update intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="c9191-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c9191-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9191-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c9191-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9191-106">Atualiza as propriedades de um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c9191-106">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9191-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c9191-107">Prerequisites</span></span>
<span data-ttu-id="c9191-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9191-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9191-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9191-110">Permission type</span></span>|<span data-ttu-id="c9191-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c9191-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9191-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9191-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9191-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9191-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c9191-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9191-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9191-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9191-115">Not supported.</span></span>|
|<span data-ttu-id="c9191-116">Application</span><span class="sxs-lookup"><span data-stu-id="c9191-116">Application</span></span>|<span data-ttu-id="c9191-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9191-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9191-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9191-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c9191-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9191-119">Request headers</span></span>
|<span data-ttu-id="c9191-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9191-120">Header</span></span>|<span data-ttu-id="c9191-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c9191-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9191-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9191-122">Authorization</span></span>|<span data-ttu-id="c9191-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9191-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9191-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c9191-124">Accept</span></span>|<span data-ttu-id="c9191-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9191-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9191-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9191-126">Request body</span></span>
<span data-ttu-id="c9191-127">No corpo da solicitação, forneça uma representação JSON do objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c9191-127">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="c9191-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c9191-128">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="c9191-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9191-129">Property</span></span>|<span data-ttu-id="c9191-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9191-130">Type</span></span>|<span data-ttu-id="c9191-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9191-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9191-132">id</span><span class="sxs-lookup"><span data-stu-id="c9191-132">id</span></span>|<span data-ttu-id="c9191-133">String</span><span class="sxs-lookup"><span data-stu-id="c9191-133">String</span></span>|<span data-ttu-id="c9191-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="c9191-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="c9191-135">destino</span><span class="sxs-lookup"><span data-stu-id="c9191-135">target</span></span>|[<span data-ttu-id="c9191-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c9191-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c9191-137">Destino de atribuição ao qual o perfil de identidade visual está atribuído.</span><span class="sxs-lookup"><span data-stu-id="c9191-137">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="c9191-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9191-138">Response</span></span>
<span data-ttu-id="c9191-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9191-139">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9191-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9191-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9191-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9191-141">Request</span></span>
<span data-ttu-id="c9191-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9191-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c9191-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9191-143">Response</span></span>
<span data-ttu-id="c9191-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9191-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




