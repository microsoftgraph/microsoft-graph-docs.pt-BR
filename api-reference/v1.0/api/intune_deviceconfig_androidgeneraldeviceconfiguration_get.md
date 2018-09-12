# <a name="get-androidgeneraldeviceconfiguration"></a><span data-ttu-id="7fdef-101">Acessar androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="7fdef-101">Get androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="7fdef-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7fdef-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fdef-103">Leia as propriedades e relações do objeto [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7fdef-103">Read properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7fdef-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7fdef-104">Prerequisites</span></span>
<span data-ttu-id="7fdef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7fdef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7fdef-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fdef-107">Permission type</span></span>|<span data-ttu-id="7fdef-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7fdef-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fdef-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fdef-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7fdef-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fdef-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7fdef-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fdef-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fdef-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fdef-112">Not supported.</span></span>|
|<span data-ttu-id="7fdef-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fdef-113">Application</span></span>|<span data-ttu-id="7fdef-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fdef-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fdef-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fdef-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7fdef-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7fdef-116">Optional query parameters</span></span>
<span data-ttu-id="7fdef-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7fdef-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7fdef-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fdef-118">Request headers</span></span>
|<span data-ttu-id="7fdef-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7fdef-119">Header</span></span>|<span data-ttu-id="7fdef-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7fdef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fdef-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fdef-121">Authorization</span></span>|<span data-ttu-id="7fdef-122">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="7fdef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fdef-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7fdef-123">Accept</span></span>|<span data-ttu-id="7fdef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7fdef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fdef-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fdef-125">Request body</span></span>
<span data-ttu-id="7fdef-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7fdef-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fdef-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fdef-127">Response</span></span>
<span data-ttu-id="7fdef-128">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fdef-128">If successful, this method returns a `200 OK` response code and [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fdef-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fdef-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="7fdef-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fdef-130">Request</span></span>
<span data-ttu-id="7fdef-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fdef-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="7fdef-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fdef-132">Response</span></span>
<span data-ttu-id="7fdef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fdef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3414

{
  "value": {
    "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
    "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "appsBlockClipboardSharing": true,
    "appsBlockCopyPaste": true,
    "appsBlockYouTube": true,
    "bluetoothBlocked": true,
    "cameraBlocked": true,
    "cellularBlockDataRoaming": true,
    "cellularBlockMessaging": true,
    "cellularBlockVoiceRoaming": true,
    "cellularBlockWiFiTethering": true,
    "compliantAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "compliantAppListType": "appsInListCompliant",
    "diagnosticDataBlockSubmission": true,
    "locationServicesBlocked": true,
    "googleAccountBlockAutoSync": true,
    "googlePlayStoreBlocked": true,
    "kioskModeBlockSleepButton": true,
    "kioskModeBlockVolumeButtons": true,
    "kioskModeApps": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "nfcBlocked": true,
    "passwordBlockFingerprintUnlock": true,
    "passwordBlockTrustAgents": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "passwordRequiredType": "alphabetic",
    "passwordRequired": true,
    "powerOffBlocked": true,
    "factoryResetBlocked": true,
    "screenCaptureBlocked": true,
    "deviceSharingAllowed": true,
    "storageBlockGoogleBackup": true,
    "storageBlockRemovableStorage": true,
    "storageRequireDeviceEncryption": true,
    "storageRequireRemovableStorageEncryption": true,
    "voiceAssistantBlocked": true,
    "voiceDialingBlocked": true,
    "webBrowserBlockPopups": true,
    "webBrowserBlockAutofill": true,
    "webBrowserBlockJavaScript": true,
    "webBrowserBlocked": true,
    "webBrowserCookieSettings": "blockAlways",
    "wiFiBlocked": true,
    "appsInstallAllowList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "appsLaunchBlockList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "appsHideList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "securityRequireVerifyApps": true
  }
}
```








