# <a name="get-windows10endpointprotectionconfiguration"></a><span data-ttu-id="36ad2-101">Get windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="36ad2-101">Get windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="36ad2-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="36ad2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36ad2-103">Ler propriedades e relações do objeto [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36ad2-103">Read properties and relationships of [plannerBucketTaskBoardTaskFormat](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36ad2-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="36ad2-104">Prerequisites</span></span>
<span data-ttu-id="36ad2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="36ad2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="36ad2-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36ad2-107">Permission type</span></span>|<span data-ttu-id="36ad2-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="36ad2-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36ad2-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36ad2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="36ad2-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="36ad2-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="36ad2-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36ad2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36ad2-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36ad2-112">Not supported.</span></span>|
|<span data-ttu-id="36ad2-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36ad2-113">Application</span></span>|<span data-ttu-id="36ad2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36ad2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36ad2-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36ad2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36ad2-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36ad2-116">Optional query parameters</span></span>
<span data-ttu-id="36ad2-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36ad2-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="36ad2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36ad2-118">Request headers</span></span>
|<span data-ttu-id="36ad2-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36ad2-119">Header</span></span>|<span data-ttu-id="36ad2-120">Valor</span><span class="sxs-lookup"><span data-stu-id="36ad2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36ad2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="36ad2-121">Authorization</span></span>|<span data-ttu-id="36ad2-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36ad2-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="36ad2-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="36ad2-123">Accept</span></span>|<span data-ttu-id="36ad2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="36ad2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36ad2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36ad2-125">Request body</span></span>
<span data-ttu-id="36ad2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36ad2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36ad2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="36ad2-127">Response</span></span>
<span data-ttu-id="36ad2-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36ad2-128">If successful, this method returns a `200 OK` response code and a [section](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36ad2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36ad2-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="36ad2-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36ad2-130">Request</span></span>
<span data-ttu-id="36ad2-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36ad2-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="36ad2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="36ad2-132">Response</span></span>
<span data-ttu-id="36ad2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36ad2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



