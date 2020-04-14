---
title: Listar macOSDeviceFeaturesConfigurations
description: Listar propriedades e relações dos objetos macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9e9dfac260f206adc4bd9d1ab6a67ca47dff46f1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438129"
---
# <a name="list-macosdevicefeaturesconfigurations"></a><span data-ttu-id="442ac-103">Listar macOSDeviceFeaturesConfigurations</span><span class="sxs-lookup"><span data-stu-id="442ac-103">List macOSDeviceFeaturesConfigurations</span></span>

<span data-ttu-id="442ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="442ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="442ac-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="442ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="442ac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="442ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="442ac-107">Listar propriedades e relações dos objetos [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="442ac-107">List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="442ac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="442ac-108">Prerequisites</span></span>
<span data-ttu-id="442ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="442ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="442ac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="442ac-111">Permission type</span></span>|<span data-ttu-id="442ac-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="442ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="442ac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="442ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="442ac-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="442ac-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="442ac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="442ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="442ac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="442ac-116">Not supported.</span></span>|
|<span data-ttu-id="442ac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="442ac-117">Application</span></span>|<span data-ttu-id="442ac-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="442ac-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="442ac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="442ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="442ac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="442ac-120">Request headers</span></span>
|<span data-ttu-id="442ac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="442ac-121">Header</span></span>|<span data-ttu-id="442ac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="442ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="442ac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="442ac-123">Authorization</span></span>|<span data-ttu-id="442ac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="442ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="442ac-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="442ac-125">Accept</span></span>|<span data-ttu-id="442ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="442ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="442ac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="442ac-127">Request body</span></span>
<span data-ttu-id="442ac-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="442ac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="442ac-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="442ac-129">Response</span></span>
<span data-ttu-id="442ac-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="442ac-130">If successful, this method returns a `200 OK` response code and a collection of [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="442ac-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="442ac-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="442ac-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="442ac-132">Request</span></span>
<span data-ttu-id="442ac-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="442ac-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="442ac-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="442ac-134">Response</span></span>
<span data-ttu-id="442ac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="442ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2985

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
      "screenLockDisableImmediate": true,
      "associatedDomains": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "singleSignOnExtension": {
        "@odata.type": "microsoft.graph.singleSignOnExtension"
      },
      "macOSSingleSignOnExtension": {
        "@odata.type": "microsoft.graph.macOSSingleSignOnExtension"
      }
    }
  ]
}
```



