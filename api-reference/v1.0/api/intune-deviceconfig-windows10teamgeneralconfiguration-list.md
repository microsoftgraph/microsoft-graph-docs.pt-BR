---
title: Listar windows10TeamGeneralConfigurations
description: Listar propriedades e relações dos objetos windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4277783f74289c5d0af8e4fb8a7ffa53c30f6f2c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971056"
---
# <a name="list-windows10teamgeneralconfigurations"></a><span data-ttu-id="e5b84-103">Listar windows10TeamGeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="e5b84-103">List windows10TeamGeneralConfigurations</span></span>

> <span data-ttu-id="e5b84-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5b84-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5b84-105">Listar propriedades e relações dos objetos [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5b84-105">List properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5b84-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e5b84-106">Prerequisites</span></span>
<span data-ttu-id="e5b84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5b84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5b84-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5b84-109">Permission type</span></span>|<span data-ttu-id="e5b84-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e5b84-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5b84-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5b84-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e5b84-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5b84-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e5b84-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5b84-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5b84-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5b84-114">Not supported.</span></span>|
|<span data-ttu-id="e5b84-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5b84-115">Application</span></span>|<span data-ttu-id="e5b84-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5b84-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5b84-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5b84-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e5b84-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5b84-118">Request headers</span></span>
|<span data-ttu-id="e5b84-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5b84-119">Header</span></span>|<span data-ttu-id="e5b84-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e5b84-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5b84-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5b84-121">Authorization</span></span>|<span data-ttu-id="e5b84-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5b84-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5b84-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e5b84-123">Accept</span></span>|<span data-ttu-id="e5b84-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e5b84-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5b84-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5b84-125">Request body</span></span>
<span data-ttu-id="e5b84-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5b84-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5b84-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5b84-127">Response</span></span>
<span data-ttu-id="e5b84-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5b84-128">If successful, this method returns a `200 OK` response code and a collection of [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5b84-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5b84-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5b84-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5b84-130">Request</span></span>
<span data-ttu-id="e5b84-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5b84-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="e5b84-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5b84-132">Response</span></span>
<span data-ttu-id="e5b84-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5b84-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



