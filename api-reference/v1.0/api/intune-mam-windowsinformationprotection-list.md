---
title: Listar windowsInformationProtections
description: Listar propriedades e relações dos objetos windowsInformationProtection.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dc8b9245bf71b8c7c81ea3a51e260ff3bca557da
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889828"
---
# <a name="list-windowsinformationprotections"></a><span data-ttu-id="e1afc-103">Listar windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="e1afc-103">List windowsInformationProtections</span></span>

> <span data-ttu-id="e1afc-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e1afc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1afc-105">Listar propriedades e relações dos objetos [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="e1afc-105">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1afc-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1afc-106">Prerequisites</span></span>
<span data-ttu-id="e1afc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1afc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1afc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1afc-109">Permission type</span></span>|<span data-ttu-id="e1afc-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1afc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1afc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1afc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e1afc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1afc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e1afc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1afc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1afc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1afc-114">Not supported.</span></span>|
|<span data-ttu-id="e1afc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1afc-115">Application</span></span>|<span data-ttu-id="e1afc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1afc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1afc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1afc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="e1afc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1afc-118">Request headers</span></span>
|<span data-ttu-id="e1afc-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1afc-119">Header</span></span>|<span data-ttu-id="e1afc-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e1afc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1afc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1afc-121">Authorization</span></span>|<span data-ttu-id="e1afc-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1afc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1afc-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1afc-123">Accept</span></span>|<span data-ttu-id="e1afc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e1afc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1afc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1afc-125">Request body</span></span>
<span data-ttu-id="e1afc-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1afc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1afc-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1afc-127">Response</span></span>
<span data-ttu-id="e1afc-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1afc-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1afc-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1afc-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1afc-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1afc-130">Request</span></span>
<span data-ttu-id="e1afc-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1afc-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="e1afc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1afc-132">Response</span></span>
<span data-ttu-id="e1afc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1afc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



