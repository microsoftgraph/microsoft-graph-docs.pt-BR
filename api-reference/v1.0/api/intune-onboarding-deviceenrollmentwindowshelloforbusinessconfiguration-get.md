---
title: Obter deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Ler propriedades e relações do objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
ms.openlocfilehash: bb8a6b580b226b4b60cd357a1e52da49ef497e95
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339141"
---
# <a name="get-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="fbd6c-103">Obter deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="fbd6c-103">Get deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="fbd6c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fbd6c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbd6c-105">Ler propriedades e relações do objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd6c-105">Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fbd6c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbd6c-106">Prerequisites</span></span>
<span data-ttu-id="fbd6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbd6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbd6c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbd6c-109">Permission type</span></span>|<span data-ttu-id="fbd6c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbd6c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbd6c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbd6c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fbd6c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbd6c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fbd6c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbd6c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbd6c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbd6c-114">Not supported.</span></span>|
|<span data-ttu-id="fbd6c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbd6c-115">Application</span></span>|<span data-ttu-id="fbd6c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbd6c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbd6c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbd6c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fbd6c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fbd6c-118">Optional query parameters</span></span>
<span data-ttu-id="fbd6c-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fbd6c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fbd6c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbd6c-120">Request headers</span></span>
|<span data-ttu-id="fbd6c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbd6c-121">Header</span></span>|<span data-ttu-id="fbd6c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fbd6c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbd6c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbd6c-123">Authorization</span></span>|<span data-ttu-id="fbd6c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbd6c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbd6c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fbd6c-125">Accept</span></span>|<span data-ttu-id="fbd6c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbd6c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbd6c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbd6c-127">Request body</span></span>
<span data-ttu-id="fbd6c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fbd6c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbd6c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbd6c-129">Response</span></span>
<span data-ttu-id="fbd6c-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbd6c-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbd6c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbd6c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fbd6c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbd6c-132">Request</span></span>
<span data-ttu-id="fbd6c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbd6c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="fbd6c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbd6c-134">Response</span></span>
<span data-ttu-id="fbd6c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbd6c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 860

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
    "enhancedBiometricsState": "enabled"
  }
}
```



