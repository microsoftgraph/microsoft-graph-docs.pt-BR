---
title: Listar windowsInformationProtectionPolicies
description: Listar propriedades e relações dos objetos windowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 98d76b9fcb3bc9095d48c0e8106a23439004c171
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974584"
---
# <a name="list-windowsinformationprotectionpolicies"></a><span data-ttu-id="a1a88-103">Listar windowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="a1a88-103">List windowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="a1a88-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1a88-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1a88-105">Listar propriedades e relações dos objetos [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1a88-105">List properties and relationships of the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1a88-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1a88-106">Prerequisites</span></span>
<span data-ttu-id="a1a88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1a88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1a88-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1a88-109">Permission type</span></span>|<span data-ttu-id="a1a88-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1a88-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1a88-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1a88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a1a88-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1a88-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a1a88-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1a88-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1a88-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1a88-114">Not supported.</span></span>|
|<span data-ttu-id="a1a88-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1a88-115">Application</span></span>|<span data-ttu-id="a1a88-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1a88-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1a88-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1a88-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="a1a88-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1a88-118">Request headers</span></span>
|<span data-ttu-id="a1a88-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1a88-119">Header</span></span>|<span data-ttu-id="a1a88-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a1a88-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1a88-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1a88-121">Authorization</span></span>|<span data-ttu-id="a1a88-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1a88-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1a88-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1a88-123">Accept</span></span>|<span data-ttu-id="a1a88-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a1a88-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1a88-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1a88-125">Request body</span></span>
<span data-ttu-id="a1a88-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1a88-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1a88-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1a88-127">Response</span></span>
<span data-ttu-id="a1a88-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1a88-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1a88-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1a88-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1a88-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1a88-130">Request</span></span>
<span data-ttu-id="a1a88-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1a88-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="a1a88-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1a88-132">Response</span></span>
<span data-ttu-id="a1a88-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1a88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5158

{
  "value": [
    {
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
  ]
}
```



