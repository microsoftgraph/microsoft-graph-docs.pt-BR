---
title: Atualizar enrollmentConfigurationAssignment
description: Atualizar as propriedades de um objeto enrollmentConfigurationAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0af3350dfaa963755b749b56b60ee57ea77d3f8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512472"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="7ed2d-103">Atualizar enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7ed2d-103">Update enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="7ed2d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ed2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ed2d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ed2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ed2d-106">Atualizar as propriedades de um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7ed2d-106">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ed2d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ed2d-107">Prerequisites</span></span>
<span data-ttu-id="7ed2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ed2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ed2d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ed2d-110">Permission type</span></span>|<span data-ttu-id="7ed2d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ed2d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ed2d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ed2d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ed2d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ed2d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7ed2d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ed2d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ed2d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ed2d-115">Not supported.</span></span>|
|<span data-ttu-id="7ed2d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ed2d-116">Application</span></span>|<span data-ttu-id="7ed2d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ed2d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ed2d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ed2d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7ed2d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed2d-119">Request headers</span></span>
|<span data-ttu-id="7ed2d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ed2d-120">Header</span></span>|<span data-ttu-id="7ed2d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7ed2d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ed2d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ed2d-122">Authorization</span></span>|<span data-ttu-id="7ed2d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ed2d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ed2d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7ed2d-124">Accept</span></span>|<span data-ttu-id="7ed2d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ed2d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ed2d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed2d-126">Request body</span></span>
<span data-ttu-id="7ed2d-127">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7ed2d-127">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="7ed2d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7ed2d-128">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="7ed2d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ed2d-129">Property</span></span>|<span data-ttu-id="7ed2d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ed2d-130">Type</span></span>|<span data-ttu-id="7ed2d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ed2d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ed2d-132">id</span><span class="sxs-lookup"><span data-stu-id="7ed2d-132">id</span></span>|<span data-ttu-id="7ed2d-133">String</span><span class="sxs-lookup"><span data-stu-id="7ed2d-133">String</span></span>|<span data-ttu-id="7ed2d-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7ed2d-134">Not yet documented</span></span>|
|<span data-ttu-id="7ed2d-135">destino</span><span class="sxs-lookup"><span data-stu-id="7ed2d-135">target</span></span>|[<span data-ttu-id="7ed2d-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7ed2d-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7ed2d-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7ed2d-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7ed2d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ed2d-138">Response</span></span>
<span data-ttu-id="7ed2d-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ed2d-139">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ed2d-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ed2d-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ed2d-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed2d-141">Request</span></span>
<span data-ttu-id="7ed2d-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ed2d-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="7ed2d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ed2d-143">Response</span></span>
<span data-ttu-id="7ed2d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ed2d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




