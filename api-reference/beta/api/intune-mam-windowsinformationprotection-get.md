---
title: Acessar windowsInformationProtection
description: Leia as propriedades e as relações do objeto windowsInformationProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8f8b2aad18a525d3b419055f32e2f8f9f812762a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463024"
---
# <a name="get-windowsinformationprotection"></a><span data-ttu-id="d3fb2-103">Acessar windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="d3fb2-103">Get windowsInformationProtection</span></span>

<span data-ttu-id="d3fb2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d3fb2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3fb2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3fb2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3fb2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3fb2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3fb2-107">Leia as propriedades e as relações do objeto [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d3fb2-107">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3fb2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3fb2-108">Prerequisites</span></span>
<span data-ttu-id="d3fb2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3fb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3fb2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3fb2-111">Permission type</span></span>|<span data-ttu-id="d3fb2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3fb2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3fb2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3fb2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3fb2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3fb2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d3fb2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3fb2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3fb2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3fb2-116">Not supported.</span></span>|
|<span data-ttu-id="d3fb2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3fb2-117">Application</span></span>|<span data-ttu-id="d3fb2-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3fb2-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3fb2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3fb2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3fb2-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d3fb2-120">Optional query parameters</span></span>
<span data-ttu-id="d3fb2-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d3fb2-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3fb2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3fb2-122">Request headers</span></span>
|<span data-ttu-id="d3fb2-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3fb2-123">Header</span></span>|<span data-ttu-id="d3fb2-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d3fb2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3fb2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3fb2-125">Authorization</span></span>|<span data-ttu-id="d3fb2-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3fb2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3fb2-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3fb2-127">Accept</span></span>|<span data-ttu-id="d3fb2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d3fb2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3fb2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3fb2-129">Request body</span></span>
<span data-ttu-id="d3fb2-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3fb2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3fb2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3fb2-131">Response</span></span>
<span data-ttu-id="d3fb2-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3fb2-132">If successful, this method returns a `200 OK` response code and [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3fb2-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3fb2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3fb2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3fb2-134">Request</span></span>
<span data-ttu-id="d3fb2-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3fb2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="d3fb2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3fb2-136">Response</span></span>
<span data-ttu-id="d3fb2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3fb2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4405

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "ca339419-9419-ca33-1994-33ca199433ca",
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
    "isAssigned": true
  }
}
```





