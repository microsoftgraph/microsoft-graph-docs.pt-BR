---
title: Obter androidForWorkGeneralDeviceConfiguration
description: Leia as propriedades e as relações do objeto androidForWorkGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a6f5cbfcde976abe180ea157c522a05e081fa84a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39928816"
---
# <a name="get-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="8bcc0-103">Obter androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8bcc0-103">Get androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="8bcc0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8bcc0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bcc0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8bcc0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bcc0-106">Leia as propriedades e as relações do objeto [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8bcc0-106">Read properties and relationships of the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bcc0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8bcc0-107">Prerequisites</span></span>
<span data-ttu-id="8bcc0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bcc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bcc0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bcc0-110">Permission type</span></span>|<span data-ttu-id="8bcc0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8bcc0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bcc0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bcc0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8bcc0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bcc0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8bcc0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bcc0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bcc0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bcc0-115">Not supported.</span></span>|
|<span data-ttu-id="8bcc0-116">Application</span><span class="sxs-lookup"><span data-stu-id="8bcc0-116">Application</span></span>|<span data-ttu-id="8bcc0-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bcc0-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bcc0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bcc0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8bcc0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8bcc0-119">Optional query parameters</span></span>
<span data-ttu-id="8bcc0-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8bcc0-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8bcc0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bcc0-121">Request headers</span></span>
|<span data-ttu-id="8bcc0-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8bcc0-122">Header</span></span>|<span data-ttu-id="8bcc0-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8bcc0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bcc0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bcc0-124">Authorization</span></span>|<span data-ttu-id="8bcc0-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bcc0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bcc0-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8bcc0-126">Accept</span></span>|<span data-ttu-id="8bcc0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8bcc0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bcc0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bcc0-128">Request body</span></span>
<span data-ttu-id="8bcc0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8bcc0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bcc0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bcc0-130">Response</span></span>
<span data-ttu-id="8bcc0-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bcc0-131">If successful, this method returns a `200 OK` response code and [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bcc0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bcc0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bcc0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bcc0-133">Request</span></span>
<span data-ttu-id="8bcc0-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bcc0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8bcc0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bcc0-135">Response</span></span>
<span data-ttu-id="8bcc0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8bcc0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3244

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
    "id": "a931a366-a366-a931-66a3-31a966a331a9",
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
}
```





