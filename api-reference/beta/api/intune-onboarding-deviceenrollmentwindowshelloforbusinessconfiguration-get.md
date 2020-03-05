---
title: Obter deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Ler propriedades e relações do objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 363ceb1eca301cb774ef971b18ede26d300e1f03
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462177"
---
# <a name="get-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="e9f81-103">Obter deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9f81-103">Get deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

<span data-ttu-id="e9f81-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e9f81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9f81-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9f81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9f81-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9f81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9f81-107">Ler propriedades e relações do objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9f81-107">Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9f81-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9f81-108">Prerequisites</span></span>
<span data-ttu-id="e9f81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9f81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9f81-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9f81-111">Permission type</span></span>|<span data-ttu-id="e9f81-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e9f81-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9f81-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9f81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9f81-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9f81-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e9f81-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9f81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9f81-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9f81-116">Not supported.</span></span>|
|<span data-ttu-id="e9f81-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9f81-117">Application</span></span>|<span data-ttu-id="e9f81-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9f81-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9f81-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9f81-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9f81-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9f81-120">Optional query parameters</span></span>
<span data-ttu-id="e9f81-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9f81-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9f81-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9f81-122">Request headers</span></span>
|<span data-ttu-id="e9f81-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9f81-123">Header</span></span>|<span data-ttu-id="e9f81-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e9f81-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9f81-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9f81-125">Authorization</span></span>|<span data-ttu-id="e9f81-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9f81-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9f81-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9f81-127">Accept</span></span>|<span data-ttu-id="e9f81-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e9f81-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9f81-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9f81-129">Request body</span></span>
<span data-ttu-id="e9f81-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9f81-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9f81-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9f81-131">Response</span></span>
<span data-ttu-id="e9f81-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9f81-132">If successful, this method returns a `200 OK` response code and [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9f81-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9f81-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9f81-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9f81-134">Request</span></span>
<span data-ttu-id="e9f81-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9f81-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e9f81-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9f81-136">Response</span></span>
<span data-ttu-id="e9f81-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9f81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





