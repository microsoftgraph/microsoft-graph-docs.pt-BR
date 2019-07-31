---
title: Listar macOSDeviceFeaturesConfigurations
description: Listar propriedades e relações dos objetos macOSDeviceFeaturesConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01b48b75172a3d6dcf2c3d37095446e96a267c10
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35947393"
---
# <a name="list-macosdevicefeaturesconfigurations"></a><span data-ttu-id="1bb70-103">Listar macOSDeviceFeaturesConfigurations</span><span class="sxs-lookup"><span data-stu-id="1bb70-103">List macOSDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="1bb70-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1bb70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bb70-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1bb70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bb70-106">Listar propriedades e relações dos objetos [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1bb70-106">List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bb70-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1bb70-107">Prerequisites</span></span>
<span data-ttu-id="1bb70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bb70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bb70-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bb70-110">Permission type</span></span>|<span data-ttu-id="1bb70-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1bb70-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bb70-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bb70-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1bb70-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bb70-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1bb70-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bb70-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bb70-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bb70-115">Not supported.</span></span>|
|<span data-ttu-id="1bb70-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bb70-116">Application</span></span>|<span data-ttu-id="1bb70-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bb70-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bb70-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bb70-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1bb70-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb70-119">Request headers</span></span>
|<span data-ttu-id="1bb70-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1bb70-120">Header</span></span>|<span data-ttu-id="1bb70-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1bb70-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bb70-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bb70-122">Authorization</span></span>|<span data-ttu-id="1bb70-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bb70-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bb70-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1bb70-124">Accept</span></span>|<span data-ttu-id="1bb70-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1bb70-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bb70-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb70-126">Request body</span></span>
<span data-ttu-id="1bb70-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1bb70-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bb70-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bb70-128">Response</span></span>
<span data-ttu-id="1bb70-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bb70-129">If successful, this method returns a `200 OK` response code and a collection of [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bb70-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bb70-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bb70-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb70-131">Request</span></span>
<span data-ttu-id="1bb70-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bb70-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1bb70-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bb70-133">Response</span></span>
<span data-ttu-id="1bb70-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bb70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





