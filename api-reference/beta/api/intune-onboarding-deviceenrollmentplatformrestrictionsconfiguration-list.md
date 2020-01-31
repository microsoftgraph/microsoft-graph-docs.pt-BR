---
title: Listar deviceEnrollmentPlatformRestrictionsConfigurations
description: Listar propriedades e relações de objeto de deviceEnrollmentPlatformRestrictionsConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: adc54ae17ad91e3256921ea9b15ba44727eeeb65
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41634974"
---
# <a name="list-deviceenrollmentplatformrestrictionsconfigurations"></a><span data-ttu-id="28c21-103">Listar deviceEnrollmentPlatformRestrictionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="28c21-103">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>

> <span data-ttu-id="28c21-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="28c21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28c21-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28c21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28c21-106">Listar propriedades e relações de objeto de [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28c21-106">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28c21-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="28c21-107">Prerequisites</span></span>
<span data-ttu-id="28c21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28c21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28c21-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28c21-110">Permission type</span></span>|<span data-ttu-id="28c21-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="28c21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28c21-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28c21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28c21-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="28c21-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="28c21-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28c21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28c21-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28c21-115">Not supported.</span></span>|
|<span data-ttu-id="28c21-116">Application</span><span class="sxs-lookup"><span data-stu-id="28c21-116">Application</span></span>|<span data-ttu-id="28c21-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="28c21-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28c21-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28c21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="28c21-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28c21-119">Request headers</span></span>
|<span data-ttu-id="28c21-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28c21-120">Header</span></span>|<span data-ttu-id="28c21-121">Valor</span><span class="sxs-lookup"><span data-stu-id="28c21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28c21-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="28c21-122">Authorization</span></span>|<span data-ttu-id="28c21-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28c21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28c21-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="28c21-124">Accept</span></span>|<span data-ttu-id="28c21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28c21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28c21-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28c21-126">Request body</span></span>
<span data-ttu-id="28c21-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28c21-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28c21-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="28c21-128">Response</span></span>
<span data-ttu-id="28c21-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28c21-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28c21-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28c21-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="28c21-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28c21-131">Request</span></span>
<span data-ttu-id="28c21-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28c21-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="28c21-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="28c21-133">Response</span></span>
<span data-ttu-id="28c21-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28c21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3280

{
  "value": [
    {
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
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ]
      },
      "windowsRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ]
      },
      "windowsMobileRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ]
      },
      "androidRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ]
      },
      "androidForWorkRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ]
      },
      "macRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ]
      },
      "macOSRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value",
        "blockedManufacturers": [
          "Blocked Manufacturers value"
        ]
      }
    }
  ]
}
```





