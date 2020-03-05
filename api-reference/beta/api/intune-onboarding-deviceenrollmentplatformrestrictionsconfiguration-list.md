---
title: Listar deviceEnrollmentPlatformRestrictionsConfigurations
description: Listar propriedades e relações de objeto de deviceEnrollmentPlatformRestrictionsConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27c1aea8a603bea38c61aa65f3a7d20db097487f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462366"
---
# <a name="list-deviceenrollmentplatformrestrictionsconfigurations"></a><span data-ttu-id="2b7fe-103">Listar deviceEnrollmentPlatformRestrictionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="2b7fe-103">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>

<span data-ttu-id="2b7fe-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2b7fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b7fe-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b7fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b7fe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b7fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b7fe-107">Listar propriedades e relações de objeto de [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b7fe-107">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b7fe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b7fe-108">Prerequisites</span></span>
<span data-ttu-id="2b7fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b7fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b7fe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b7fe-111">Permission type</span></span>|<span data-ttu-id="2b7fe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2b7fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b7fe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b7fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b7fe-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b7fe-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2b7fe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b7fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b7fe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b7fe-116">Not supported.</span></span>|
|<span data-ttu-id="2b7fe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b7fe-117">Application</span></span>|<span data-ttu-id="2b7fe-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b7fe-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b7fe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b7fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2b7fe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b7fe-120">Request headers</span></span>
|<span data-ttu-id="2b7fe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b7fe-121">Header</span></span>|<span data-ttu-id="2b7fe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2b7fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b7fe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b7fe-123">Authorization</span></span>|<span data-ttu-id="2b7fe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b7fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b7fe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2b7fe-125">Accept</span></span>|<span data-ttu-id="2b7fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b7fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b7fe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b7fe-127">Request body</span></span>
<span data-ttu-id="2b7fe-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b7fe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b7fe-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b7fe-129">Response</span></span>
<span data-ttu-id="2b7fe-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b7fe-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b7fe-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b7fe-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b7fe-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b7fe-132">Request</span></span>
<span data-ttu-id="2b7fe-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b7fe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="2b7fe-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b7fe-134">Response</span></span>
<span data-ttu-id="2b7fe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b7fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





