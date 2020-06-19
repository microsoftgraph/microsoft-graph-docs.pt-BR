---
title: Atualizar enrollmentConfigurationAssignment
description: Atualizar as propriedades de um objeto enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aa4556309abf27cb92defa45869b072b1d351eea
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791774"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="99c01-103">Atualizar enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="99c01-103">Update enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="99c01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99c01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99c01-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99c01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99c01-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99c01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99c01-107">Atualizar as propriedades de um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="99c01-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99c01-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99c01-108">Prerequisites</span></span>
<span data-ttu-id="99c01-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="99c01-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="99c01-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99c01-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99c01-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99c01-111">Permission type</span></span>|<span data-ttu-id="99c01-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99c01-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99c01-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99c01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99c01-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99c01-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="99c01-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99c01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99c01-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99c01-116">Not supported.</span></span>|
|<span data-ttu-id="99c01-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99c01-117">Application</span></span>|<span data-ttu-id="99c01-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99c01-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99c01-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99c01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="99c01-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99c01-120">Request headers</span></span>
|<span data-ttu-id="99c01-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99c01-121">Header</span></span>|<span data-ttu-id="99c01-122">Valor</span><span class="sxs-lookup"><span data-stu-id="99c01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99c01-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="99c01-123">Authorization</span></span>|<span data-ttu-id="99c01-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99c01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99c01-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99c01-125">Accept</span></span>|<span data-ttu-id="99c01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99c01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99c01-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99c01-127">Request body</span></span>
<span data-ttu-id="99c01-128">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="99c01-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="99c01-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="99c01-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="99c01-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99c01-130">Property</span></span>|<span data-ttu-id="99c01-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="99c01-131">Type</span></span>|<span data-ttu-id="99c01-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="99c01-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99c01-133">id</span><span class="sxs-lookup"><span data-stu-id="99c01-133">id</span></span>|<span data-ttu-id="99c01-134">String</span><span class="sxs-lookup"><span data-stu-id="99c01-134">String</span></span>|<span data-ttu-id="99c01-135">Chave da atribuição de configuração de registro</span><span class="sxs-lookup"><span data-stu-id="99c01-135">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="99c01-136">destino</span><span class="sxs-lookup"><span data-stu-id="99c01-136">target</span></span>|[<span data-ttu-id="99c01-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="99c01-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="99c01-138">Representa uma atribuição para dispositivos gerenciados no locatário</span><span class="sxs-lookup"><span data-stu-id="99c01-138">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="99c01-139">source</span><span class="sxs-lookup"><span data-stu-id="99c01-139">source</span></span>|[<span data-ttu-id="99c01-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="99c01-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="99c01-141">Tipo de recurso usado para implantação em um grupo, direto ou policyset.</span><span class="sxs-lookup"><span data-stu-id="99c01-141">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="99c01-142">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="99c01-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="99c01-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="99c01-143">sourceId</span></span>|<span data-ttu-id="99c01-144">String</span><span class="sxs-lookup"><span data-stu-id="99c01-144">String</span></span>|<span data-ttu-id="99c01-145">Identificador para o recurso usado para implantação em um grupo</span><span class="sxs-lookup"><span data-stu-id="99c01-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="99c01-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="99c01-146">Response</span></span>
<span data-ttu-id="99c01-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99c01-147">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99c01-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99c01-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="99c01-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99c01-149">Request</span></span>
<span data-ttu-id="99c01-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99c01-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 389

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="99c01-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="99c01-151">Response</span></span>
<span data-ttu-id="99c01-152">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="99c01-152">Here is an example of the response.</span></span> <span data-ttu-id="99c01-153">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="99c01-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="99c01-154">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="99c01-154">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 438

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



