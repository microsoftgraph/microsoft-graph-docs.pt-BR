---
title: Listar deviceEnrollmentPlatformRestrictionsConfigurations
description: Listar propriedades e relações de objeto de deviceEnrollmentPlatformRestrictionsConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 906cd94551f1deb425a388407a53f45aa0e06e96
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362579"
---
# <a name="list-deviceenrollmentplatformrestrictionsconfigurations"></a><span data-ttu-id="c5f49-103">Listar deviceEnrollmentPlatformRestrictionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="c5f49-103">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>

> <span data-ttu-id="c5f49-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5f49-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5f49-105">Listar propriedades e relações de objeto de [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5f49-105">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5f49-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5f49-106">Prerequisites</span></span>
<span data-ttu-id="c5f49-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5f49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5f49-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5f49-109">Permission type</span></span>|<span data-ttu-id="c5f49-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5f49-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5f49-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5f49-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c5f49-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5f49-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c5f49-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5f49-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5f49-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5f49-114">Not supported.</span></span>|
|<span data-ttu-id="c5f49-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5f49-115">Application</span></span>|<span data-ttu-id="c5f49-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5f49-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5f49-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5f49-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c5f49-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f49-118">Request headers</span></span>
|<span data-ttu-id="c5f49-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5f49-119">Header</span></span>|<span data-ttu-id="c5f49-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c5f49-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5f49-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5f49-121">Authorization</span></span>|<span data-ttu-id="c5f49-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5f49-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5f49-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5f49-123">Accept</span></span>|<span data-ttu-id="c5f49-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c5f49-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5f49-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f49-125">Request body</span></span>
<span data-ttu-id="c5f49-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5f49-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5f49-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5f49-127">Response</span></span>
<span data-ttu-id="c5f49-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5f49-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5f49-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5f49-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5f49-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f49-130">Request</span></span>
<span data-ttu-id="c5f49-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5f49-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="c5f49-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5f49-132">Response</span></span>
<span data-ttu-id="c5f49-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5f49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2027

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




