---
title: Listar deviceEnrollmentWindowsHelloForBusinessConfigurations
description: Listar propriedades e relações de objetos de deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d2e7a620b007e1a28c18727bbcbc8e9fcd69dc8c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846687"
---
# <a name="list-deviceenrollmentwindowshelloforbusinessconfigurations"></a><span data-ttu-id="6091f-103">Listar deviceEnrollmentWindowsHelloForBusinessConfigurations</span><span class="sxs-lookup"><span data-stu-id="6091f-103">List deviceEnrollmentWindowsHelloForBusinessConfigurations</span></span>

> <span data-ttu-id="6091f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6091f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6091f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6091f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6091f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6091f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6091f-107">Listar propriedades e relações de objetos de [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6091f-107">List properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6091f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6091f-108">Prerequisites</span></span>
<span data-ttu-id="6091f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6091f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6091f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6091f-111">Permission type</span></span>|<span data-ttu-id="6091f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6091f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6091f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6091f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6091f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6091f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6091f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6091f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6091f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6091f-116">Not supported.</span></span>|
|<span data-ttu-id="6091f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6091f-117">Application</span></span>|<span data-ttu-id="6091f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6091f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6091f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6091f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6091f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6091f-120">Request headers</span></span>
|<span data-ttu-id="6091f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6091f-121">Header</span></span>|<span data-ttu-id="6091f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6091f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6091f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6091f-123">Authorization</span></span>|<span data-ttu-id="6091f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6091f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6091f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6091f-125">Accept</span></span>|<span data-ttu-id="6091f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6091f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6091f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6091f-127">Request body</span></span>
<span data-ttu-id="6091f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6091f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6091f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6091f-129">Response</span></span>
<span data-ttu-id="6091f-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6091f-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6091f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6091f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6091f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6091f-132">Request</span></span>
<span data-ttu-id="6091f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6091f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="6091f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6091f-134">Response</span></span>
<span data-ttu-id="6091f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6091f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
  "value": [
    {
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
  ]
}
```





