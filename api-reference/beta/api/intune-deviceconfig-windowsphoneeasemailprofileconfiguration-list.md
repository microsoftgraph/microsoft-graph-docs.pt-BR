---
title: Listar windowsPhoneEASEmailProfileConfigurations
description: Listar Propriedades e relações dos objetos windowsPhoneEASEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe45a7a101fe68313f617715226338453f944cc8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961466"
---
# <a name="list-windowsphoneeasemailprofileconfigurations"></a><span data-ttu-id="48790-103">Listar windowsPhoneEASEmailProfileConfigurations</span><span class="sxs-lookup"><span data-stu-id="48790-103">List windowsPhoneEASEmailProfileConfigurations</span></span>

> <span data-ttu-id="48790-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48790-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48790-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48790-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48790-106">Listar Propriedades e relações dos objetos [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="48790-106">List properties and relationships of the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48790-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="48790-107">Prerequisites</span></span>
<span data-ttu-id="48790-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48790-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48790-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48790-110">Permission type</span></span>|<span data-ttu-id="48790-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="48790-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48790-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48790-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48790-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="48790-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="48790-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48790-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48790-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48790-115">Not supported.</span></span>|
|<span data-ttu-id="48790-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48790-116">Application</span></span>|<span data-ttu-id="48790-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48790-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48790-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48790-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="48790-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48790-119">Request headers</span></span>
|<span data-ttu-id="48790-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48790-120">Header</span></span>|<span data-ttu-id="48790-121">Valor</span><span class="sxs-lookup"><span data-stu-id="48790-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48790-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="48790-122">Authorization</span></span>|<span data-ttu-id="48790-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48790-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48790-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="48790-124">Accept</span></span>|<span data-ttu-id="48790-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48790-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48790-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48790-126">Request body</span></span>
<span data-ttu-id="48790-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48790-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48790-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="48790-128">Response</span></span>
<span data-ttu-id="48790-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48790-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48790-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48790-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="48790-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48790-131">Request</span></span>
<span data-ttu-id="48790-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48790-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="48790-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="48790-133">Response</span></span>
<span data-ttu-id="48790-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48790-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1956

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
      "id": "554f402a-402a-554f-2a40-4f552a404f55",
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
      "applyOnlyToWindowsPhone81": true,
      "syncCalendar": true,
      "syncContacts": true,
      "syncTasks": true,
      "durationOfEmailToSync": "oneDay",
      "emailAddressSource": "primarySmtpAddress",
      "emailSyncSchedule": "asMessagesArrive",
      "hostName": "Host Name value",
      "requireSsl": true
    }
  ]
}
```





