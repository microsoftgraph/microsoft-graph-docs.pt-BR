---
title: Get windows10TeamGeneralConfiguration
description: Ler propriedades e relações do objeto windows10TeamGeneralConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4af4e45dc87a569553eb4c00628bb880ad56fad3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42738113"
---
# <a name="get-windows10teamgeneralconfiguration"></a><span data-ttu-id="e9fdc-103">Get windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9fdc-103">Get windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="e9fdc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9fdc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9fdc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9fdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9fdc-106">Ler propriedades e relações do objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9fdc-106">Read properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9fdc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9fdc-107">Prerequisites</span></span>
<span data-ttu-id="e9fdc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9fdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9fdc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9fdc-110">Permission type</span></span>|<span data-ttu-id="e9fdc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e9fdc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9fdc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9fdc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e9fdc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9fdc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e9fdc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9fdc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9fdc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9fdc-115">Not supported.</span></span>|
|<span data-ttu-id="e9fdc-116">Application</span><span class="sxs-lookup"><span data-stu-id="e9fdc-116">Application</span></span>|<span data-ttu-id="e9fdc-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9fdc-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9fdc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9fdc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9fdc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9fdc-119">Optional query parameters</span></span>
<span data-ttu-id="e9fdc-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9fdc-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9fdc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9fdc-121">Request headers</span></span>
|<span data-ttu-id="e9fdc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9fdc-122">Header</span></span>|<span data-ttu-id="e9fdc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e9fdc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9fdc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9fdc-124">Authorization</span></span>|<span data-ttu-id="e9fdc-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9fdc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9fdc-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9fdc-126">Accept</span></span>|<span data-ttu-id="e9fdc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e9fdc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9fdc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9fdc-128">Request body</span></span>
<span data-ttu-id="e9fdc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9fdc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9fdc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9fdc-130">Response</span></span>
<span data-ttu-id="e9fdc-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9fdc-131">If successful, this method returns a `200 OK` response code and [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9fdc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9fdc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9fdc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9fdc-133">Request</span></span>
<span data-ttu-id="e9fdc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9fdc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e9fdc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9fdc-135">Response</span></span>
<span data-ttu-id="e9fdc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9fdc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2310

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
    "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "deviceManagementApplicabilityRuleOsEdition": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
      "osEditionTypes": [
        "windows10EnterpriseN"
      ],
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleOsVersion": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
      "minOSVersion": "Min OSVersion value",
      "maxOSVersion": "Max OSVersion value",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleDeviceMode": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
      "deviceMode": "sModeConfiguration",
      "name": "Name value",
      "ruleType": "exclude"
    },
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




