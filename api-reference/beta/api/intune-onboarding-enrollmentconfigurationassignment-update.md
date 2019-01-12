---
title: Atualizar enrollmentConfigurationAssignment
description: Atualizar as propriedades de um objeto enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 01d17a5f4cb1f5d61e05e1e9d0b14a4708dce8b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963182"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="a4699-103">Atualizar enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a4699-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="a4699-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a4699-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4699-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a4699-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4699-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a4699-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4699-107">Atualizar as propriedades de um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a4699-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a4699-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a4699-108">Prerequisites</span></span>
<span data-ttu-id="a4699-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4699-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4699-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4699-111">Permission type</span></span>|<span data-ttu-id="a4699-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a4699-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4699-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4699-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4699-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4699-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a4699-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4699-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4699-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4699-116">Not supported.</span></span>|
|<span data-ttu-id="a4699-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4699-117">Application</span></span>|<span data-ttu-id="a4699-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4699-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4699-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4699-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="a4699-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4699-120">Request headers</span></span>
|<span data-ttu-id="a4699-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a4699-121">Header</span></span>|<span data-ttu-id="a4699-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a4699-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4699-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4699-123">Authorization</span></span>|<span data-ttu-id="a4699-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4699-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4699-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a4699-125">Accept</span></span>|<span data-ttu-id="a4699-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4699-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4699-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4699-127">Request body</span></span>
<span data-ttu-id="a4699-128">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a4699-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="a4699-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a4699-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="a4699-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4699-130">Property</span></span>|<span data-ttu-id="a4699-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4699-131">Type</span></span>|<span data-ttu-id="a4699-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4699-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4699-133">id</span><span class="sxs-lookup"><span data-stu-id="a4699-133">id</span></span>|<span data-ttu-id="a4699-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4699-134">String</span></span>|<span data-ttu-id="a4699-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a4699-135">Not yet documented</span></span>|
|<span data-ttu-id="a4699-136">destino</span><span class="sxs-lookup"><span data-stu-id="a4699-136">target</span></span>|[<span data-ttu-id="a4699-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a4699-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a4699-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a4699-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a4699-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4699-139">Response</span></span>
<span data-ttu-id="a4699-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4699-140">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4699-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4699-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a4699-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4699-142">Request</span></span>
<span data-ttu-id="a4699-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4699-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="a4699-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4699-144">Response</span></span>
<span data-ttu-id="a4699-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4699-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





