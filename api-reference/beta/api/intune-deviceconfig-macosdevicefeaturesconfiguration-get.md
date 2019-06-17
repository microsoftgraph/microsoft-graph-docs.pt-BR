---
title: Obter macOSDeviceFeaturesConfiguration
description: Ler propriedades e relações do objeto macOSDeviceFeaturesConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4437be5924c9bb30b0d4b2bbf952cc867eef453
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34976852"
---
# <a name="get-macosdevicefeaturesconfiguration"></a><span data-ttu-id="e03d3-103">Obter macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="e03d3-103">Get macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="e03d3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e03d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e03d3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e03d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e03d3-106">Ler propriedades e relações do objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e03d3-106">Read properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e03d3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e03d3-107">Prerequisites</span></span>
<span data-ttu-id="e03d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e03d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e03d3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e03d3-110">Permission type</span></span>|<span data-ttu-id="e03d3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e03d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e03d3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e03d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e03d3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e03d3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e03d3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e03d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e03d3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e03d3-115">Not supported.</span></span>|
|<span data-ttu-id="e03d3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e03d3-116">Application</span></span>|<span data-ttu-id="e03d3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e03d3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e03d3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e03d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e03d3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e03d3-119">Optional query parameters</span></span>
<span data-ttu-id="e03d3-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e03d3-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e03d3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e03d3-121">Request headers</span></span>
|<span data-ttu-id="e03d3-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e03d3-122">Header</span></span>|<span data-ttu-id="e03d3-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e03d3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e03d3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e03d3-124">Authorization</span></span>|<span data-ttu-id="e03d3-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e03d3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e03d3-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e03d3-126">Accept</span></span>|<span data-ttu-id="e03d3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e03d3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e03d3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e03d3-128">Request body</span></span>
<span data-ttu-id="e03d3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e03d3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e03d3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e03d3-130">Response</span></span>
<span data-ttu-id="e03d3-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e03d3-131">If successful, this method returns a `200 OK` response code and [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e03d3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e03d3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e03d3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e03d3-133">Request</span></span>
<span data-ttu-id="e03d3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e03d3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e03d3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e03d3-135">Response</span></span>
<span data-ttu-id="e03d3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e03d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2428

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
    "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
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
    "airPrintDestinations": [
      {
        "@odata.type": "microsoft.graph.airPrintDestination",
        "ipAddress": "Ip Address value",
        "resourcePath": "Resource Path value",
        "port": 4,
        "forceTls": true
      }
    ],
    "autoLaunchItems": [
      {
        "@odata.type": "microsoft.graph.macOSLaunchItem",
        "path": "Path value",
        "hide": true
      }
    ],
    "adminShowHostInfo": true,
    "loginWindowText": "Login Window Text value",
    "authorizedUsersListHidden": true,
    "authorizedUsersListHideLocalUsers": true,
    "authorizedUsersListHideMobileAccounts": true,
    "authorizedUsersListIncludeNetworkUsers": true,
    "authorizedUsersListHideAdminUsers": true,
    "authorizedUsersListShowOtherManagedUsers": true,
    "shutDownDisabled": true,
    "restartDisabled": true,
    "sleepDisabled": true,
    "consoleAccessDisabled": true,
    "shutDownDisabledWhileLoggedIn": true,
    "restartDisabledWhileLoggedIn": true,
    "powerOffDisabledWhileLoggedIn": true,
    "logOutDisabledWhileLoggedIn": true,
    "screenLockDisableImmediate": true
  }
}
```





