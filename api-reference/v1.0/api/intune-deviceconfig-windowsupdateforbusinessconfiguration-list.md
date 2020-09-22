---
title: Listar windowsUpdateForBusinessConfigurations
description: Listar propriedades e relações dos objetos windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3c0772abf8a8500b1c1308130aaa2428027ca575
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063195"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="a6007-103">Listar windowsUpdateForBusinessConfigurations</span><span class="sxs-lookup"><span data-stu-id="a6007-103">List windowsUpdateForBusinessConfigurations</span></span>

<span data-ttu-id="a6007-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6007-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6007-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6007-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6007-106">Listar propriedades e relações dos objetos [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6007-106">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6007-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6007-107">Prerequisites</span></span>
<span data-ttu-id="a6007-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6007-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6007-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6007-110">Permission type</span></span>|<span data-ttu-id="a6007-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6007-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6007-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6007-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6007-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6007-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a6007-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6007-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6007-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6007-115">Not supported.</span></span>|
|<span data-ttu-id="a6007-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6007-116">Application</span></span>|<span data-ttu-id="a6007-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6007-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6007-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6007-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a6007-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6007-119">Request headers</span></span>
|<span data-ttu-id="a6007-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6007-120">Header</span></span>|<span data-ttu-id="a6007-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a6007-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6007-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6007-122">Authorization</span></span>|<span data-ttu-id="a6007-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6007-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6007-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6007-124">Accept</span></span>|<span data-ttu-id="a6007-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6007-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6007-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6007-126">Request body</span></span>
<span data-ttu-id="a6007-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6007-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6007-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6007-128">Response</span></span>
<span data-ttu-id="a6007-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6007-129">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6007-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6007-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6007-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6007-131">Request</span></span>
<span data-ttu-id="a6007-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6007-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a6007-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6007-133">Response</span></span>
<span data-ttu-id="a6007-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6007-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1211

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
      "id": "4928dd6a-dd6a-4928-6add-28496add2849",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "deliveryOptimizationMode": "httpOnly",
      "prereleaseFeatures": "settingsOnly",
      "automaticUpdateMode": "notifyDownload",
      "microsoftUpdateServiceAllowed": true,
      "driversExcluded": true,
      "installationSchedule": {
        "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
        "scheduledInstallDay": "everyday",
        "scheduledInstallTime": "11:59:31.3170000"
      },
      "qualityUpdatesDeferralPeriodInDays": 2,
      "featureUpdatesDeferralPeriodInDays": 2,
      "qualityUpdatesPaused": true,
      "featureUpdatesPaused": true,
      "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
      "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
      "businessReadyUpdatesOnly": "all"
    }
  ]
}
```









