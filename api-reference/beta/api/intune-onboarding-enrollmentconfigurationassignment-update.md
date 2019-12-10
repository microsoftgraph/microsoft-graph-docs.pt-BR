---
title: Atualizar enrollmentConfigurationAssignment
description: Atualizar as propriedades de um objeto enrollmentConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ab02a29b0e0803484be4fb0e1930f7ba3fd987ae
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941649"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="d25d8-103">Atualizar enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d25d8-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="d25d8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d25d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d25d8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d25d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d25d8-106">Atualizar as propriedades de um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d25d8-106">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d25d8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d25d8-107">Prerequisites</span></span>
<span data-ttu-id="d25d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d25d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d25d8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d25d8-110">Permission type</span></span>|<span data-ttu-id="d25d8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d25d8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d25d8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d25d8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d25d8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d25d8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d25d8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d25d8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d25d8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d25d8-115">Not supported.</span></span>|
|<span data-ttu-id="d25d8-116">Application</span><span class="sxs-lookup"><span data-stu-id="d25d8-116">Application</span></span>|<span data-ttu-id="d25d8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d25d8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d25d8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d25d8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d25d8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d25d8-119">Request headers</span></span>
|<span data-ttu-id="d25d8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d25d8-120">Header</span></span>|<span data-ttu-id="d25d8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d25d8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d25d8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d25d8-122">Authorization</span></span>|<span data-ttu-id="d25d8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d25d8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d25d8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d25d8-124">Accept</span></span>|<span data-ttu-id="d25d8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d25d8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d25d8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d25d8-126">Request body</span></span>
<span data-ttu-id="d25d8-127">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d25d8-127">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="d25d8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d25d8-128">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="d25d8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d25d8-129">Property</span></span>|<span data-ttu-id="d25d8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d25d8-130">Type</span></span>|<span data-ttu-id="d25d8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d25d8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d25d8-132">id</span><span class="sxs-lookup"><span data-stu-id="d25d8-132">id</span></span>|<span data-ttu-id="d25d8-133">String</span><span class="sxs-lookup"><span data-stu-id="d25d8-133">String</span></span>|<span data-ttu-id="d25d8-134">Chave da atribuição de configuração de registro</span><span class="sxs-lookup"><span data-stu-id="d25d8-134">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="d25d8-135">destino</span><span class="sxs-lookup"><span data-stu-id="d25d8-135">target</span></span>|[<span data-ttu-id="d25d8-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d25d8-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d25d8-137">Representa uma atribuição para dispositivos gerenciados no locatário</span><span class="sxs-lookup"><span data-stu-id="d25d8-137">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="d25d8-138">source</span><span class="sxs-lookup"><span data-stu-id="d25d8-138">source</span></span>|[<span data-ttu-id="d25d8-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="d25d8-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="d25d8-140">Tipo de recurso usado para implantação em um grupo, direto ou policyset.</span><span class="sxs-lookup"><span data-stu-id="d25d8-140">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="d25d8-141">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="d25d8-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="d25d8-142">sourceId</span><span class="sxs-lookup"><span data-stu-id="d25d8-142">sourceId</span></span>|<span data-ttu-id="d25d8-143">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d25d8-143">String</span></span>|<span data-ttu-id="d25d8-144">Identificador para o recurso usado para implantação em um grupo</span><span class="sxs-lookup"><span data-stu-id="d25d8-144">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="d25d8-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d25d8-145">Response</span></span>
<span data-ttu-id="d25d8-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d25d8-146">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d25d8-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d25d8-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d25d8-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d25d8-148">Request</span></span>
<span data-ttu-id="d25d8-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d25d8-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 234

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="d25d8-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d25d8-150">Response</span></span>
<span data-ttu-id="d25d8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d25d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 283

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```





