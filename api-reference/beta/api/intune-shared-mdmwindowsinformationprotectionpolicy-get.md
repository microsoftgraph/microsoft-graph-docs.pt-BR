---
title: Get mdmWindowsInformationProtectionPolicy
description: Ler propriedades e relações do objeto mdmWindowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 09dfb6d52c596df53f5743a85c64bd8e4cb1b786
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538046"
---
# <a name="get-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="2460e-103">Get mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="2460e-103">Get mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="2460e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2460e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2460e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2460e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2460e-106">Ler propriedades e relações do objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2460e-106">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2460e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2460e-107">Prerequisites</span></span>
<span data-ttu-id="2460e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2460e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2460e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2460e-110">Permission type</span></span>|<span data-ttu-id="2460e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2460e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2460e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2460e-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2460e-113">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="2460e-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="2460e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2460e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="2460e-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="2460e-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2460e-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2460e-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2460e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2460e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2460e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2460e-118">Not supported.</span></span>|
|<span data-ttu-id="2460e-119">Application</span><span class="sxs-lookup"><span data-stu-id="2460e-119">Application</span></span>||
| <span data-ttu-id="2460e-120">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="2460e-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="2460e-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2460e-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="2460e-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="2460e-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2460e-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2460e-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2460e-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2460e-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2460e-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2460e-125">Optional query parameters</span></span>
<span data-ttu-id="2460e-126">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2460e-126">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2460e-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2460e-127">Request headers</span></span>
|<span data-ttu-id="2460e-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2460e-128">Header</span></span>|<span data-ttu-id="2460e-129">Valor</span><span class="sxs-lookup"><span data-stu-id="2460e-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2460e-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="2460e-130">Authorization</span></span>|<span data-ttu-id="2460e-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2460e-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2460e-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2460e-132">Accept</span></span>|<span data-ttu-id="2460e-133">application/json</span><span class="sxs-lookup"><span data-stu-id="2460e-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2460e-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2460e-134">Request body</span></span>
<span data-ttu-id="2460e-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2460e-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2460e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2460e-136">Response</span></span>
<span data-ttu-id="2460e-137">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2460e-137">If successful, this method returns a `200 OK` response code and [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2460e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2460e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2460e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2460e-139">Request</span></span>
<span data-ttu-id="2460e-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2460e-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="2460e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2460e-141">Response</span></span>
<span data-ttu-id="2460e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2460e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4414

{
  "value": {
    "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
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
}
```






