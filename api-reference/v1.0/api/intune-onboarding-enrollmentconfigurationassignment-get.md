---
title: Get enrollmentConfigurationAssignment
description: Ler propriedades e relações do objeto enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9c5bcfaaf7e372df7ca84fc348afae80ec9e8770
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942420"
---
# <a name="get-enrollmentconfigurationassignment"></a><span data-ttu-id="8e87d-103">Get enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8e87d-103">Get enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="8e87d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8e87d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e87d-105">Ler propriedades e relações do objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8e87d-105">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e87d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e87d-106">Prerequisites</span></span>
<span data-ttu-id="8e87d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e87d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e87d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e87d-109">Permission type</span></span>|<span data-ttu-id="8e87d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e87d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e87d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e87d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e87d-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e87d-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8e87d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e87d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e87d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e87d-114">Not supported.</span></span>|
|<span data-ttu-id="8e87d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e87d-115">Application</span></span>|<span data-ttu-id="8e87d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e87d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e87d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e87d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e87d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8e87d-118">Optional query parameters</span></span>
<span data-ttu-id="8e87d-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8e87d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8e87d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e87d-120">Request headers</span></span>
|<span data-ttu-id="8e87d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e87d-121">Header</span></span>|<span data-ttu-id="8e87d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8e87d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e87d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e87d-123">Authorization</span></span>|<span data-ttu-id="8e87d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e87d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e87d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e87d-125">Accept</span></span>|<span data-ttu-id="8e87d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e87d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e87d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e87d-127">Request body</span></span>
<span data-ttu-id="8e87d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e87d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e87d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e87d-129">Response</span></span>
<span data-ttu-id="8e87d-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e87d-130">If successful, this method returns a `200 OK` response code and [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e87d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e87d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e87d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e87d-132">Request</span></span>
<span data-ttu-id="8e87d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e87d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="8e87d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e87d-134">Response</span></span>
<span data-ttu-id="8e87d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e87d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
    "id": "705b021c-021c-705b-1c02-5b701c025b70",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```



