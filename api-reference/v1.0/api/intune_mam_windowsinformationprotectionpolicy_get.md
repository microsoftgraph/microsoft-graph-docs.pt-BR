# <a name="get-windowsinformationprotectionpolicy"></a><span data-ttu-id="89196-101">Obter windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="89196-101">Get windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="89196-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="89196-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89196-103">Ler propriedades e relações do objeto [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="89196-103">Read properties and relationships of the [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89196-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89196-104">Prerequisites</span></span>
<span data-ttu-id="89196-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="89196-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="89196-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89196-107">Permission type</span></span>|<span data-ttu-id="89196-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89196-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89196-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89196-109">Delegated (work or school account)</span></span>|<span data-ttu-id="89196-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="89196-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="89196-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89196-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89196-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89196-112">Not supported.</span></span>|
|<span data-ttu-id="89196-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89196-113">Application</span></span>|<span data-ttu-id="89196-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89196-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89196-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89196-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89196-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="89196-116">Optional query parameters</span></span>
<span data-ttu-id="89196-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="89196-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="89196-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89196-118">Request headers</span></span>
|<span data-ttu-id="89196-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89196-119">Header</span></span>|<span data-ttu-id="89196-120">Valor</span><span class="sxs-lookup"><span data-stu-id="89196-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89196-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="89196-121">Authorization</span></span>|<span data-ttu-id="89196-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89196-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89196-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="89196-123">Accept</span></span>|<span data-ttu-id="89196-124">application/json</span><span class="sxs-lookup"><span data-stu-id="89196-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89196-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89196-125">Request body</span></span>
<span data-ttu-id="89196-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="89196-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89196-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="89196-127">Response</span></span>
<span data-ttu-id="89196-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89196-128">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89196-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89196-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="89196-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89196-130">Request</span></span>
<span data-ttu-id="89196-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89196-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="89196-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="89196-132">Response</span></span>
<span data-ttu-id="89196-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89196-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4870

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "6397be61-be61-6397-61be-976361be9763",
    "version": "Version value",
    "enforcementLevel": "encryptAndAuditOnly",
    "enterpriseDomain": "Enterprise Domain value",
    "enterpriseProtectedDomainNames": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "protectionUnderLockConfigRequired": true,
    "dataRecoveryCertificate": {
      "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
      "subjectName": "Subject Name value",
      "description": "Description value",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "certificate": "Y2VydGlmaWNhdGU="
    },
    "revokeOnUnenrollDisabled": true,
    "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
    "azureRightsManagementServicesAllowed": true,
    "iconsVisible": true,
    "protectedApps": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
        "displayName": "Display Name value",
        "description": "Description value",
        "publisherName": "Publisher Name value",
        "productName": "Product Name value",
        "denied": true
      }
    ],
    "exemptApps": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
        "displayName": "Display Name value",
        "description": "Description value",
        "publisherName": "Publisher Name value",
        "productName": "Product Name value",
        "denied": true
      }
    ],
    "enterpriseNetworkDomainNames": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "enterpriseProxiedDomains": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
        "displayName": "Display Name value",
        "proxiedDomains": [
          {
            "@odata.type": "microsoft.graph.proxiedDomain",
            "ipAddressOrFQDN": "Ip Address Or FQDN value",
            "proxy": "Proxy value"
          }
        ]
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
        "displayName": "Display Name value",
        "ranges": [
          {
            "@odata.type": "microsoft.graph.iPv6Range",
            "lowerAddress": "Lower Address value",
            "upperAddress": "Upper Address value"
          }
        ]
      }
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "enterpriseInternalProxyServers": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "indexingEncryptedStoresOrItemsBlocked": true,
    "smbAutoEncryptedFileExtensions": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "isAssigned": true,
    "revokeOnMdmHandoffDisabled": true,
    "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
    "windowsHelloForBusinessBlocked": true,
    "pinMinimumLength": 0,
    "pinUppercaseLetters": "requireAtLeastOne",
    "pinLowercaseLetters": "requireAtLeastOne",
    "pinSpecialCharacters": "requireAtLeastOne",
    "pinExpirationDays": 1,
    "numberOfPastPinsRemembered": 10,
    "passwordMaximumAttemptCount": 11,
    "minutesOfInactivityBeforeDeviceLock": 3,
    "daysWithoutContactBeforeUnenroll": 0
  }
}
```



