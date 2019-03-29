---
title: Criar intuneBrandingProfileAssignment
description: Criar um novo objeto intuneBrandingProfileAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97e8743b93ab0ce89f43d7714c7bf9aa12d81b06
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960549"
---
# <a name="create-intunebrandingprofileassignment"></a><span data-ttu-id="9541f-103">Criar intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="9541f-103">Create intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="9541f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9541f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9541f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9541f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9541f-106">Criar um novo objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9541f-106">Create a new [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9541f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9541f-107">Prerequisites</span></span>
<span data-ttu-id="9541f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9541f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9541f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9541f-110">Permission type</span></span>|<span data-ttu-id="9541f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9541f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9541f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9541f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9541f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9541f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9541f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9541f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9541f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9541f-115">Not supported.</span></span>|
|<span data-ttu-id="9541f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9541f-116">Application</span></span>|<span data-ttu-id="9541f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9541f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9541f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9541f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9541f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9541f-119">Request headers</span></span>
|<span data-ttu-id="9541f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9541f-120">Header</span></span>|<span data-ttu-id="9541f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9541f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9541f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9541f-122">Authorization</span></span>|<span data-ttu-id="9541f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9541f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9541f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9541f-124">Accept</span></span>|<span data-ttu-id="9541f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9541f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9541f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9541f-126">Request body</span></span>
<span data-ttu-id="9541f-127">No corpo da solicitação, forneça uma representação JSON do objeto intuneBrandingProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="9541f-127">In the request body, supply a JSON representation for the intuneBrandingProfileAssignment object.</span></span>

<span data-ttu-id="9541f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar intuneBrandingProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="9541f-128">The following table shows the properties that are required when you create the intuneBrandingProfileAssignment.</span></span>

|<span data-ttu-id="9541f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9541f-129">Property</span></span>|<span data-ttu-id="9541f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9541f-130">Type</span></span>|<span data-ttu-id="9541f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9541f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9541f-132">id</span><span class="sxs-lookup"><span data-stu-id="9541f-132">id</span></span>|<span data-ttu-id="9541f-133">String</span><span class="sxs-lookup"><span data-stu-id="9541f-133">String</span></span>|<span data-ttu-id="9541f-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="9541f-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="9541f-135">destino</span><span class="sxs-lookup"><span data-stu-id="9541f-135">target</span></span>|[<span data-ttu-id="9541f-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9541f-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9541f-137">Destino de atribuição ao qual o perfil de identidade visual está atribuído.</span><span class="sxs-lookup"><span data-stu-id="9541f-137">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="9541f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9541f-138">Response</span></span>
<span data-ttu-id="9541f-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9541f-139">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9541f-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9541f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="9541f-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9541f-141">Request</span></span>
<span data-ttu-id="9541f-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9541f-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
Content-type: application/json
Content-length: 171

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="9541f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9541f-143">Response</span></span>
<span data-ttu-id="9541f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9541f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




