---
title: Listar iosEasEmailProfileConfigurations
description: Listar Propriedades e relações dos objetos iosEasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 19a44d1056c8c1be18e2dde93741f9c499848765
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35948479"
---
# <a name="list-ioseasemailprofileconfigurations"></a><span data-ttu-id="9fc81-103">Listar iosEasEmailProfileConfigurations</span><span class="sxs-lookup"><span data-stu-id="9fc81-103">List iosEasEmailProfileConfigurations</span></span>

> <span data-ttu-id="9fc81-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9fc81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fc81-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9fc81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fc81-106">Listar Propriedades e relações dos objetos [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9fc81-106">List properties and relationships of the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fc81-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9fc81-107">Prerequisites</span></span>
<span data-ttu-id="9fc81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fc81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fc81-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fc81-110">Permission type</span></span>|<span data-ttu-id="9fc81-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9fc81-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fc81-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fc81-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9fc81-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fc81-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9fc81-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fc81-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fc81-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fc81-115">Not supported.</span></span>|
|<span data-ttu-id="9fc81-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fc81-116">Application</span></span>|<span data-ttu-id="9fc81-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fc81-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fc81-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fc81-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9fc81-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fc81-119">Request headers</span></span>
|<span data-ttu-id="9fc81-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9fc81-120">Header</span></span>|<span data-ttu-id="9fc81-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9fc81-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fc81-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fc81-122">Authorization</span></span>|<span data-ttu-id="9fc81-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fc81-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fc81-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9fc81-124">Accept</span></span>|<span data-ttu-id="9fc81-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9fc81-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fc81-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fc81-126">Request body</span></span>
<span data-ttu-id="9fc81-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9fc81-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fc81-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fc81-128">Response</span></span>
<span data-ttu-id="9fc81-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fc81-129">If successful, this method returns a `200 OK` response code and a collection of [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fc81-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fc81-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fc81-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fc81-131">Request</span></span>
<span data-ttu-id="9fc81-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fc81-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9fc81-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fc81-133">Response</span></span>
<span data-ttu-id="9fc81-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fc81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
      "id": "e03086da-86da-e030-da86-30e0da8630e0",
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
      "usernameSource": "primarySmtpAddress",
      "usernameAADSource": "primarySmtpAddress",
      "userDomainNameSource": "netBiosDomainName",
      "customDomainName": "Custom Domain Name value",
      "accountName": "Account Name value",
      "authenticationMethod": "certificate",
      "blockMovingMessagesToOtherEmailAccounts": true,
      "blockSendingEmailFromThirdPartyApps": true,
      "blockSyncingRecentlyUsedEmailAddresses": true,
      "durationOfEmailToSync": "oneDay",
      "emailAddressSource": "primarySmtpAddress",
      "hostName": "Host Name value",
      "requireSmime": true,
      "smimeEnablePerMessageSwitch": true,
      "smimeEncryptByDefaultEnabled": true,
      "smimeSigningEnabled": true,
      "smimeSigningUserOverrideEnabled": true,
      "smimeEncryptByDefaultUserOverrideEnabled": true,
      "smimeSigningCertificateUserOverrideEnabled": true,
      "smimeEncryptionCertificateUserOverrideEnabled": true,
      "requireSsl": true,
      "useOAuth": true,
      "signingCertificateType": "certificate",
      "encryptionCertificateType": "certificate"
    }
  ]
}
```





