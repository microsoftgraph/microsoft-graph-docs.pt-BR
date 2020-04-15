---
title: Listar windows10TeamGeneralConfigurations
description: Listar propriedades e relações dos objetos windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d71e29b1ef9e0fb181334f97afe1523bb6cbd8e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442009"
---
# <a name="list-windows10teamgeneralconfigurations"></a><span data-ttu-id="c1b06-103">Listar windows10TeamGeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="c1b06-103">List windows10TeamGeneralConfigurations</span></span>

<span data-ttu-id="c1b06-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1b06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1b06-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c1b06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1b06-106">Listar propriedades e relações dos objetos [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1b06-106">List properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1b06-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c1b06-107">Prerequisites</span></span>
<span data-ttu-id="c1b06-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1b06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1b06-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1b06-110">Permission type</span></span>|<span data-ttu-id="c1b06-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c1b06-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1b06-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1b06-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1b06-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1b06-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c1b06-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1b06-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1b06-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1b06-115">Not supported.</span></span>|
|<span data-ttu-id="c1b06-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1b06-116">Application</span></span>|<span data-ttu-id="c1b06-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1b06-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1b06-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1b06-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c1b06-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1b06-119">Request headers</span></span>
|<span data-ttu-id="c1b06-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c1b06-120">Header</span></span>|<span data-ttu-id="c1b06-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c1b06-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1b06-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1b06-122">Authorization</span></span>|<span data-ttu-id="c1b06-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1b06-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1b06-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c1b06-124">Accept</span></span>|<span data-ttu-id="c1b06-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1b06-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1b06-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1b06-126">Request body</span></span>
<span data-ttu-id="c1b06-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c1b06-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1b06-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1b06-128">Response</span></span>
<span data-ttu-id="c1b06-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1b06-129">If successful, this method returns a `200 OK` response code and a collection of [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1b06-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1b06-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1b06-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1b06-131">Request</span></span>
<span data-ttu-id="c1b06-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1b06-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c1b06-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1b06-133">Response</span></span>
<span data-ttu-id="c1b06-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1b06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






