---
title: Listar windowsPhone81GeneralConfigurations
description: Listar propriedades e relações dos objetos windowsPhone81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3b4f0ab6c4c1940a0150765235ea045abf475ad2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726875"
---
# <a name="list-windowsphone81generalconfigurations"></a><span data-ttu-id="61d42-103">Listar windowsPhone81GeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="61d42-103">List windowsPhone81GeneralConfigurations</span></span>

<span data-ttu-id="61d42-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61d42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61d42-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61d42-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61d42-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61d42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61d42-107">Listar propriedades e relações dos objetos [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="61d42-107">List properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61d42-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61d42-108">Prerequisites</span></span>
<span data-ttu-id="61d42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61d42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61d42-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61d42-111">Permission type</span></span>|<span data-ttu-id="61d42-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61d42-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61d42-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61d42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61d42-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="61d42-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="61d42-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61d42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61d42-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61d42-116">Not supported.</span></span>|
|<span data-ttu-id="61d42-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61d42-117">Application</span></span>|<span data-ttu-id="61d42-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="61d42-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61d42-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61d42-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="61d42-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61d42-120">Request headers</span></span>
|<span data-ttu-id="61d42-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61d42-121">Header</span></span>|<span data-ttu-id="61d42-122">Valor</span><span class="sxs-lookup"><span data-stu-id="61d42-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61d42-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="61d42-123">Authorization</span></span>|<span data-ttu-id="61d42-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61d42-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61d42-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61d42-125">Accept</span></span>|<span data-ttu-id="61d42-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61d42-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61d42-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61d42-127">Request body</span></span>
<span data-ttu-id="61d42-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61d42-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61d42-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="61d42-129">Response</span></span>
<span data-ttu-id="61d42-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61d42-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61d42-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61d42-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="61d42-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61d42-132">Request</span></span>
<span data-ttu-id="61d42-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61d42-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="61d42-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="61d42-134">Response</span></span>
<span data-ttu-id="61d42-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61d42-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2807

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
      "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
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
      "applyOnlyToWindowsPhone81": true,
      "appsBlockCopyPaste": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "cellularBlockWifiTethering": true,
      "compliantAppsList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "compliantAppListType": "appsInListCompliant",
      "diagnosticDataBlockSubmission": true,
      "emailBlockAddingAccounts": true,
      "locationServicesBlocked": true,
      "microsoftAccountBlocked": true,
      "nfcBlocked": true,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordMinimumCharacterSetCount": 0,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "alphanumeric",
      "passwordRequired": true,
      "screenCaptureBlocked": true,
      "storageBlockRemovableStorage": true,
      "storageRequireEncryption": true,
      "webBrowserBlocked": true,
      "wifiBlocked": true,
      "wifiBlockAutomaticConnectHotspots": true,
      "wifiBlockHotspotReporting": true,
      "windowsStoreBlocked": true
    }
  ]
}
```





