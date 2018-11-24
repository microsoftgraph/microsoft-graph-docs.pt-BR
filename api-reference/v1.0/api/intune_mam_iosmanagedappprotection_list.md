# <a name="list-iosmanagedappprotections"></a><span data-ttu-id="e2550-101">Listar iosManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="e2550-101">List iosManagedAppProtections</span></span>

> <span data-ttu-id="e2550-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e2550-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2550-103">Listar propriedades e relações dos objetos [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="e2550-103">List properties and relationships of the [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e2550-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2550-104">Prerequisites</span></span>
<span data-ttu-id="e2550-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e2550-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e2550-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2550-107">Permission type</span></span>|<span data-ttu-id="e2550-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e2550-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2550-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2550-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e2550-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2550-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e2550-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2550-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2550-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2550-112">Not supported.</span></span>|
|<span data-ttu-id="e2550-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2550-113">Application</span></span>|<span data-ttu-id="e2550-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2550-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2550-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2550-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="e2550-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2550-116">Request headers</span></span>
|<span data-ttu-id="e2550-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2550-117">Header</span></span>|<span data-ttu-id="e2550-118">Valor</span><span class="sxs-lookup"><span data-stu-id="e2550-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2550-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2550-119">Authorization</span></span>|<span data-ttu-id="e2550-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2550-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2550-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e2550-121">Accept</span></span>|<span data-ttu-id="e2550-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e2550-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2550-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2550-123">Request body</span></span>
<span data-ttu-id="e2550-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e2550-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2550-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2550-125">Response</span></span>
<span data-ttu-id="e2550-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2550-126">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2550-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2550-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2550-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2550-128">Request</span></span>
<span data-ttu-id="e2550-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2550-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="e2550-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2550-130">Response</span></span>
<span data-ttu-id="e2550-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2550-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1933

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
      "version": "Version value",
      "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
      "periodOnlineBeforeAccessCheck": "PT35.0018757S",
      "allowedInboundDataTransferSources": "managedApps",
      "allowedOutboundDataTransferDestinations": "managedApps",
      "organizationalCredentialsRequired": true,
      "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
      "dataBackupBlocked": true,
      "deviceComplianceRequired": true,
      "managedBrowserToOpenLinksRequired": true,
      "saveAsBlocked": true,
      "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
      "pinRequired": true,
      "maximumPinRetries": 1,
      "simplePinBlocked": true,
      "minimumPinLength": 0,
      "pinCharacterSet": "alphanumericAndSymbol",
      "periodBeforePinReset": "PT3M29.6631862S",
      "allowedDataStorageLocations": [
        "sharePoint"
      ],
      "contactSyncBlocked": true,
      "printBlocked": true,
      "fingerprintBlocked": true,
      "disableAppPinIfDevicePinIsSet": true,
      "minimumRequiredOsVersion": "Minimum Required Os Version value",
      "minimumWarningOsVersion": "Minimum Warning Os Version value",
      "minimumRequiredAppVersion": "Minimum Required App Version value",
      "minimumWarningAppVersion": "Minimum Warning App Version value",
      "isAssigned": true,
      "appDataEncryptionType": "afterDeviceRestart",
      "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
      "deployedAppCount": 0,
      "faceIdBlocked": true
    }
  ]
}
```



