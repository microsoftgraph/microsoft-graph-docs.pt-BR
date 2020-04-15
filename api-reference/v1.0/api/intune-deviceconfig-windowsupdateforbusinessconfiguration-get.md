---
title: Get windowsUpdateForBusinessConfiguration
description: Ler propriedades e relações do objeto windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 53965c1370382794d6aa048a176db75a1fd3ee7f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43423428"
---
# <a name="get-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="4af24-103">Get windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="4af24-103">Get windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="4af24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4af24-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4af24-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4af24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4af24-106">Ler propriedades e relações do objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4af24-106">Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4af24-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4af24-107">Prerequisites</span></span>
<span data-ttu-id="4af24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4af24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4af24-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4af24-110">Permission type</span></span>|<span data-ttu-id="4af24-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4af24-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4af24-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4af24-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4af24-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4af24-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4af24-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4af24-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4af24-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4af24-115">Not supported.</span></span>|
|<span data-ttu-id="4af24-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4af24-116">Application</span></span>|<span data-ttu-id="4af24-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4af24-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4af24-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4af24-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4af24-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4af24-119">Optional query parameters</span></span>
<span data-ttu-id="4af24-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4af24-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4af24-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4af24-121">Request headers</span></span>
|<span data-ttu-id="4af24-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4af24-122">Header</span></span>|<span data-ttu-id="4af24-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4af24-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4af24-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4af24-124">Authorization</span></span>|<span data-ttu-id="4af24-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4af24-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4af24-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4af24-126">Accept</span></span>|<span data-ttu-id="4af24-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4af24-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4af24-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4af24-128">Request body</span></span>
<span data-ttu-id="4af24-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4af24-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4af24-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4af24-130">Response</span></span>
<span data-ttu-id="4af24-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4af24-131">If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4af24-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4af24-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4af24-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4af24-133">Request</span></span>
<span data-ttu-id="4af24-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4af24-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="4af24-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4af24-135">Response</span></span>
<span data-ttu-id="4af24-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4af24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1149

{
  "value": {
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
}
```






