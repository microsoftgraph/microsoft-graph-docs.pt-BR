---
title: Criar enrollmentConfigurationAssignment
description: Criar um novo objeto enrollmentConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 336cb12367b6092152febb275c329e31a9ad3c33
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941677"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="8df39-103">Criar enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8df39-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="8df39-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8df39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8df39-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8df39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8df39-106">Criar um novo objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8df39-106">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8df39-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8df39-107">Prerequisites</span></span>
<span data-ttu-id="8df39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8df39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8df39-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8df39-110">Permission type</span></span>|<span data-ttu-id="8df39-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8df39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8df39-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8df39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8df39-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8df39-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8df39-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8df39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8df39-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8df39-115">Not supported.</span></span>|
|<span data-ttu-id="8df39-116">Application</span><span class="sxs-lookup"><span data-stu-id="8df39-116">Application</span></span>|<span data-ttu-id="8df39-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8df39-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8df39-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8df39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8df39-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8df39-119">Request headers</span></span>
|<span data-ttu-id="8df39-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8df39-120">Header</span></span>|<span data-ttu-id="8df39-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8df39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8df39-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8df39-122">Authorization</span></span>|<span data-ttu-id="8df39-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8df39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8df39-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8df39-124">Accept</span></span>|<span data-ttu-id="8df39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8df39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8df39-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8df39-126">Request body</span></span>
<span data-ttu-id="8df39-127">No corpo da solicitação, forneça uma representação JSON do objeto enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="8df39-127">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="8df39-128">A tabela a seguir mostra as propriedades que são necessárias ao criar enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="8df39-128">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="8df39-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8df39-129">Property</span></span>|<span data-ttu-id="8df39-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8df39-130">Type</span></span>|<span data-ttu-id="8df39-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8df39-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8df39-132">id</span><span class="sxs-lookup"><span data-stu-id="8df39-132">id</span></span>|<span data-ttu-id="8df39-133">String</span><span class="sxs-lookup"><span data-stu-id="8df39-133">String</span></span>|<span data-ttu-id="8df39-134">Chave da atribuição de configuração de registro</span><span class="sxs-lookup"><span data-stu-id="8df39-134">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="8df39-135">destino</span><span class="sxs-lookup"><span data-stu-id="8df39-135">target</span></span>|[<span data-ttu-id="8df39-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8df39-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8df39-137">Representa uma atribuição para dispositivos gerenciados no locatário</span><span class="sxs-lookup"><span data-stu-id="8df39-137">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="8df39-138">source</span><span class="sxs-lookup"><span data-stu-id="8df39-138">source</span></span>|[<span data-ttu-id="8df39-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="8df39-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="8df39-140">Tipo de recurso usado para implantação em um grupo, direto ou policyset.</span><span class="sxs-lookup"><span data-stu-id="8df39-140">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="8df39-141">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="8df39-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="8df39-142">sourceId</span><span class="sxs-lookup"><span data-stu-id="8df39-142">sourceId</span></span>|<span data-ttu-id="8df39-143">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8df39-143">String</span></span>|<span data-ttu-id="8df39-144">Identificador para o recurso usado para implantação em um grupo</span><span class="sxs-lookup"><span data-stu-id="8df39-144">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="8df39-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8df39-145">Response</span></span>
<span data-ttu-id="8df39-146">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8df39-146">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8df39-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8df39-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="8df39-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8df39-148">Request</span></span>
<span data-ttu-id="8df39-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8df39-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
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

### <a name="response"></a><span data-ttu-id="8df39-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8df39-150">Response</span></span>
<span data-ttu-id="8df39-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8df39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





