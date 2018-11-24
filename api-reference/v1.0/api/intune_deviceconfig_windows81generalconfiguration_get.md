# <a name="get-windows81generalconfiguration"></a><span data-ttu-id="edc55-101">Obter windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="edc55-101">Get windows81GeneralConfiguration</span></span>

> <span data-ttu-id="edc55-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="edc55-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="edc55-103">Ler propriedades e relações do objeto [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edc55-103">Read properties and relationships of the [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="edc55-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="edc55-104">Prerequisites</span></span>
<span data-ttu-id="edc55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="edc55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="edc55-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="edc55-107">Permission type</span></span>|<span data-ttu-id="edc55-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="edc55-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edc55-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="edc55-109">Delegated (work or school account)</span></span>|<span data-ttu-id="edc55-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="edc55-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="edc55-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="edc55-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edc55-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="edc55-112">Not supported.</span></span>|
|<span data-ttu-id="edc55-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="edc55-113">Application</span></span>|<span data-ttu-id="edc55-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="edc55-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="edc55-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="edc55-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="edc55-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="edc55-116">Optional query parameters</span></span>
<span data-ttu-id="edc55-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="edc55-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="edc55-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="edc55-118">Request headers</span></span>
|<span data-ttu-id="edc55-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="edc55-119">Header</span></span>|<span data-ttu-id="edc55-120">Valor</span><span class="sxs-lookup"><span data-stu-id="edc55-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edc55-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="edc55-121">Authorization</span></span>|<span data-ttu-id="edc55-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edc55-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edc55-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="edc55-123">Accept</span></span>|<span data-ttu-id="edc55-124">application/json</span><span class="sxs-lookup"><span data-stu-id="edc55-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edc55-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="edc55-125">Request body</span></span>
<span data-ttu-id="edc55-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="edc55-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edc55-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="edc55-127">Response</span></span>
<span data-ttu-id="edc55-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="edc55-128">If successful, this method returns a `200 OK` response code and [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edc55-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="edc55-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="edc55-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="edc55-130">Request</span></span>
<span data-ttu-id="edc55-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="edc55-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="edc55-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="edc55-132">Response</span></span>
<span data-ttu-id="edc55-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="edc55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1964

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
    "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "accountsBlockAddingNonMicrosoftAccountEmail": true,
    "applyOnlyToWindows81": true,
    "browserBlockAutofill": true,
    "browserBlockAutomaticDetectionOfIntranetSites": true,
    "browserBlockEnterpriseModeAccess": true,
    "browserBlockJavaScript": true,
    "browserBlockPlugins": true,
    "browserBlockPopups": true,
    "browserBlockSendingDoNotTrackHeader": true,
    "browserBlockSingleWordEntryOnIntranetSites": true,
    "browserRequireSmartScreen": true,
    "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
    "browserInternetSecurityLevel": "medium",
    "browserIntranetSecurityLevel": "low",
    "browserLoggingReportLocation": "Browser Logging Report Location value",
    "browserRequireHighSecurityForRestrictedSites": true,
    "browserRequireFirewall": true,
    "browserRequireFraudWarning": true,
    "browserTrustedSitesSecurityLevel": "low",
    "cellularBlockDataRoaming": true,
    "diagnosticsBlockDataSubmission": true,
    "passwordBlockPicturePasswordAndPin": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordMinimumCharacterSetCount": 0,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequiredType": "alphanumeric",
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "storageRequireDeviceEncryption": true,
    "updatesRequireAutomaticUpdates": true,
    "userAccountControlSettings": "alwaysNotify",
    "workFoldersUrl": "https://example.com/workFoldersUrl/"
  }
}
```



