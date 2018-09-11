# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="d2b3b-101">Obter iosManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="d2b3b-101">Get iosManagedAppProtection</span></span>

> <span data-ttu-id="d2b3b-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d2b3b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2b3b-103">Ler propriedades e relações do objeto [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d2b3b-103">Read properties and relationships of the [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2b3b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d2b3b-104">Prerequisites</span></span>
<span data-ttu-id="d2b3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d2b3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d2b3b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2b3b-107">Permission type</span></span>|<span data-ttu-id="d2b3b-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d2b3b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2b3b-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2b3b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d2b3b-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2b3b-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d2b3b-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2b3b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2b3b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2b3b-112">Not supported.</span></span>|
|<span data-ttu-id="d2b3b-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2b3b-113">Application</span></span>|<span data-ttu-id="d2b3b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2b3b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2b3b-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2b3b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2b3b-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d2b3b-116">Optional query parameters</span></span>
<span data-ttu-id="d2b3b-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d2b3b-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d2b3b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2b3b-118">Request headers</span></span>
|<span data-ttu-id="d2b3b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2b3b-119">Header</span></span>|<span data-ttu-id="d2b3b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d2b3b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2b3b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2b3b-121">Authorization</span></span>|<span data-ttu-id="d2b3b-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="d2b3b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2b3b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d2b3b-123">Accept</span></span>|<span data-ttu-id="d2b3b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d2b3b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2b3b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2b3b-125">Request body</span></span>
<span data-ttu-id="d2b3b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2b3b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2b3b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2b3b-127">Response</span></span>
<span data-ttu-id="d2b3b-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2b3b-128">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2b3b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2b3b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2b3b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2b3b-130">Request</span></span>
<span data-ttu-id="d2b3b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2b3b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="d2b3b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2b3b-132">Response</span></span>
<span data-ttu-id="d2b3b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2b3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1839

{
  "value": {
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
}
```








