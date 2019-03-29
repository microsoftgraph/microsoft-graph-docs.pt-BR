---
title: Atualizar intuneBrandingProfileAssignment
description: Atualiza as propriedades de um objeto intuneBrandingProfileAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e951ba830d60d1114c24f604e75d6afc55c83b1e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964518"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="57ffd-103">Atualizar intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="57ffd-103">Update intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="57ffd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57ffd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57ffd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57ffd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57ffd-106">Atualiza as propriedades de um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="57ffd-106">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57ffd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57ffd-107">Prerequisites</span></span>
<span data-ttu-id="57ffd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57ffd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57ffd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57ffd-110">Permission type</span></span>|<span data-ttu-id="57ffd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57ffd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57ffd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57ffd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57ffd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57ffd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="57ffd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57ffd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57ffd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57ffd-115">Not supported.</span></span>|
|<span data-ttu-id="57ffd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57ffd-116">Application</span></span>|<span data-ttu-id="57ffd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57ffd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57ffd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57ffd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="57ffd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57ffd-119">Request headers</span></span>
|<span data-ttu-id="57ffd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57ffd-120">Header</span></span>|<span data-ttu-id="57ffd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="57ffd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57ffd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="57ffd-122">Authorization</span></span>|<span data-ttu-id="57ffd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57ffd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57ffd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57ffd-124">Accept</span></span>|<span data-ttu-id="57ffd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57ffd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57ffd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57ffd-126">Request body</span></span>
<span data-ttu-id="57ffd-127">No corpo da solicitação, forneça uma representação JSON do objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="57ffd-127">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="57ffd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="57ffd-128">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="57ffd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57ffd-129">Property</span></span>|<span data-ttu-id="57ffd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="57ffd-130">Type</span></span>|<span data-ttu-id="57ffd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="57ffd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57ffd-132">id</span><span class="sxs-lookup"><span data-stu-id="57ffd-132">id</span></span>|<span data-ttu-id="57ffd-133">String</span><span class="sxs-lookup"><span data-stu-id="57ffd-133">String</span></span>|<span data-ttu-id="57ffd-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="57ffd-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="57ffd-135">destino</span><span class="sxs-lookup"><span data-stu-id="57ffd-135">target</span></span>|[<span data-ttu-id="57ffd-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="57ffd-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="57ffd-137">Destino de atribuição ao qual o perfil de identidade visual está atribuído.</span><span class="sxs-lookup"><span data-stu-id="57ffd-137">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="57ffd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="57ffd-138">Response</span></span>
<span data-ttu-id="57ffd-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57ffd-139">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57ffd-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57ffd-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="57ffd-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57ffd-141">Request</span></span>
<span data-ttu-id="57ffd-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57ffd-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="57ffd-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="57ffd-143">Response</span></span>
<span data-ttu-id="57ffd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57ffd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




