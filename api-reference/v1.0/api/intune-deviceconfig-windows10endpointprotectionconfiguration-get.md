---
title: Get windows10EndpointProtectionConfiguration
description: Ler propriedades e relações do objeto windows10EndpointProtectionConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1965bf36dea19e91e07e3301d1bcf5ae184216f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514102"
---
# <a name="get-windows10endpointprotectionconfiguration"></a><span data-ttu-id="bffeb-103">Get windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="bffeb-103">Get windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="bffeb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bffeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bffeb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bffeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bffeb-106">Ler propriedades e relações do objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bffeb-106">Read properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bffeb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bffeb-107">Prerequisites</span></span>
<span data-ttu-id="bffeb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bffeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bffeb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bffeb-110">Permission type</span></span>|<span data-ttu-id="bffeb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bffeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bffeb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bffeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bffeb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bffeb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bffeb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bffeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bffeb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bffeb-115">Not supported.</span></span>|
|<span data-ttu-id="bffeb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bffeb-116">Application</span></span>|<span data-ttu-id="bffeb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bffeb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bffeb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bffeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bffeb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bffeb-119">Optional query parameters</span></span>
<span data-ttu-id="bffeb-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bffeb-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bffeb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bffeb-121">Request headers</span></span>
|<span data-ttu-id="bffeb-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bffeb-122">Header</span></span>|<span data-ttu-id="bffeb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="bffeb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bffeb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bffeb-124">Authorization</span></span>|<span data-ttu-id="bffeb-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bffeb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bffeb-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bffeb-126">Accept</span></span>|<span data-ttu-id="bffeb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bffeb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bffeb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bffeb-128">Request body</span></span>
<span data-ttu-id="bffeb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bffeb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bffeb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bffeb-130">Response</span></span>
<span data-ttu-id="bffeb-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bffeb-131">If successful, this method returns a `200 OK` response code and [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bffeb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bffeb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bffeb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bffeb-133">Request</span></span>
<span data-ttu-id="bffeb-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bffeb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="bffeb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="bffeb-135">Response</span></span>
<span data-ttu-id="bffeb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bffeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4628

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
    "id": "09709403-9403-0970-0394-700903947009",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "firewallBlockStatefulFTP": true,
    "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
    "firewallPreSharedKeyEncodingMethod": "none",
    "firewallIPSecExemptionsAllowNeighborDiscovery": true,
    "firewallIPSecExemptionsAllowICMP": true,
    "firewallIPSecExemptionsAllowRouterDiscovery": true,
    "firewallIPSecExemptionsAllowDHCP": true,
    "firewallCertificateRevocationListCheckMethod": "none",
    "firewallMergeKeyingModuleSettings": true,
    "firewallPacketQueueingMethod": "disabled",
    "firewallProfileDomain": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeBlocked": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "policyRulesFromGroupPolicyMerged": true
    },
    "firewallProfilePublic": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeBlocked": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "policyRulesFromGroupPolicyMerged": true
    },
    "firewallProfilePrivate": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeBlocked": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "policyRulesFromGroupPolicyMerged": true
    },
    "defenderAttackSurfaceReductionExcludedPaths": [
      "Defender Attack Surface Reduction Excluded Paths value"
    ],
    "defenderGuardedFoldersAllowedAppPaths": [
      "Defender Guarded Folders Allowed App Paths value"
    ],
    "defenderAdditionalGuardedFolders": [
      "Defender Additional Guarded Folders value"
    ],
    "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
    "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
    "defenderSecurityCenterBlockExploitProtectionOverride": true,
    "appLockerApplicationControl": "enforceComponentsAndStoreApps",
    "smartScreenEnableInShell": true,
    "smartScreenBlockOverrideForFiles": true,
    "applicationGuardEnabled": true,
    "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
    "applicationGuardBlockNonEnterpriseContent": true,
    "applicationGuardAllowPersistence": true,
    "applicationGuardForceAuditing": true,
    "applicationGuardBlockClipboardSharing": "blockBoth",
    "applicationGuardAllowPrintToPDF": true,
    "applicationGuardAllowPrintToXPS": true,
    "applicationGuardAllowPrintToLocalPrinters": true,
    "applicationGuardAllowPrintToNetworkPrinters": true,
    "bitLockerDisableWarningForOtherDiskEncryption": true,
    "bitLockerEnableStorageCardEncryptionOnMobile": true,
    "bitLockerEncryptDevice": true,
    "bitLockerRemovableDrivePolicy": {
      "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
      "encryptionMethod": "aesCbc256",
      "requireEncryptionForWriteAccess": true,
      "blockCrossOrganizationWriteAccess": true
    }
  }
}
```




