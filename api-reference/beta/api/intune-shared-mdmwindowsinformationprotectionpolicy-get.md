---
title: Get mdmWindowsInformationProtectionPolicy
description: Ler propriedades e relações do objeto mdmWindowsInformationProtectionPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3c5f4d93727cb9da563b81f2f87db1b1a45f8fc2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724049"
---
# <a name="get-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="e69e0-103">Get mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e69e0-103">Get mdmWindowsInformationProtectionPolicy</span></span>

<span data-ttu-id="e69e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e69e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e69e0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e69e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e69e0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e69e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e69e0-107">Ler propriedades e relações do objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e69e0-107">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e69e0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e69e0-108">Prerequisites</span></span>
<span data-ttu-id="e69e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e69e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e69e0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e69e0-111">Permission type</span></span>|<span data-ttu-id="e69e0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e69e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e69e0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e69e0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e69e0-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="e69e0-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="e69e0-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e69e0-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="e69e0-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="e69e0-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e69e0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e69e0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e69e0-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e69e0-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e69e0-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e69e0-119">Not supported.</span></span>|
|<span data-ttu-id="e69e0-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e69e0-120">Application</span></span>||
| <span data-ttu-id="e69e0-121">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="e69e0-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="e69e0-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e69e0-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="e69e0-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="e69e0-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e69e0-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e69e0-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e69e0-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e69e0-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e69e0-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e69e0-126">Optional query parameters</span></span>
<span data-ttu-id="e69e0-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e69e0-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e69e0-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e69e0-128">Request headers</span></span>
|<span data-ttu-id="e69e0-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e69e0-129">Header</span></span>|<span data-ttu-id="e69e0-130">Valor</span><span class="sxs-lookup"><span data-stu-id="e69e0-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e69e0-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="e69e0-131">Authorization</span></span>|<span data-ttu-id="e69e0-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e69e0-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e69e0-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e69e0-133">Accept</span></span>|<span data-ttu-id="e69e0-134">application/json</span><span class="sxs-lookup"><span data-stu-id="e69e0-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e69e0-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e69e0-135">Request body</span></span>
<span data-ttu-id="e69e0-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e69e0-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e69e0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e69e0-137">Response</span></span>
<span data-ttu-id="e69e0-138">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e69e0-138">If successful, this method returns a `200 OK` response code and [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e69e0-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e69e0-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="e69e0-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e69e0-140">Request</span></span>
<span data-ttu-id="e69e0-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e69e0-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="e69e0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e69e0-142">Response</span></span>
<span data-ttu-id="e69e0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e69e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








