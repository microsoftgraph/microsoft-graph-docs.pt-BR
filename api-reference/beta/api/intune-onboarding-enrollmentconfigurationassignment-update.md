---
title: Atualizar enrollmentConfigurationAssignment
description: Atualizar as propriedades de um objeto enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a9689ee23dfcfee522fd57070c118160d0bb58f5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157810"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="4def4-103">Atualizar enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4def4-103">Update enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="4def4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4def4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4def4-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4def4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4def4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4def4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4def4-107">Atualizar as propriedades de um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4def4-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4def4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4def4-108">Prerequisites</span></span>
<span data-ttu-id="4def4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4def4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4def4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4def4-111">Permission type</span></span>|<span data-ttu-id="4def4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4def4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4def4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4def4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4def4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4def4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4def4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4def4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4def4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4def4-116">Not supported.</span></span>|
|<span data-ttu-id="4def4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4def4-117">Application</span></span>|<span data-ttu-id="4def4-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4def4-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4def4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4def4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4def4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4def4-120">Request headers</span></span>
|<span data-ttu-id="4def4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4def4-121">Header</span></span>|<span data-ttu-id="4def4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4def4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4def4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4def4-123">Authorization</span></span>|<span data-ttu-id="4def4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4def4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4def4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4def4-125">Accept</span></span>|<span data-ttu-id="4def4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4def4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4def4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4def4-127">Request body</span></span>
<span data-ttu-id="4def4-128">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4def4-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="4def4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4def4-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="4def4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4def4-130">Property</span></span>|<span data-ttu-id="4def4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4def4-131">Type</span></span>|<span data-ttu-id="4def4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4def4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4def4-133">id</span><span class="sxs-lookup"><span data-stu-id="4def4-133">id</span></span>|<span data-ttu-id="4def4-134">String</span><span class="sxs-lookup"><span data-stu-id="4def4-134">String</span></span>|<span data-ttu-id="4def4-135">Chave da atribuição de configuração de registro</span><span class="sxs-lookup"><span data-stu-id="4def4-135">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="4def4-136">destino</span><span class="sxs-lookup"><span data-stu-id="4def4-136">target</span></span>|[<span data-ttu-id="4def4-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4def4-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4def4-138">Representa uma atribuição a dispositivos gerenciados no locatário</span><span class="sxs-lookup"><span data-stu-id="4def4-138">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="4def4-139">source</span><span class="sxs-lookup"><span data-stu-id="4def4-139">source</span></span>|[<span data-ttu-id="4def4-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="4def4-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="4def4-141">Tipo de recurso usado para implantação em um grupo, direct ou policySet.</span><span class="sxs-lookup"><span data-stu-id="4def4-141">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="4def4-142">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="4def4-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="4def4-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="4def4-143">sourceId</span></span>|<span data-ttu-id="4def4-144">String</span><span class="sxs-lookup"><span data-stu-id="4def4-144">String</span></span>|<span data-ttu-id="4def4-145">Identificador de recurso usado para implantação em um grupo</span><span class="sxs-lookup"><span data-stu-id="4def4-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="4def4-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="4def4-146">Response</span></span>
<span data-ttu-id="4def4-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4def4-147">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4def4-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4def4-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="4def4-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4def4-149">Request</span></span>
<span data-ttu-id="4def4-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4def4-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 453

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="4def4-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="4def4-151">Response</span></span>
<span data-ttu-id="4def4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4def4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




