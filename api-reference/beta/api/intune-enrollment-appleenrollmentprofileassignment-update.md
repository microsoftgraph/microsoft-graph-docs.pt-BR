---
title: Atualizar appleEnrollmentProfileAssignment
description: Atualiza as propriedades de um objeto appleEnrollmentProfileAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 66af75684e8f6cbb761ed70262e52cadb719fc76
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813499"
---
# <a name="update-appleenrollmentprofileassignment"></a><span data-ttu-id="71ac3-103">Atualizar appleEnrollmentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="71ac3-103">Update appleEnrollmentProfileAssignment</span></span>

> <span data-ttu-id="71ac3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71ac3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71ac3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71ac3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71ac3-106">Atualiza as propriedades de um objeto [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="71ac3-106">Update the properties of a [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71ac3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71ac3-107">Prerequisites</span></span>
<span data-ttu-id="71ac3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71ac3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71ac3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71ac3-110">Permission type</span></span>|<span data-ttu-id="71ac3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71ac3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71ac3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71ac3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71ac3-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71ac3-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="71ac3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71ac3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71ac3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71ac3-115">Not supported.</span></span>|
|<span data-ttu-id="71ac3-116">Application</span><span class="sxs-lookup"><span data-stu-id="71ac3-116">Application</span></span>|<span data-ttu-id="71ac3-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71ac3-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71ac3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71ac3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="71ac3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71ac3-119">Request headers</span></span>
|<span data-ttu-id="71ac3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71ac3-120">Header</span></span>|<span data-ttu-id="71ac3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="71ac3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71ac3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="71ac3-122">Authorization</span></span>|<span data-ttu-id="71ac3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71ac3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71ac3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71ac3-124">Accept</span></span>|<span data-ttu-id="71ac3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71ac3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71ac3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71ac3-126">Request body</span></span>
<span data-ttu-id="71ac3-127">No corpo da solicitação, forneça uma representação JSON do objeto [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="71ac3-127">In the request body, supply a JSON representation for the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

<span data-ttu-id="71ac3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="71ac3-128">The following table shows the properties that are required when you create the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md).</span></span>

|<span data-ttu-id="71ac3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71ac3-129">Property</span></span>|<span data-ttu-id="71ac3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="71ac3-130">Type</span></span>|<span data-ttu-id="71ac3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="71ac3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71ac3-132">id</span><span class="sxs-lookup"><span data-stu-id="71ac3-132">id</span></span>|<span data-ttu-id="71ac3-133">String</span><span class="sxs-lookup"><span data-stu-id="71ac3-133">String</span></span>|<span data-ttu-id="71ac3-134">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="71ac3-134">The key of the assignment.</span></span>|
|<span data-ttu-id="71ac3-135">destino</span><span class="sxs-lookup"><span data-stu-id="71ac3-135">target</span></span>|[<span data-ttu-id="71ac3-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="71ac3-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="71ac3-137">O destino de atribuição para o perfil de implantação iniciado pelo usuário da Apple.</span><span class="sxs-lookup"><span data-stu-id="71ac3-137">The assignment target for the Apple user initiated deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="71ac3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="71ac3-138">Response</span></span>
<span data-ttu-id="71ac3-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71ac3-139">If successful, this method returns a `200 OK` response code and an updated [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71ac3-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71ac3-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="71ac3-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71ac3-141">Request</span></span>
<span data-ttu-id="71ac3-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71ac3-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="71ac3-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="71ac3-143">Response</span></span>
<span data-ttu-id="71ac3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71ac3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "id": "5b603771-3771-5b60-7137-605b7137605b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




