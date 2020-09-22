---
title: Get windows10TeamGeneralConfiguration
description: Ler propriedades e relações do objeto windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56679df217ee7a5be7426c9d2d1daa32ad81856c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069957"
---
# <a name="get-windows10teamgeneralconfiguration"></a><span data-ttu-id="5a29d-103">Get windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="5a29d-103">Get windows10TeamGeneralConfiguration</span></span>

<span data-ttu-id="5a29d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a29d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a29d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5a29d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a29d-106">Ler propriedades e relações do objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a29d-106">Read properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a29d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5a29d-107">Prerequisites</span></span>
<span data-ttu-id="5a29d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a29d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a29d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a29d-110">Permission type</span></span>|<span data-ttu-id="5a29d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5a29d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a29d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a29d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a29d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a29d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5a29d-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a29d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a29d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a29d-115">Not supported.</span></span>|
|<span data-ttu-id="5a29d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a29d-116">Application</span></span>|<span data-ttu-id="5a29d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a29d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a29d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a29d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5a29d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5a29d-119">Optional query parameters</span></span>
<span data-ttu-id="5a29d-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5a29d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a29d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a29d-121">Request headers</span></span>
|<span data-ttu-id="5a29d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5a29d-122">Header</span></span>|<span data-ttu-id="5a29d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5a29d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a29d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a29d-124">Authorization</span></span>|<span data-ttu-id="5a29d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a29d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a29d-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5a29d-126">Accept</span></span>|<span data-ttu-id="5a29d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5a29d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a29d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a29d-128">Request body</span></span>
<span data-ttu-id="5a29d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a29d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a29d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a29d-130">Response</span></span>
<span data-ttu-id="5a29d-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a29d-131">If successful, this method returns a `200 OK` response code and [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a29d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a29d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a29d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a29d-133">Request</span></span>
<span data-ttu-id="5a29d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a29d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5a29d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a29d-135">Response</span></span>
<span data-ttu-id="5a29d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a29d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1395

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
    "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "azureOperationalInsightsBlockTelemetry": true,
    "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
    "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
    "connectAppBlockAutoLaunch": true,
    "maintenanceWindowBlocked": true,
    "maintenanceWindowDurationInHours": 0,
    "maintenanceWindowStartTime": "11:59:09.3130000",
    "miracastChannel": "one",
    "miracastBlocked": true,
    "miracastRequirePin": true,
    "settingsBlockMyMeetingsAndFiles": true,
    "settingsBlockSessionResume": true,
    "settingsBlockSigninSuggestions": true,
    "settingsDefaultVolume": 5,
    "settingsScreenTimeoutInMinutes": 14,
    "settingsSessionTimeoutInMinutes": 15,
    "settingsSleepTimeoutInMinutes": 13,
    "welcomeScreenBlockAutomaticWakeUp": true,
    "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
    "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
  }
}
```









