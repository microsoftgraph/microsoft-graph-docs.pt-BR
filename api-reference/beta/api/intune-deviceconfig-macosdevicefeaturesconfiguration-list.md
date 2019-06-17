---
title: Listar macOSDeviceFeaturesConfigurations
description: Listar propriedades e relações dos objetos macOSDeviceFeaturesConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b0560e86a6de5e406e96b6f377ea6ae40fc7adf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963377"
---
# <a name="list-macosdevicefeaturesconfigurations"></a><span data-ttu-id="fca9b-103">Listar macOSDeviceFeaturesConfigurations</span><span class="sxs-lookup"><span data-stu-id="fca9b-103">List macOSDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="fca9b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fca9b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fca9b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fca9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fca9b-106">Listar propriedades e relações dos objetos [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fca9b-106">List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fca9b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fca9b-107">Prerequisites</span></span>
<span data-ttu-id="fca9b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fca9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fca9b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fca9b-110">Permission type</span></span>|<span data-ttu-id="fca9b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fca9b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fca9b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fca9b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fca9b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fca9b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fca9b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fca9b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fca9b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fca9b-115">Not supported.</span></span>|
|<span data-ttu-id="fca9b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fca9b-116">Application</span></span>|<span data-ttu-id="fca9b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fca9b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fca9b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fca9b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fca9b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fca9b-119">Request headers</span></span>
|<span data-ttu-id="fca9b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fca9b-120">Header</span></span>|<span data-ttu-id="fca9b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fca9b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fca9b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fca9b-122">Authorization</span></span>|<span data-ttu-id="fca9b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fca9b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fca9b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fca9b-124">Accept</span></span>|<span data-ttu-id="fca9b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fca9b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fca9b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fca9b-126">Request body</span></span>
<span data-ttu-id="fca9b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fca9b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fca9b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fca9b-128">Response</span></span>
<span data-ttu-id="fca9b-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fca9b-129">If successful, this method returns a `200 OK` response code and a collection of [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fca9b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fca9b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fca9b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fca9b-131">Request</span></span>
<span data-ttu-id="fca9b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fca9b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="fca9b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fca9b-133">Response</span></span>
<span data-ttu-id="fca9b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fca9b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2572

{
  "value": [
    {
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
  ]
}
```





