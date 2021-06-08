---
title: Listar mdmWindowsInformationProtectionPolicies
description: Listar propriedades e relações dos objetos mdmWindowsInformationProtectionPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 72f512779439a11c41e89f22be5abfcf31efd5ad
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760346"
---
# <a name="list-mdmwindowsinformationprotectionpolicies"></a><span data-ttu-id="19022-103">Listar mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="19022-103">List mdmWindowsInformationProtectionPolicies</span></span>

<span data-ttu-id="19022-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19022-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19022-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19022-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19022-106">Listar propriedades e relações dos objetos [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="19022-106">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19022-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="19022-107">Prerequisites</span></span>
<span data-ttu-id="19022-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19022-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19022-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19022-110">Permission type</span></span>|<span data-ttu-id="19022-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19022-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19022-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19022-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19022-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19022-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="19022-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19022-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19022-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19022-115">Not supported.</span></span>|
|<span data-ttu-id="19022-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19022-116">Application</span></span>|<span data-ttu-id="19022-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19022-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19022-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19022-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="19022-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19022-119">Request headers</span></span>
|<span data-ttu-id="19022-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19022-120">Header</span></span>|<span data-ttu-id="19022-121">Valor</span><span class="sxs-lookup"><span data-stu-id="19022-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19022-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="19022-122">Authorization</span></span>|<span data-ttu-id="19022-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19022-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19022-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="19022-124">Accept</span></span>|<span data-ttu-id="19022-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19022-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19022-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19022-126">Request body</span></span>
<span data-ttu-id="19022-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="19022-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19022-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="19022-128">Response</span></span>
<span data-ttu-id="19022-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19022-129">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19022-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19022-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="19022-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19022-131">Request</span></span>
<span data-ttu-id="19022-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19022-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="19022-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="19022-133">Response</span></span>
<span data-ttu-id="19022-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19022-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4610

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "8efb0c35-0c35-8efb-350c-fb8e350cfb8e",
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




