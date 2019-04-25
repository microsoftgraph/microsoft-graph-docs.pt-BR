---
title: Criar enrollmentConfigurationAssignment
description: Criar um novo objeto enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c725f8468b9b8b210f7067705e0e19fe575fb4e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528824"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="9810f-103">Criar enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9810f-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="9810f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9810f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9810f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9810f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9810f-106">Criar um novo objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9810f-106">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9810f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9810f-107">Prerequisites</span></span>
<span data-ttu-id="9810f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9810f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9810f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9810f-110">Permission type</span></span>|<span data-ttu-id="9810f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9810f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9810f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9810f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9810f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9810f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9810f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9810f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9810f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9810f-115">Not supported.</span></span>|
|<span data-ttu-id="9810f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9810f-116">Application</span></span>|<span data-ttu-id="9810f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9810f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9810f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9810f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9810f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9810f-119">Request headers</span></span>
|<span data-ttu-id="9810f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9810f-120">Header</span></span>|<span data-ttu-id="9810f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9810f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9810f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9810f-122">Authorization</span></span>|<span data-ttu-id="9810f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9810f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9810f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9810f-124">Accept</span></span>|<span data-ttu-id="9810f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9810f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9810f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9810f-126">Request body</span></span>
<span data-ttu-id="9810f-127">No corpo da solicitação, forneça uma representação JSON do objeto enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="9810f-127">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="9810f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="9810f-128">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="9810f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9810f-129">Property</span></span>|<span data-ttu-id="9810f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9810f-130">Type</span></span>|<span data-ttu-id="9810f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9810f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9810f-132">id</span><span class="sxs-lookup"><span data-stu-id="9810f-132">id</span></span>|<span data-ttu-id="9810f-133">String</span><span class="sxs-lookup"><span data-stu-id="9810f-133">String</span></span>|<span data-ttu-id="9810f-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9810f-134">Not yet documented</span></span>|
|<span data-ttu-id="9810f-135">destino</span><span class="sxs-lookup"><span data-stu-id="9810f-135">target</span></span>|[<span data-ttu-id="9810f-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9810f-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9810f-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9810f-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9810f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9810f-138">Response</span></span>
<span data-ttu-id="9810f-139">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9810f-139">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9810f-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9810f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="9810f-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9810f-141">Request</span></span>
<span data-ttu-id="9810f-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9810f-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="9810f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9810f-143">Response</span></span>
<span data-ttu-id="9810f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9810f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





