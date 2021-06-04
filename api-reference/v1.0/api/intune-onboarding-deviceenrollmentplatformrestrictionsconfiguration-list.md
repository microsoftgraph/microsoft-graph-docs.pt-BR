---
title: Listar deviceEnrollmentPlatformRestrictionsConfigurations
description: Listar propriedades e relações de objeto de deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f1b1c5e77818a57bd0de2ea0817ebb17d09c3095
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52744677"
---
# <a name="list-deviceenrollmentplatformrestrictionsconfigurations"></a><span data-ttu-id="fa122-103">Listar deviceEnrollmentPlatformRestrictionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="fa122-103">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>

<span data-ttu-id="fa122-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa122-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa122-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa122-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa122-106">Listar propriedades e relações de objeto de [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa122-106">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa122-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fa122-107">Prerequisites</span></span>
<span data-ttu-id="fa122-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa122-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa122-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa122-110">Permission type</span></span>|<span data-ttu-id="fa122-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa122-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa122-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa122-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa122-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa122-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fa122-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa122-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa122-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa122-115">Not supported.</span></span>|
|<span data-ttu-id="fa122-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa122-116">Application</span></span>|<span data-ttu-id="fa122-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa122-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa122-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa122-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fa122-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa122-119">Request headers</span></span>
|<span data-ttu-id="fa122-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa122-120">Header</span></span>|<span data-ttu-id="fa122-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fa122-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa122-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa122-122">Authorization</span></span>|<span data-ttu-id="fa122-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa122-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa122-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fa122-124">Accept</span></span>|<span data-ttu-id="fa122-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa122-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa122-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa122-126">Request body</span></span>
<span data-ttu-id="fa122-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa122-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa122-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa122-128">Response</span></span>
<span data-ttu-id="fa122-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa122-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa122-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa122-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa122-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa122-131">Request</span></span>
<span data-ttu-id="fa122-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa122-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="fa122-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa122-133">Response</span></span>
<span data-ttu-id="fa122-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa122-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




