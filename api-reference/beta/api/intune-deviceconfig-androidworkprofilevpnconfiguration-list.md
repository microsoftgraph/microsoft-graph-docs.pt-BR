---
title: Listar androidWorkProfileVpnConfigurations
description: Listar Propriedades e relações dos objetos androidWorkProfileVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10f2fe70b5e205e1b91b7f6487384d86d24c5de0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722778"
---
# <a name="list-androidworkprofilevpnconfigurations"></a><span data-ttu-id="662bf-103">Listar androidWorkProfileVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="662bf-103">List androidWorkProfileVpnConfigurations</span></span>

<span data-ttu-id="662bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="662bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="662bf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="662bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="662bf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="662bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="662bf-107">Listar Propriedades e relações dos objetos [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="662bf-107">List properties and relationships of the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="662bf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="662bf-108">Prerequisites</span></span>
<span data-ttu-id="662bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="662bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="662bf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="662bf-111">Permission type</span></span>|<span data-ttu-id="662bf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="662bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="662bf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="662bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="662bf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="662bf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="662bf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="662bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="662bf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="662bf-116">Not supported.</span></span>|
|<span data-ttu-id="662bf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="662bf-117">Application</span></span>|<span data-ttu-id="662bf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="662bf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="662bf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="662bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="662bf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="662bf-120">Request headers</span></span>
|<span data-ttu-id="662bf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="662bf-121">Header</span></span>|<span data-ttu-id="662bf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="662bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="662bf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="662bf-123">Authorization</span></span>|<span data-ttu-id="662bf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="662bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="662bf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="662bf-125">Accept</span></span>|<span data-ttu-id="662bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="662bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="662bf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="662bf-127">Request body</span></span>
<span data-ttu-id="662bf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="662bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="662bf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="662bf-129">Response</span></span>
<span data-ttu-id="662bf-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="662bf-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="662bf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="662bf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="662bf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="662bf-132">Request</span></span>
<span data-ttu-id="662bf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="662bf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="662bf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="662bf-134">Response</span></span>
<span data-ttu-id="662bf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="662bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2951

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
      "id": "32910378-0378-3291-7803-913278039132",
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
      "connectionName": "Connection Name value",
      "connectionType": "pulseSecure",
      "role": "Role value",
      "realm": "Realm value",
      "servers": [
        {
          "@odata.type": "microsoft.graph.vpnServer",
          "description": "Description value",
          "address": "Address value",
          "isDefaultServer": true
        }
      ],
      "fingerprint": "Fingerprint value",
      "customData": [
        {
          "@odata.type": "microsoft.graph.keyValue",
          "key": "Key value",
          "value": "Value value"
        }
      ],
      "customKeyValueData": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "authenticationMethod": "usernameAndPassword",
      "proxyServer": {
        "@odata.type": "microsoft.graph.vpnProxyServer",
        "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
        "address": "Address value",
        "port": 4
      },
      "targetedPackageIds": [
        "Targeted Package Ids value"
      ],
      "targetedMobileApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "alwaysOn": true,
      "alwaysOnLockdown": true,
      "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
    }
  ]
}
```





