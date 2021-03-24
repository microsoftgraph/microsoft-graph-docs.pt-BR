---
title: Atualizar enrollmentConfigurationAssignment
description: Atualizar as propriedades de um objeto enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 24a37d1369bcedc6cc388cc07b1c8c17b9b40a29
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145394"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="b9e77-103">Atualizar enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b9e77-103">Update enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="b9e77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9e77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9e77-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9e77-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9e77-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9e77-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9e77-107">Atualizar as propriedades de um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b9e77-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9e77-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9e77-108">Prerequisites</span></span>
<span data-ttu-id="b9e77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9e77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9e77-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9e77-111">Permission type</span></span>|<span data-ttu-id="b9e77-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9e77-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9e77-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9e77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9e77-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9e77-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b9e77-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9e77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9e77-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9e77-116">Not supported.</span></span>|
|<span data-ttu-id="b9e77-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9e77-117">Application</span></span>|<span data-ttu-id="b9e77-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9e77-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9e77-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9e77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b9e77-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9e77-120">Request headers</span></span>
|<span data-ttu-id="b9e77-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9e77-121">Header</span></span>|<span data-ttu-id="b9e77-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b9e77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9e77-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9e77-123">Authorization</span></span>|<span data-ttu-id="b9e77-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9e77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9e77-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9e77-125">Accept</span></span>|<span data-ttu-id="b9e77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9e77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9e77-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9e77-127">Request body</span></span>
<span data-ttu-id="b9e77-128">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b9e77-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="b9e77-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b9e77-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="b9e77-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9e77-130">Property</span></span>|<span data-ttu-id="b9e77-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9e77-131">Type</span></span>|<span data-ttu-id="b9e77-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9e77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9e77-133">id</span><span class="sxs-lookup"><span data-stu-id="b9e77-133">id</span></span>|<span data-ttu-id="b9e77-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9e77-134">String</span></span>|<span data-ttu-id="b9e77-135">Chave da atribuição de configuração de registro</span><span class="sxs-lookup"><span data-stu-id="b9e77-135">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="b9e77-136">destino</span><span class="sxs-lookup"><span data-stu-id="b9e77-136">target</span></span>|[<span data-ttu-id="b9e77-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b9e77-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b9e77-138">Representa uma atribuição a dispositivos gerenciados no locatário</span><span class="sxs-lookup"><span data-stu-id="b9e77-138">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="b9e77-139">source</span><span class="sxs-lookup"><span data-stu-id="b9e77-139">source</span></span>|[<span data-ttu-id="b9e77-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="b9e77-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="b9e77-141">Tipo de recurso usado para implantação para um grupo, direto ou policySet.</span><span class="sxs-lookup"><span data-stu-id="b9e77-141">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="b9e77-142">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="b9e77-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="b9e77-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="b9e77-143">sourceId</span></span>|<span data-ttu-id="b9e77-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9e77-144">String</span></span>|<span data-ttu-id="b9e77-145">Identificador de recurso usado para implantação em um grupo</span><span class="sxs-lookup"><span data-stu-id="b9e77-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="b9e77-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9e77-146">Response</span></span>
<span data-ttu-id="b9e77-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9e77-147">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9e77-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9e77-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9e77-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9e77-149">Request</span></span>
<span data-ttu-id="b9e77-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9e77-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b9e77-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9e77-151">Response</span></span>
<span data-ttu-id="b9e77-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9e77-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




