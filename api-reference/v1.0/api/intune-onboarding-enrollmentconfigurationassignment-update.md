---
title: Atualizar enrollmentConfigurationAssignment
description: Atualizar as propriedades de um objeto enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da5bd6cdba47ffb80e5d20ea93b442942b0f102f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259378"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="1c0a3-103">Atualizar enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1c0a3-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="1c0a3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c0a3-105">Atualizar as propriedades de um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1c0a3-105">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c0a3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c0a3-106">Prerequisites</span></span>
<span data-ttu-id="1c0a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c0a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1c0a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c0a3-109">Permission type</span></span>|<span data-ttu-id="1c0a3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c0a3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c0a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c0a3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1c0a3-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c0a3-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1c0a3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c0a3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c0a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-114">Not supported.</span></span>|
|<span data-ttu-id="1c0a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c0a3-115">Application</span></span>|<span data-ttu-id="1c0a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c0a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c0a3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1c0a3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c0a3-118">Request headers</span></span>
|<span data-ttu-id="1c0a3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c0a3-119">Header</span></span>|<span data-ttu-id="1c0a3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1c0a3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c0a3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c0a3-121">Authorization</span></span>|<span data-ttu-id="1c0a3-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c0a3-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c0a3-123">Accept</span></span>|<span data-ttu-id="1c0a3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1c0a3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c0a3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c0a3-125">Request body</span></span>
<span data-ttu-id="1c0a3-126">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1c0a3-126">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="1c0a3-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1c0a3-127">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="1c0a3-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c0a3-128">Property</span></span>|<span data-ttu-id="1c0a3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c0a3-129">Type</span></span>|<span data-ttu-id="1c0a3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c0a3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c0a3-131">id</span><span class="sxs-lookup"><span data-stu-id="1c0a3-131">id</span></span>|<span data-ttu-id="1c0a3-132">String</span><span class="sxs-lookup"><span data-stu-id="1c0a3-132">String</span></span>|<span data-ttu-id="1c0a3-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1c0a3-133">Not yet documented</span></span>|
|<span data-ttu-id="1c0a3-134">destino</span><span class="sxs-lookup"><span data-stu-id="1c0a3-134">target</span></span>|[<span data-ttu-id="1c0a3-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1c0a3-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1c0a3-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1c0a3-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1c0a3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c0a3-137">Response</span></span>
<span data-ttu-id="1c0a3-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-138">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c0a3-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c0a3-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c0a3-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c0a3-140">Request</span></span>
<span data-ttu-id="1c0a3-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1c0a3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c0a3-142">Response</span></span>
<span data-ttu-id="1c0a3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c0a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



