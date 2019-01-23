---
title: Listar windowsInformationProtectionPolicies
description: Listar propriedades e relações dos objetos windowsInformationProtectionPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7f022fe1102c5c04c835df41083d21856163e800
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402682"
---
# <a name="list-windowsinformationprotectionpolicies"></a><span data-ttu-id="2b734-103">Listar windowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="2b734-103">List windowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="2b734-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2b734-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2b734-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2b734-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b734-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2b734-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b734-107">Listar propriedades e relações dos objetos [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2b734-107">List properties and relationships of the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b734-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b734-108">Prerequisites</span></span>
<span data-ttu-id="2b734-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2b734-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2b734-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b734-111">Permission type</span></span>|<span data-ttu-id="2b734-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2b734-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b734-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b734-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b734-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b734-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2b734-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b734-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b734-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b734-116">Not supported.</span></span>|
|<span data-ttu-id="2b734-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b734-117">Application</span></span>|<span data-ttu-id="2b734-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b734-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b734-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b734-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="2b734-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b734-120">Request headers</span></span>
|<span data-ttu-id="2b734-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b734-121">Header</span></span>|<span data-ttu-id="2b734-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2b734-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b734-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b734-123">Authorization</span></span>|<span data-ttu-id="2b734-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b734-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b734-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2b734-125">Accept</span></span>|<span data-ttu-id="2b734-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b734-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b734-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b734-127">Request body</span></span>
<span data-ttu-id="2b734-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b734-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b734-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b734-129">Response</span></span>
<span data-ttu-id="2b734-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b734-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b734-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b734-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b734-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b734-132">Request</span></span>
<span data-ttu-id="2b734-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b734-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="2b734-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b734-134">Response</span></span>
<span data-ttu-id="2b734-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b734-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5232

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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




