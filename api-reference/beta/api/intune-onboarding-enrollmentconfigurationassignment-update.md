---
title: Atualizar enrollmentConfigurationAssignment
description: Atualizar as propriedades de um objeto enrollmentConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 96831fcb811b79aa62e19f7d12694c3385494098
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352599"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="f979e-103">Atualizar enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f979e-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="f979e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f979e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f979e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f979e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f979e-106">Atualizar as propriedades de um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f979e-106">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f979e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f979e-107">Prerequisites</span></span>
<span data-ttu-id="f979e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f979e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f979e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f979e-110">Permission type</span></span>|<span data-ttu-id="f979e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f979e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f979e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f979e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f979e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f979e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f979e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f979e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f979e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f979e-115">Not supported.</span></span>|
|<span data-ttu-id="f979e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f979e-116">Application</span></span>|<span data-ttu-id="f979e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f979e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f979e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f979e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f979e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f979e-119">Request headers</span></span>
|<span data-ttu-id="f979e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f979e-120">Header</span></span>|<span data-ttu-id="f979e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f979e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f979e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f979e-122">Authorization</span></span>|<span data-ttu-id="f979e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f979e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f979e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f979e-124">Accept</span></span>|<span data-ttu-id="f979e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f979e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f979e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f979e-126">Request body</span></span>
<span data-ttu-id="f979e-127">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f979e-127">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="f979e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f979e-128">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="f979e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f979e-129">Property</span></span>|<span data-ttu-id="f979e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f979e-130">Type</span></span>|<span data-ttu-id="f979e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f979e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f979e-132">id</span><span class="sxs-lookup"><span data-stu-id="f979e-132">id</span></span>|<span data-ttu-id="f979e-133">String</span><span class="sxs-lookup"><span data-stu-id="f979e-133">String</span></span>|<span data-ttu-id="f979e-134">Chave da atribuição de configuração de registro</span><span class="sxs-lookup"><span data-stu-id="f979e-134">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="f979e-135">destino</span><span class="sxs-lookup"><span data-stu-id="f979e-135">target</span></span>|[<span data-ttu-id="f979e-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f979e-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f979e-137">Representa uma atribuição para dispositivos gerenciados no locatário</span><span class="sxs-lookup"><span data-stu-id="f979e-137">Represents an assignment to managed devices in the tenant</span></span>|



## <a name="response"></a><span data-ttu-id="f979e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f979e-138">Response</span></span>
<span data-ttu-id="f979e-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f979e-139">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f979e-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f979e-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f979e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f979e-141">Request</span></span>
<span data-ttu-id="f979e-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f979e-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="f979e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f979e-143">Response</span></span>
<span data-ttu-id="f979e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f979e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






