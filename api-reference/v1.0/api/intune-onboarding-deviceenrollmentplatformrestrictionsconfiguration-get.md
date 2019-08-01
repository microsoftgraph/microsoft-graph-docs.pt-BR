---
title: Get deviceEnrollmentPlatformRestrictionsConfiguration
description: Ler propriedades e relações do objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 52a5e06df8051be907ecfc85f0491ebc59397003
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974665"
---
# <a name="get-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="f077b-103">Get deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="f077b-103">Get deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="f077b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f077b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f077b-105">Ler propriedades e relações do objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f077b-105">Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f077b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f077b-106">Prerequisites</span></span>
<span data-ttu-id="f077b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f077b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f077b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f077b-109">Permission type</span></span>|<span data-ttu-id="f077b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f077b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f077b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f077b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f077b-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f077b-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f077b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f077b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f077b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f077b-114">Not supported.</span></span>|
|<span data-ttu-id="f077b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f077b-115">Application</span></span>|<span data-ttu-id="f077b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f077b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f077b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f077b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f077b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f077b-118">Optional query parameters</span></span>
<span data-ttu-id="f077b-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f077b-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f077b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f077b-120">Request headers</span></span>
|<span data-ttu-id="f077b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f077b-121">Header</span></span>|<span data-ttu-id="f077b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f077b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f077b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f077b-123">Authorization</span></span>|<span data-ttu-id="f077b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f077b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f077b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f077b-125">Accept</span></span>|<span data-ttu-id="f077b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f077b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f077b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f077b-127">Request body</span></span>
<span data-ttu-id="f077b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f077b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f077b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f077b-129">Response</span></span>
<span data-ttu-id="f077b-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f077b-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f077b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f077b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f077b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f077b-132">Request</span></span>
<span data-ttu-id="f077b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f077b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f077b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f077b-134">Response</span></span>
<span data-ttu-id="f077b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f077b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1927

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
    "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7,
    "iosRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    },
    "windowsRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    },
    "windowsMobileRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    },
    "androidRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    },
    "macOSRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    }
  }
}
```



