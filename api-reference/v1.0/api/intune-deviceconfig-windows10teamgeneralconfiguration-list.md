---
title: Listar windows10TeamGeneralConfigurations
description: Listar propriedades e relações dos objetos windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8cc7992b95d44a01795d49b4153e4cc2f9524b96
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760423"
---
# <a name="list-windows10teamgeneralconfigurations"></a><span data-ttu-id="72414-103">Listar windows10TeamGeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="72414-103">List windows10TeamGeneralConfigurations</span></span>

<span data-ttu-id="72414-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72414-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72414-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72414-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72414-106">Listar propriedades e relações dos objetos [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72414-106">List properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72414-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72414-107">Prerequisites</span></span>
<span data-ttu-id="72414-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72414-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72414-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72414-110">Permission type</span></span>|<span data-ttu-id="72414-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72414-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72414-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72414-112">Delegated (work or school account)</span></span>|<span data-ttu-id="72414-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72414-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72414-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72414-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72414-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72414-115">Not supported.</span></span>|
|<span data-ttu-id="72414-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72414-116">Application</span></span>|<span data-ttu-id="72414-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72414-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72414-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72414-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="72414-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72414-119">Request headers</span></span>
|<span data-ttu-id="72414-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72414-120">Header</span></span>|<span data-ttu-id="72414-121">Valor</span><span class="sxs-lookup"><span data-stu-id="72414-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72414-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="72414-122">Authorization</span></span>|<span data-ttu-id="72414-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72414-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72414-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="72414-124">Accept</span></span>|<span data-ttu-id="72414-125">application/json</span><span class="sxs-lookup"><span data-stu-id="72414-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72414-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72414-126">Request body</span></span>
<span data-ttu-id="72414-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72414-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72414-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="72414-128">Response</span></span>
<span data-ttu-id="72414-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72414-129">If successful, this method returns a `200 OK` response code and a collection of [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72414-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72414-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="72414-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72414-131">Request</span></span>
<span data-ttu-id="72414-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72414-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="72414-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="72414-133">Response</span></span>
<span data-ttu-id="72414-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72414-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




