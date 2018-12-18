---
title: Listar windows10EndpointProtectionConfigurations
description: Listar propriedades e relações dos objetos windows10EndpointProtectionConfiguration.
author: tfitzmac
ms.openlocfilehash: 0435cbb3edb3a0f4ce94a71fa019fd3f982c25c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323041"
---
# <a name="list-windows10endpointprotectionconfigurations"></a><span data-ttu-id="a86aa-103">Listar windows10EndpointProtectionConfigurations</span><span class="sxs-lookup"><span data-stu-id="a86aa-103">List windows10EndpointProtectionConfigurations</span></span>

> <span data-ttu-id="a86aa-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a86aa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a86aa-105">Listar propriedades e relações dos objetos [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a86aa-105">List properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a86aa-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a86aa-106">Prerequisites</span></span>
<span data-ttu-id="a86aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a86aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a86aa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a86aa-109">Permission type</span></span>|<span data-ttu-id="a86aa-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a86aa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a86aa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a86aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a86aa-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a86aa-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a86aa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a86aa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a86aa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a86aa-114">Not supported.</span></span>|
|<span data-ttu-id="a86aa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a86aa-115">Application</span></span>|<span data-ttu-id="a86aa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a86aa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a86aa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a86aa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a86aa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a86aa-118">Request headers</span></span>
|<span data-ttu-id="a86aa-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a86aa-119">Header</span></span>|<span data-ttu-id="a86aa-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a86aa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a86aa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a86aa-121">Authorization</span></span>|<span data-ttu-id="a86aa-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a86aa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a86aa-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a86aa-123">Accept</span></span>|<span data-ttu-id="a86aa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a86aa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a86aa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a86aa-125">Request body</span></span>
<span data-ttu-id="a86aa-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a86aa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a86aa-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a86aa-127">Response</span></span>
<span data-ttu-id="a86aa-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a86aa-128">If successful, this method returns a `200 OK` response code and a collection of [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a86aa-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a86aa-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a86aa-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a86aa-130">Request</span></span>
<span data-ttu-id="a86aa-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a86aa-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a86aa-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a86aa-132">Response</span></span>
<span data-ttu-id="a86aa-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a86aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



