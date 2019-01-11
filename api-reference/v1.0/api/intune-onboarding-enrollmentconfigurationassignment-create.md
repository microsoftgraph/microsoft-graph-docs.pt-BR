---
title: Criar enrollmentConfigurationAssignment
description: Criar um novo objeto enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d378b9f4663a6f3770d00a0f7971d1bc4c3b01b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844083"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="741ad-103">Criar enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="741ad-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="741ad-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="741ad-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="741ad-105">Criar um novo objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="741ad-105">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="741ad-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="741ad-106">Prerequisites</span></span>
<span data-ttu-id="741ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="741ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="741ad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="741ad-109">Permission type</span></span>|<span data-ttu-id="741ad-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="741ad-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="741ad-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="741ad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="741ad-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="741ad-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="741ad-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="741ad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="741ad-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="741ad-114">Not supported.</span></span>|
|<span data-ttu-id="741ad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="741ad-115">Application</span></span>|<span data-ttu-id="741ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="741ad-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="741ad-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="741ad-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="741ad-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="741ad-118">Request headers</span></span>
|<span data-ttu-id="741ad-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="741ad-119">Header</span></span>|<span data-ttu-id="741ad-120">Valor</span><span class="sxs-lookup"><span data-stu-id="741ad-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="741ad-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="741ad-121">Authorization</span></span>|<span data-ttu-id="741ad-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="741ad-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="741ad-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="741ad-123">Accept</span></span>|<span data-ttu-id="741ad-124">application/json</span><span class="sxs-lookup"><span data-stu-id="741ad-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="741ad-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="741ad-125">Request body</span></span>
<span data-ttu-id="741ad-126">No corpo da solicitação, forneça uma representação JSON do objeto enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="741ad-126">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="741ad-127">A tabela a seguir mostra as propriedades que são necessárias ao criar enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="741ad-127">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="741ad-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="741ad-128">Property</span></span>|<span data-ttu-id="741ad-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="741ad-129">Type</span></span>|<span data-ttu-id="741ad-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="741ad-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="741ad-131">id</span><span class="sxs-lookup"><span data-stu-id="741ad-131">id</span></span>|<span data-ttu-id="741ad-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="741ad-132">String</span></span>|<span data-ttu-id="741ad-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="741ad-133">Not yet documented</span></span>|
|<span data-ttu-id="741ad-134">destino</span><span class="sxs-lookup"><span data-stu-id="741ad-134">target</span></span>|[<span data-ttu-id="741ad-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="741ad-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="741ad-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="741ad-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="741ad-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="741ad-137">Response</span></span>
<span data-ttu-id="741ad-138">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="741ad-138">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="741ad-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="741ad-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="741ad-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="741ad-140">Request</span></span>
<span data-ttu-id="741ad-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="741ad-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="741ad-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="741ad-142">Response</span></span>
<span data-ttu-id="741ad-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="741ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



