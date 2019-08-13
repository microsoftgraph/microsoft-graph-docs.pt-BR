---
title: Obter deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Ler propriedades e relações do objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a003bd5227b5d76c0be7998d9be49987a0b7044d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352858"
---
# <a name="get-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="1beba-103">Obter deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="1beba-103">Get deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="1beba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1beba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1beba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1beba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1beba-106">Ler propriedades e relações do objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1beba-106">Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1beba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1beba-107">Prerequisites</span></span>
<span data-ttu-id="1beba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1beba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1beba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1beba-110">Permission type</span></span>|<span data-ttu-id="1beba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1beba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1beba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1beba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1beba-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1beba-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1beba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1beba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1beba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1beba-115">Not supported.</span></span>|
|<span data-ttu-id="1beba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1beba-116">Application</span></span>|<span data-ttu-id="1beba-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1beba-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1beba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1beba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1beba-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1beba-119">Optional query parameters</span></span>
<span data-ttu-id="1beba-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1beba-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1beba-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1beba-121">Request headers</span></span>
|<span data-ttu-id="1beba-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1beba-122">Header</span></span>|<span data-ttu-id="1beba-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1beba-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1beba-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1beba-124">Authorization</span></span>|<span data-ttu-id="1beba-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1beba-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1beba-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1beba-126">Accept</span></span>|<span data-ttu-id="1beba-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1beba-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1beba-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1beba-128">Request body</span></span>
<span data-ttu-id="1beba-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1beba-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1beba-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1beba-130">Response</span></span>
<span data-ttu-id="1beba-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1beba-131">If successful, this method returns a `200 OK` response code and [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1beba-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1beba-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1beba-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1beba-133">Request</span></span>
<span data-ttu-id="1beba-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1beba-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="1beba-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1beba-135">Response</span></span>
<span data-ttu-id="1beba-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1beba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 900

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
    "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7,
    "pinMinimumLength": 0,
    "pinMaximumLength": 0,
    "pinUppercaseCharactersUsage": "required",
    "pinLowercaseCharactersUsage": "required",
    "pinSpecialCharactersUsage": "required",
    "state": "enabled",
    "securityDeviceRequired": true,
    "unlockWithBiometricsEnabled": true,
    "remotePassportEnabled": true,
    "pinPreviousBlockCount": 5,
    "pinExpirationInDays": 3,
    "enhancedBiometricsState": "enabled",
    "securityKeyForSignIn": "enabled"
  }
}
```






