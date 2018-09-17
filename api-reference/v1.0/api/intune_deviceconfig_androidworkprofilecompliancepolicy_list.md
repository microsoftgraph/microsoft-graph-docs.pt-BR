# <a name="list-androidworkprofilecompliancepolicies"></a><span data-ttu-id="89b2a-101">Lista androidWorkProfileCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="89b2a-101">List androidWorkProfileCompliancePolicies</span></span>

> <span data-ttu-id="89b2a-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="89b2a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89b2a-103">Propriedades de lista e relacionamentos dos objetos [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="89b2a-103">List properties and relationships of the [deviceCategory](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89b2a-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89b2a-104">Prerequisites</span></span>
<span data-ttu-id="89b2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="89b2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="89b2a-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89b2a-107">Permission type</span></span>|<span data-ttu-id="89b2a-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89b2a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89b2a-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89b2a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="89b2a-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89b2a-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="89b2a-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89b2a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89b2a-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89b2a-112">Not supported.</span></span>|
|<span data-ttu-id="89b2a-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89b2a-113">Application</span></span>|<span data-ttu-id="89b2a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89b2a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89b2a-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89b2a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="89b2a-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89b2a-116">Request headers</span></span>
|<span data-ttu-id="89b2a-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89b2a-117">Header</span></span>|<span data-ttu-id="89b2a-118">Valor</span><span class="sxs-lookup"><span data-stu-id="89b2a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89b2a-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="89b2a-119">Authorization</span></span>|<span data-ttu-id="89b2a-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="89b2a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89b2a-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="89b2a-121">Accept</span></span>|<span data-ttu-id="89b2a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="89b2a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89b2a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89b2a-123">Request body</span></span>
<span data-ttu-id="89b2a-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="89b2a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89b2a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="89b2a-125">Response</span></span>
<span data-ttu-id="89b2a-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89b2a-126">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89b2a-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89b2a-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="89b2a-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89b2a-128">Request</span></span>
<span data-ttu-id="89b2a-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89b2a-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="89b2a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="89b2a-130">Response</span></span>
<span data-ttu-id="89b2a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89b2a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1487

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
      "id": "4e385271-5271-4e38-7152-384e7152384e",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordMinimumLength": 5,
      "passwordRequiredType": "alphabetic",
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordPreviousPasswordBlockCount": 2,
      "securityPreventInstallAppsFromUnknownSources": true,
      "securityDisableUsbDebugging": true,
      "securityRequireVerifyApps": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "securityBlockJailbrokenDevices": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
      "storageRequireEncryption": true,
      "securityRequireSafetyNetAttestationBasicIntegrity": true,
      "securityRequireSafetyNetAttestationCertifiedDevice": true,
      "securityRequireGooglePlayServices": true,
      "securityRequireUpToDateSecurityProviders": true,
      "securityRequireCompanyPortalAppIntegrity": true
    }
  ]
}
```








