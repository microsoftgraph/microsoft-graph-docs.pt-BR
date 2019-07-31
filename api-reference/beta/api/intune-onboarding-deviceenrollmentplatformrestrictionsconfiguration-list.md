---
title: Listar deviceEnrollmentPlatformRestrictionsConfigurations
description: Listar propriedades e relações de objeto de deviceEnrollmentPlatformRestrictionsConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86bc9b40cb06e98de7e9a2a92c4c601ef91cee5f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984591"
---
# <a name="list-deviceenrollmentplatformrestrictionsconfigurations"></a><span data-ttu-id="d43ce-103">Listar deviceEnrollmentPlatformRestrictionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="d43ce-103">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>

> <span data-ttu-id="d43ce-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d43ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d43ce-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d43ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d43ce-106">Listar propriedades e relações de objeto de [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d43ce-106">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d43ce-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d43ce-107">Prerequisites</span></span>
<span data-ttu-id="d43ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d43ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d43ce-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d43ce-110">Permission type</span></span>|<span data-ttu-id="d43ce-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d43ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d43ce-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d43ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d43ce-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d43ce-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d43ce-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d43ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d43ce-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d43ce-115">Not supported.</span></span>|
|<span data-ttu-id="d43ce-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d43ce-116">Application</span></span>|<span data-ttu-id="d43ce-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d43ce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d43ce-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d43ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d43ce-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d43ce-119">Request headers</span></span>
|<span data-ttu-id="d43ce-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d43ce-120">Header</span></span>|<span data-ttu-id="d43ce-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d43ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d43ce-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d43ce-122">Authorization</span></span>|<span data-ttu-id="d43ce-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d43ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d43ce-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d43ce-124">Accept</span></span>|<span data-ttu-id="d43ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d43ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d43ce-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d43ce-126">Request body</span></span>
<span data-ttu-id="d43ce-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d43ce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d43ce-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d43ce-128">Response</span></span>
<span data-ttu-id="d43ce-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d43ce-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d43ce-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d43ce-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d43ce-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d43ce-131">Request</span></span>
<span data-ttu-id="d43ce-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d43ce-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="d43ce-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d43ce-133">Response</span></span>
<span data-ttu-id="d43ce-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d43ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2664

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
      "androidForWorkRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "macRestriction": {
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
  ]
}
```





