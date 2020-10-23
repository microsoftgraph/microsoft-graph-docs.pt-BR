---
title: Listar mdmWindowsInformationProtectionPolicies
description: Listar propriedades e relações dos objetos mdmWindowsInformationProtectionPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 213c0b518f6e8360a5ba1cc1d70e1451eef2cde5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724007"
---
# <a name="list-mdmwindowsinformationprotectionpolicies"></a><span data-ttu-id="1bf6c-103">Listar mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="1bf6c-103">List mdmWindowsInformationProtectionPolicies</span></span>

<span data-ttu-id="1bf6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bf6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bf6c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1bf6c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bf6c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1bf6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bf6c-107">Listar propriedades e relações dos objetos [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1bf6c-107">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bf6c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1bf6c-108">Prerequisites</span></span>
<span data-ttu-id="1bf6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bf6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bf6c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bf6c-111">Permission type</span></span>|<span data-ttu-id="1bf6c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1bf6c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bf6c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bf6c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1bf6c-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="1bf6c-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="1bf6c-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bf6c-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="1bf6c-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="1bf6c-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1bf6c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bf6c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1bf6c-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bf6c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bf6c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bf6c-119">Not supported.</span></span>|
|<span data-ttu-id="1bf6c-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bf6c-120">Application</span></span>||
| <span data-ttu-id="1bf6c-121">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="1bf6c-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="1bf6c-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bf6c-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="1bf6c-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="1bf6c-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1bf6c-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bf6c-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bf6c-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bf6c-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="1bf6c-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bf6c-126">Request headers</span></span>
|<span data-ttu-id="1bf6c-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1bf6c-127">Header</span></span>|<span data-ttu-id="1bf6c-128">Valor</span><span class="sxs-lookup"><span data-stu-id="1bf6c-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bf6c-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bf6c-129">Authorization</span></span>|<span data-ttu-id="1bf6c-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bf6c-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bf6c-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1bf6c-131">Accept</span></span>|<span data-ttu-id="1bf6c-132">application/json</span><span class="sxs-lookup"><span data-stu-id="1bf6c-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bf6c-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bf6c-133">Request body</span></span>
<span data-ttu-id="1bf6c-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1bf6c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bf6c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bf6c-135">Response</span></span>
<span data-ttu-id="1bf6c-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bf6c-136">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bf6c-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bf6c-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bf6c-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bf6c-138">Request</span></span>
<span data-ttu-id="1bf6c-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bf6c-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="1bf6c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bf6c-140">Response</span></span>
<span data-ttu-id="1bf6c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bf6c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4684

{
  "value": [
    {
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
  ]
}
```








