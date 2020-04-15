---
title: Acessar windowsInformationProtection
description: Leia as propriedades e as relações do objeto windowsInformationProtection.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fa03ebdbef0adcce6b1784f3ce6cfc5e7eab933c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43418622"
---
# <a name="get-windowsinformationprotection"></a><span data-ttu-id="a7c66-103">Acessar windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="a7c66-103">Get windowsInformationProtection</span></span>

<span data-ttu-id="a7c66-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7c66-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7c66-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a7c66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7c66-106">Leia as propriedades e as relações do objeto [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="a7c66-106">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7c66-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a7c66-107">Prerequisites</span></span>
<span data-ttu-id="a7c66-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7c66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7c66-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7c66-110">Permission type</span></span>|<span data-ttu-id="a7c66-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a7c66-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7c66-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7c66-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a7c66-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7c66-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a7c66-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7c66-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7c66-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7c66-115">Not supported.</span></span>|
|<span data-ttu-id="a7c66-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7c66-116">Application</span></span>|<span data-ttu-id="a7c66-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7c66-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7c66-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7c66-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7c66-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a7c66-119">Optional query parameters</span></span>
<span data-ttu-id="a7c66-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a7c66-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7c66-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7c66-121">Request headers</span></span>
|<span data-ttu-id="a7c66-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7c66-122">Header</span></span>|<span data-ttu-id="a7c66-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a7c66-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7c66-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7c66-124">Authorization</span></span>|<span data-ttu-id="a7c66-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7c66-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7c66-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a7c66-126">Accept</span></span>|<span data-ttu-id="a7c66-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a7c66-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7c66-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7c66-128">Request body</span></span>
<span data-ttu-id="a7c66-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7c66-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7c66-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7c66-130">Response</span></span>
<span data-ttu-id="a7c66-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7c66-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7c66-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7c66-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7c66-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7c66-133">Request</span></span>
<span data-ttu-id="a7c66-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7c66-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="a7c66-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7c66-135">Response</span></span>
<span data-ttu-id="a7c66-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7c66-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4337

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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






