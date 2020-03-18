---
title: Listar androidWorkProfileGeneralDeviceConfigurations
description: Listar Propriedades e relações dos objetos Entidadeandroidforworkprofiledeviceconfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e7dbfa07fee15e2a36167038620f73eeec98f13e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42758464"
---
# <a name="list-androidworkprofilegeneraldeviceconfigurations"></a><span data-ttu-id="f2f60-103">Listar androidWorkProfileGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="f2f60-103">List androidWorkProfileGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="f2f60-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2f60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2f60-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2f60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2f60-106">Listar Propriedades e relações dos objetos [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f2f60-106">List properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2f60-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2f60-107">Prerequisites</span></span>
<span data-ttu-id="f2f60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2f60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2f60-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2f60-110">Permission type</span></span>|<span data-ttu-id="f2f60-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2f60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2f60-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2f60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f2f60-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2f60-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f2f60-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2f60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2f60-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2f60-115">Not supported.</span></span>|
|<span data-ttu-id="f2f60-116">Application</span><span class="sxs-lookup"><span data-stu-id="f2f60-116">Application</span></span>|<span data-ttu-id="f2f60-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2f60-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2f60-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2f60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f2f60-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2f60-119">Request headers</span></span>
|<span data-ttu-id="f2f60-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2f60-120">Header</span></span>|<span data-ttu-id="f2f60-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f2f60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2f60-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2f60-122">Authorization</span></span>|<span data-ttu-id="f2f60-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2f60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2f60-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2f60-124">Accept</span></span>|<span data-ttu-id="f2f60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f2f60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2f60-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2f60-126">Request body</span></span>
<span data-ttu-id="f2f60-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2f60-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2f60-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2f60-128">Response</span></span>
<span data-ttu-id="f2f60-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2f60-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2f60-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2f60-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2f60-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2f60-131">Request</span></span>
<span data-ttu-id="f2f60-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2f60-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f2f60-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2f60-133">Response</span></span>
<span data-ttu-id="f2f60-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2f60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3402

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
      "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
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
      "passwordBlockFingerprintUnlock": true,
      "passwordBlockTrustAgents": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "lowSecurityBiometric",
      "workProfileDataSharingType": "preventAny",
      "workProfileBlockNotificationsWhileDeviceLocked": true,
      "workProfileBlockAddingAccounts": true,
      "workProfileBluetoothEnableContactSharing": true,
      "workProfileBlockScreenCapture": true,
      "workProfileBlockCrossProfileCallerId": true,
      "workProfileBlockCamera": true,
      "workProfileBlockCrossProfileContactsSearch": true,
      "workProfileBlockCrossProfileCopyPaste": true,
      "workProfileDefaultAppPermissionPolicy": "prompt",
      "workProfilePasswordBlockFingerprintUnlock": true,
      "workProfilePasswordBlockTrustAgents": true,
      "workProfilePasswordExpirationDays": 1,
      "workProfilePasswordMinimumLength": 0,
      "workProfilePasswordMinNumericCharacters": 7,
      "workProfilePasswordMinNonLetterCharacters": 9,
      "workProfilePasswordMinLetterCharacters": 6,
      "workProfilePasswordMinLowerCaseCharacters": 9,
      "workProfilePasswordMinUpperCaseCharacters": 9,
      "workProfilePasswordMinSymbolCharacters": 6,
      "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
      "workProfilePasswordPreviousPasswordBlockCount": 13,
      "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
      "workProfilePasswordRequiredType": "lowSecurityBiometric",
      "workProfileRequirePassword": true,
      "securityRequireVerifyApps": true,
      "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
      "vpnEnableAlwaysOnLockdownMode": true,
      "workProfileAllowWidgets": true,
      "workProfileBlockPersonalAppInstallsFromUnknownSources": true
    }
  ]
}
```




