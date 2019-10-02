---
title: Listar windows10TeamGeneralConfigurations
description: Listar propriedades e relações dos objetos windows10TeamGeneralConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10e8f0fe24f5e7ceb522b2d26f20564c49b8b061
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365201"
---
# <a name="list-windows10teamgeneralconfigurations"></a><span data-ttu-id="dd03c-103">Listar windows10TeamGeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="dd03c-103">List windows10TeamGeneralConfigurations</span></span>

> <span data-ttu-id="dd03c-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd03c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd03c-105">Listar propriedades e relações dos objetos [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd03c-105">List properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd03c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dd03c-106">Prerequisites</span></span>
<span data-ttu-id="dd03c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd03c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd03c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd03c-109">Permission type</span></span>|<span data-ttu-id="dd03c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dd03c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd03c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd03c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dd03c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd03c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dd03c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd03c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd03c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd03c-114">Not supported.</span></span>|
|<span data-ttu-id="dd03c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd03c-115">Application</span></span>|<span data-ttu-id="dd03c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd03c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd03c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd03c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dd03c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd03c-118">Request headers</span></span>
|<span data-ttu-id="dd03c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd03c-119">Header</span></span>|<span data-ttu-id="dd03c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="dd03c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd03c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd03c-121">Authorization</span></span>|<span data-ttu-id="dd03c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd03c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd03c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dd03c-123">Accept</span></span>|<span data-ttu-id="dd03c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dd03c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd03c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd03c-125">Request body</span></span>
<span data-ttu-id="dd03c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dd03c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd03c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd03c-127">Response</span></span>
<span data-ttu-id="dd03c-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd03c-128">If successful, this method returns a `200 OK` response code and a collection of [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd03c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd03c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd03c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd03c-130">Request</span></span>
<span data-ttu-id="dd03c-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd03c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="dd03c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd03c-132">Response</span></span>
<span data-ttu-id="dd03c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd03c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1463

{
  "value": [
    {
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
  ]
}
```




