---
title: Obter windows10EnrollmentCompletionPageConfiguration
description: Leia as propriedades e as relações do objeto windows10EnrollmentCompletionPageConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5979d7d446a79a8abdc4e7a2eae08968e1dafc3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147142"
---
# <a name="get-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="86ff5-103">Obter windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="86ff5-103">Get windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="86ff5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86ff5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86ff5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86ff5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86ff5-106">Leia as propriedades e as relações do objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="86ff5-106">Read properties and relationships of the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86ff5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86ff5-107">Prerequisites</span></span>
<span data-ttu-id="86ff5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="86ff5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="86ff5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86ff5-110">Permission type</span></span>|<span data-ttu-id="86ff5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86ff5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86ff5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86ff5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86ff5-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="86ff5-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="86ff5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86ff5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86ff5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86ff5-115">Not supported.</span></span>|
|<span data-ttu-id="86ff5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86ff5-116">Application</span></span>|<span data-ttu-id="86ff5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86ff5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86ff5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86ff5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86ff5-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="86ff5-119">Optional query parameters</span></span>
<span data-ttu-id="86ff5-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="86ff5-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86ff5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86ff5-121">Request headers</span></span>
|<span data-ttu-id="86ff5-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86ff5-122">Header</span></span>|<span data-ttu-id="86ff5-123">Valor</span><span class="sxs-lookup"><span data-stu-id="86ff5-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86ff5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="86ff5-124">Authorization</span></span>|<span data-ttu-id="86ff5-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86ff5-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86ff5-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86ff5-126">Accept</span></span>|<span data-ttu-id="86ff5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="86ff5-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86ff5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86ff5-128">Request body</span></span>
<span data-ttu-id="86ff5-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86ff5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86ff5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="86ff5-130">Response</span></span>
<span data-ttu-id="86ff5-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86ff5-131">If successful, this method returns a `200 OK` response code and [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86ff5-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86ff5-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="86ff5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86ff5-133">Request</span></span>
<span data-ttu-id="86ff5-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86ff5-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="86ff5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="86ff5-135">Response</span></span>
<span data-ttu-id="86ff5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86ff5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
    "id": "77bf8248-8248-77bf-4882-bf774882bf77",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7,
    "showInstallationProgress": true,
    "blockDeviceSetupRetryByUser": true,
    "allowDeviceResetOnInstallFailure": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "Custom Error Message value",
    "installProgressTimeoutInMinutes": 15,
    "allowDeviceUseOnInstallFailure": true,
    "selectedMobileAppIds": [
      "Selected Mobile App Ids value"
    ]
  }
}
```




