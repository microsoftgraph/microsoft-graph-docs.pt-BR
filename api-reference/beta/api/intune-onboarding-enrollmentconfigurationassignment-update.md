---
title: Atualizar enrollmentConfigurationAssignment
description: Atualizar as propriedades de um objeto enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8f4aba8c5e1cd6a392661e84d60cf11496ec39f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868100"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="93ea3-103">Atualizar enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="93ea3-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="93ea3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="93ea3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93ea3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="93ea3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="93ea3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="93ea3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93ea3-107">Atualizar as propriedades de um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="93ea3-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="93ea3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="93ea3-108">Prerequisites</span></span>
<span data-ttu-id="93ea3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93ea3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93ea3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93ea3-111">Permission type</span></span>|<span data-ttu-id="93ea3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="93ea3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93ea3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93ea3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93ea3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93ea3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="93ea3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93ea3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93ea3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93ea3-116">Not supported.</span></span>|
|<span data-ttu-id="93ea3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93ea3-117">Application</span></span>|<span data-ttu-id="93ea3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93ea3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93ea3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93ea3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="93ea3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93ea3-120">Request headers</span></span>
|<span data-ttu-id="93ea3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93ea3-121">Header</span></span>|<span data-ttu-id="93ea3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="93ea3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93ea3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="93ea3-123">Authorization</span></span>|<span data-ttu-id="93ea3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93ea3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93ea3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="93ea3-125">Accept</span></span>|<span data-ttu-id="93ea3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93ea3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93ea3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93ea3-127">Request body</span></span>
<span data-ttu-id="93ea3-128">No corpo da solicitação, forneça uma representação JSON do objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="93ea3-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="93ea3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="93ea3-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="93ea3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93ea3-130">Property</span></span>|<span data-ttu-id="93ea3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="93ea3-131">Type</span></span>|<span data-ttu-id="93ea3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="93ea3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93ea3-133">id</span><span class="sxs-lookup"><span data-stu-id="93ea3-133">id</span></span>|<span data-ttu-id="93ea3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93ea3-134">String</span></span>|<span data-ttu-id="93ea3-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="93ea3-135">Not yet documented</span></span>|
|<span data-ttu-id="93ea3-136">destino</span><span class="sxs-lookup"><span data-stu-id="93ea3-136">target</span></span>|[<span data-ttu-id="93ea3-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="93ea3-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="93ea3-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="93ea3-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="93ea3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="93ea3-139">Response</span></span>
<span data-ttu-id="93ea3-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93ea3-140">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93ea3-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93ea3-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="93ea3-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93ea3-142">Request</span></span>
<span data-ttu-id="93ea3-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93ea3-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="93ea3-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="93ea3-144">Response</span></span>
<span data-ttu-id="93ea3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93ea3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





