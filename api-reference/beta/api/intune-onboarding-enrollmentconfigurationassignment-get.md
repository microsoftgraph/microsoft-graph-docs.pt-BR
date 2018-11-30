---
title: Get enrollmentConfigurationAssignment
description: Ler propriedades e relações do objeto enrollmentConfigurationAssignment.
ms.openlocfilehash: 43e24d13802d07883e4a99daa19fe12fc7ca9390
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27032920"
---
# <a name="get-enrollmentconfigurationassignment"></a><span data-ttu-id="baf99-103">Get enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="baf99-103">Get enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="baf99-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="baf99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="baf99-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="baf99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="baf99-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="baf99-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="baf99-107">Ler propriedades e relações do objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="baf99-107">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="baf99-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="baf99-108">Prerequisites</span></span>
<span data-ttu-id="baf99-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baf99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baf99-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="baf99-111">Permission type</span></span>|<span data-ttu-id="baf99-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="baf99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baf99-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="baf99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="baf99-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="baf99-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="baf99-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="baf99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baf99-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="baf99-116">Not supported.</span></span>|
|<span data-ttu-id="baf99-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="baf99-117">Application</span></span>|<span data-ttu-id="baf99-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="baf99-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="baf99-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="baf99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="baf99-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="baf99-120">Optional query parameters</span></span>
<span data-ttu-id="baf99-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="baf99-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="baf99-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="baf99-122">Request headers</span></span>
|<span data-ttu-id="baf99-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="baf99-123">Header</span></span>|<span data-ttu-id="baf99-124">Valor</span><span class="sxs-lookup"><span data-stu-id="baf99-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="baf99-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="baf99-125">Authorization</span></span>|<span data-ttu-id="baf99-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="baf99-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="baf99-127">Accept</span><span class="sxs-lookup"><span data-stu-id="baf99-127">Accept</span></span>|<span data-ttu-id="baf99-128">application/json</span><span class="sxs-lookup"><span data-stu-id="baf99-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="baf99-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="baf99-129">Request body</span></span>
<span data-ttu-id="baf99-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="baf99-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="baf99-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="baf99-131">Response</span></span>
<span data-ttu-id="baf99-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="baf99-132">If successful, this method returns a `200 OK` response code and [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baf99-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="baf99-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="baf99-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="baf99-134">Request</span></span>
<span data-ttu-id="baf99-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="baf99-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="baf99-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="baf99-136">Response</span></span>
<span data-ttu-id="baf99-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="baf99-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





