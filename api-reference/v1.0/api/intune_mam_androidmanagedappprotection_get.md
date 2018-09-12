# <a name="get-androidmanagedappprotection"></a><span data-ttu-id="6aa1e-101">Get androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="6aa1e-101">Get androidManagedAppProtection</span></span>

> <span data-ttu-id="6aa1e-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6aa1e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6aa1e-103">Ler propriedades e relações do objeto [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="6aa1e-103">Read properties and relationships of the [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6aa1e-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6aa1e-104">Prerequisites</span></span>
<span data-ttu-id="6aa1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6aa1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6aa1e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6aa1e-107">Permission type</span></span>|<span data-ttu-id="6aa1e-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6aa1e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aa1e-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6aa1e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6aa1e-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6aa1e-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6aa1e-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6aa1e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aa1e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6aa1e-112">Not supported.</span></span>|
|<span data-ttu-id="6aa1e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6aa1e-113">Application</span></span>|<span data-ttu-id="6aa1e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6aa1e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aa1e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6aa1e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6aa1e-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6aa1e-116">Optional query parameters</span></span>
<span data-ttu-id="6aa1e-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6aa1e-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6aa1e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6aa1e-118">Request headers</span></span>
|<span data-ttu-id="6aa1e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6aa1e-119">Header</span></span>|<span data-ttu-id="6aa1e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6aa1e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aa1e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6aa1e-121">Authorization</span></span>|<span data-ttu-id="6aa1e-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="6aa1e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6aa1e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6aa1e-123">Accept</span></span>|<span data-ttu-id="6aa1e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6aa1e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aa1e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6aa1e-125">Request body</span></span>
<span data-ttu-id="6aa1e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6aa1e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6aa1e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aa1e-127">Response</span></span>
<span data-ttu-id="6aa1e-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6aa1e-128">If successful, this method returns a `200 OK` response code and [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aa1e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6aa1e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6aa1e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6aa1e-130">Request</span></span>
<span data-ttu-id="6aa1e-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6aa1e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="6aa1e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aa1e-132">Response</span></span>
<span data-ttu-id="6aa1e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6aa1e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1967

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
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
    "screenCaptureBlocked": true,
    "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
    "encryptAppData": true,
    "deployedAppCount": 0,
    "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
    "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
  }
}
```








