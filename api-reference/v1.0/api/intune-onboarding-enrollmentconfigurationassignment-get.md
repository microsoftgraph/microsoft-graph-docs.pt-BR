---
title: Get enrollmentConfigurationAssignment
description: Ler propriedades e relações do objeto enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 18cb232f9a5bef40e56147efbb9035f98a0c55d4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024123"
---
# <a name="get-enrollmentconfigurationassignment"></a><span data-ttu-id="b6f29-103">Get enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b6f29-103">Get enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="b6f29-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6f29-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6f29-105">Ler propriedades e relações do objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b6f29-105">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6f29-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6f29-106">Prerequisites</span></span>
<span data-ttu-id="b6f29-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6f29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6f29-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6f29-109">Permission type</span></span>|<span data-ttu-id="b6f29-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6f29-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6f29-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6f29-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b6f29-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6f29-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b6f29-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6f29-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6f29-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6f29-114">Not supported.</span></span>|
|<span data-ttu-id="b6f29-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6f29-115">Application</span></span>|<span data-ttu-id="b6f29-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6f29-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6f29-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6f29-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6f29-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6f29-118">Optional query parameters</span></span>
<span data-ttu-id="b6f29-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6f29-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6f29-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f29-120">Request headers</span></span>
|<span data-ttu-id="b6f29-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6f29-121">Header</span></span>|<span data-ttu-id="b6f29-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6f29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6f29-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6f29-123">Authorization</span></span>|<span data-ttu-id="b6f29-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6f29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6f29-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6f29-125">Accept</span></span>|<span data-ttu-id="b6f29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6f29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6f29-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f29-127">Request body</span></span>
<span data-ttu-id="b6f29-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6f29-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6f29-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f29-129">Response</span></span>
<span data-ttu-id="b6f29-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6f29-130">If successful, this method returns a `200 OK` response code and [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6f29-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6f29-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6f29-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f29-132">Request</span></span>
<span data-ttu-id="b6f29-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6f29-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="b6f29-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f29-134">Response</span></span>
<span data-ttu-id="b6f29-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6f29-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



