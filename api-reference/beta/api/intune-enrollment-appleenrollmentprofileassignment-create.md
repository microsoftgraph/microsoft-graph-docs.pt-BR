---
title: Criar appleEnrollmentProfileAssignment
description: Crie um novo objeto appleEnrollmentProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ef40664db80b16329771eef64b02f94b0d38c87e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157762"
---
# <a name="create-appleenrollmentprofileassignment"></a><span data-ttu-id="bc290-103">Criar appleEnrollmentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="bc290-103">Create appleEnrollmentProfileAssignment</span></span>

<span data-ttu-id="bc290-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc290-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc290-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc290-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc290-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc290-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc290-107">Crie um novo [objeto appleEnrollmentProfileAssignment.](../resources/intune-enrollment-appleenrollmentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bc290-107">Create a new [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc290-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc290-108">Prerequisites</span></span>
<span data-ttu-id="bc290-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc290-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc290-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc290-111">Permission type</span></span>|<span data-ttu-id="bc290-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc290-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc290-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc290-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc290-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc290-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bc290-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc290-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc290-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc290-116">Not supported.</span></span>|
|<span data-ttu-id="bc290-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc290-117">Application</span></span>|<span data-ttu-id="bc290-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc290-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc290-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc290-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="bc290-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc290-120">Request headers</span></span>
|<span data-ttu-id="bc290-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc290-121">Header</span></span>|<span data-ttu-id="bc290-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bc290-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc290-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc290-123">Authorization</span></span>|<span data-ttu-id="bc290-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc290-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc290-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc290-125">Accept</span></span>|<span data-ttu-id="bc290-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc290-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc290-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc290-127">Request body</span></span>
<span data-ttu-id="bc290-128">No corpo da solicitação, fornece uma representação JSON para o objeto appleEnrollmentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="bc290-128">In the request body, supply a JSON representation for the appleEnrollmentProfileAssignment object.</span></span>

<span data-ttu-id="bc290-129">A tabela a seguir mostra as propriedades que são necessárias ao criar appleEnrollmentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="bc290-129">The following table shows the properties that are required when you create the appleEnrollmentProfileAssignment.</span></span>

|<span data-ttu-id="bc290-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc290-130">Property</span></span>|<span data-ttu-id="bc290-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc290-131">Type</span></span>|<span data-ttu-id="bc290-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc290-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc290-133">id</span><span class="sxs-lookup"><span data-stu-id="bc290-133">id</span></span>|<span data-ttu-id="bc290-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc290-134">String</span></span>|<span data-ttu-id="bc290-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="bc290-135">The key of the assignment.</span></span>|
|<span data-ttu-id="bc290-136">destino</span><span class="sxs-lookup"><span data-stu-id="bc290-136">target</span></span>|[<span data-ttu-id="bc290-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bc290-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bc290-138">O destino de atribuição para o perfil de implantação iniciado pelo usuário da Apple.</span><span class="sxs-lookup"><span data-stu-id="bc290-138">The assignment target for the Apple user initiated deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="bc290-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc290-139">Response</span></span>
<span data-ttu-id="bc290-140">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc290-140">If successful, this method returns a `201 Created` response code and a [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc290-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc290-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc290-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc290-142">Request</span></span>
<span data-ttu-id="bc290-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc290-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="bc290-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc290-144">Response</span></span>
<span data-ttu-id="bc290-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc290-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "id": "5b603771-3771-5b60-7137-605b7137605b",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




