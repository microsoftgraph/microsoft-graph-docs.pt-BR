---
title: Listar windows10EndpointProtectionConfigurations
description: Listar propriedades e relações dos objetos windows10EndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2142f8d3146f00106537aa13c18b4033e8c33b4a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467425"
---
# <a name="list-windows10endpointprotectionconfigurations"></a><span data-ttu-id="df54a-103">Listar windows10EndpointProtectionConfigurations</span><span class="sxs-lookup"><span data-stu-id="df54a-103">List windows10EndpointProtectionConfigurations</span></span>

<span data-ttu-id="df54a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df54a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df54a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df54a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df54a-106">Listar propriedades e relações dos objetos [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df54a-106">List properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df54a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df54a-107">Prerequisites</span></span>
<span data-ttu-id="df54a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df54a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df54a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df54a-110">Permission type</span></span>|<span data-ttu-id="df54a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df54a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df54a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df54a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df54a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="df54a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="df54a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df54a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df54a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df54a-115">Not supported.</span></span>|
|<span data-ttu-id="df54a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df54a-116">Application</span></span>|<span data-ttu-id="df54a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df54a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df54a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df54a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="df54a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df54a-119">Request headers</span></span>
|<span data-ttu-id="df54a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df54a-120">Header</span></span>|<span data-ttu-id="df54a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="df54a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df54a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="df54a-122">Authorization</span></span>|<span data-ttu-id="df54a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df54a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df54a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df54a-124">Accept</span></span>|<span data-ttu-id="df54a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df54a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df54a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df54a-126">Request body</span></span>
<span data-ttu-id="df54a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df54a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df54a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="df54a-128">Response</span></span>
<span data-ttu-id="df54a-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df54a-129">If successful, this method returns a `200 OK` response code and a collection of [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df54a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df54a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="df54a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df54a-131">Request</span></span>
<span data-ttu-id="df54a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df54a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="df54a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="df54a-133">Response</span></span>
<span data-ttu-id="df54a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df54a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4834

{
  "value": [
    {
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
  ]
}
```






