---
title: Listar windowsInformationProtections
description: Listar propriedades e relações dos objetos windowsInformationProtection.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0622ab68ac9ec4635048ec6c12e2d1c3171bef20
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447836"
---
# <a name="list-windowsinformationprotections"></a><span data-ttu-id="9bf56-103">Listar windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="9bf56-103">List windowsInformationProtections</span></span>

<span data-ttu-id="9bf56-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bf56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bf56-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9bf56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bf56-106">Listar propriedades e relações dos objetos [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9bf56-106">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bf56-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9bf56-107">Prerequisites</span></span>
<span data-ttu-id="9bf56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bf56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bf56-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bf56-110">Permission type</span></span>|<span data-ttu-id="9bf56-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9bf56-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bf56-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bf56-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9bf56-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bf56-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9bf56-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bf56-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bf56-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bf56-115">Not supported.</span></span>|
|<span data-ttu-id="9bf56-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bf56-116">Application</span></span>|<span data-ttu-id="9bf56-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bf56-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bf56-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bf56-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="9bf56-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf56-119">Request headers</span></span>
|<span data-ttu-id="9bf56-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9bf56-120">Header</span></span>|<span data-ttu-id="9bf56-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9bf56-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bf56-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bf56-122">Authorization</span></span>|<span data-ttu-id="9bf56-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bf56-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bf56-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9bf56-124">Accept</span></span>|<span data-ttu-id="9bf56-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9bf56-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bf56-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf56-126">Request body</span></span>
<span data-ttu-id="9bf56-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9bf56-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bf56-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bf56-128">Response</span></span>
<span data-ttu-id="9bf56-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bf56-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bf56-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bf56-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bf56-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf56-131">Request</span></span>
<span data-ttu-id="9bf56-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bf56-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="9bf56-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bf56-133">Response</span></span>
<span data-ttu-id="9bf56-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bf56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4601

{
  "value": [
    {
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
  ]
}
```






