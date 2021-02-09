---
title: Atualizar appleEnrollmentProfileAssignment
description: Atualizar as propriedades de um objeto appleEnrollmentProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f10a0d383f0fe0475a7178b3f3a97b07eded50a4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159959"
---
# <a name="update-appleenrollmentprofileassignment"></a><span data-ttu-id="abe7f-103">Atualizar appleEnrollmentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="abe7f-103">Update appleEnrollmentProfileAssignment</span></span>

<span data-ttu-id="abe7f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abe7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abe7f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="abe7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abe7f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abe7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abe7f-107">Atualizar as propriedades de um [objeto appleEnrollmentProfileAssignment.](../resources/intune-enrollment-appleenrollmentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="abe7f-107">Update the properties of a [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abe7f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abe7f-108">Prerequisites</span></span>
<span data-ttu-id="abe7f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abe7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abe7f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abe7f-111">Permission type</span></span>|<span data-ttu-id="abe7f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="abe7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abe7f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abe7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abe7f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abe7f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="abe7f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abe7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abe7f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abe7f-116">Not supported.</span></span>|
|<span data-ttu-id="abe7f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abe7f-117">Application</span></span>|<span data-ttu-id="abe7f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abe7f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abe7f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abe7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="abe7f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abe7f-120">Request headers</span></span>
|<span data-ttu-id="abe7f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abe7f-121">Header</span></span>|<span data-ttu-id="abe7f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="abe7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abe7f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="abe7f-123">Authorization</span></span>|<span data-ttu-id="abe7f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abe7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abe7f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abe7f-125">Accept</span></span>|<span data-ttu-id="abe7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abe7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abe7f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abe7f-127">Request body</span></span>
<span data-ttu-id="abe7f-128">No corpo da solicitação, fornece uma representação JSON do [objeto appleEnrollmentProfileAssignment.](../resources/intune-enrollment-appleenrollmentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="abe7f-128">In the request body, supply a JSON representation for the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

<span data-ttu-id="abe7f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="abe7f-129">The following table shows the properties that are required when you create the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md).</span></span>

|<span data-ttu-id="abe7f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abe7f-130">Property</span></span>|<span data-ttu-id="abe7f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="abe7f-131">Type</span></span>|<span data-ttu-id="abe7f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="abe7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abe7f-133">id</span><span class="sxs-lookup"><span data-stu-id="abe7f-133">id</span></span>|<span data-ttu-id="abe7f-134">String</span><span class="sxs-lookup"><span data-stu-id="abe7f-134">String</span></span>|<span data-ttu-id="abe7f-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="abe7f-135">The key of the assignment.</span></span>|
|<span data-ttu-id="abe7f-136">destino</span><span class="sxs-lookup"><span data-stu-id="abe7f-136">target</span></span>|[<span data-ttu-id="abe7f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="abe7f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="abe7f-138">O destino da atribuição para o perfil de implantação iniciado pelo usuário da Apple.</span><span class="sxs-lookup"><span data-stu-id="abe7f-138">The assignment target for the Apple user initiated deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="abe7f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="abe7f-139">Response</span></span>
<span data-ttu-id="abe7f-140">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abe7f-140">If successful, this method returns a `200 OK` response code and an updated [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abe7f-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abe7f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="abe7f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abe7f-142">Request</span></span>
<span data-ttu-id="abe7f-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abe7f-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
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

### <a name="response"></a><span data-ttu-id="abe7f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="abe7f-144">Response</span></span>
<span data-ttu-id="abe7f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abe7f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




