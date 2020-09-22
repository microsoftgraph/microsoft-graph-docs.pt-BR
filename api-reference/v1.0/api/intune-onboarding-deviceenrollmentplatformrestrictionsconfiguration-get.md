---
title: Get deviceEnrollmentPlatformRestrictionsConfiguration
description: Ler propriedades e relações do objeto deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 306ecc66788a50d2d12450db8824dc4e316238ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033143"
---
# <a name="get-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="de2ca-103">Get deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="de2ca-103">Get deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="de2ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de2ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de2ca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de2ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de2ca-106">Ler propriedades e relações do objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="de2ca-106">Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de2ca-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de2ca-107">Prerequisites</span></span>
<span data-ttu-id="de2ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de2ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de2ca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de2ca-110">Permission type</span></span>|<span data-ttu-id="de2ca-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de2ca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de2ca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de2ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de2ca-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="de2ca-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="de2ca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de2ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de2ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de2ca-115">Not supported.</span></span>|
|<span data-ttu-id="de2ca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de2ca-116">Application</span></span>|<span data-ttu-id="de2ca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de2ca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de2ca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de2ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de2ca-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="de2ca-119">Optional query parameters</span></span>
<span data-ttu-id="de2ca-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="de2ca-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de2ca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de2ca-121">Request headers</span></span>
|<span data-ttu-id="de2ca-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de2ca-122">Header</span></span>|<span data-ttu-id="de2ca-123">Valor</span><span class="sxs-lookup"><span data-stu-id="de2ca-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de2ca-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="de2ca-124">Authorization</span></span>|<span data-ttu-id="de2ca-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de2ca-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de2ca-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de2ca-126">Accept</span></span>|<span data-ttu-id="de2ca-127">application/json</span><span class="sxs-lookup"><span data-stu-id="de2ca-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de2ca-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de2ca-128">Request body</span></span>
<span data-ttu-id="de2ca-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de2ca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de2ca-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="de2ca-130">Response</span></span>
<span data-ttu-id="de2ca-131">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de2ca-131">If successful, this method returns a `200 OK` response code and [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de2ca-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de2ca-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="de2ca-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de2ca-133">Request</span></span>
<span data-ttu-id="de2ca-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de2ca-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="de2ca-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="de2ca-135">Response</span></span>
<span data-ttu-id="de2ca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de2ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









