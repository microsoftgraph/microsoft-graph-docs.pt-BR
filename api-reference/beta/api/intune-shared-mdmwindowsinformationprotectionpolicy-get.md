---
title: Get mdmWindowsInformationProtectionPolicy
description: Ler propriedades e relações do objeto mdmWindowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca55cae17366d5c0ffd79e4e70ffbd66b59417c7
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865485"
---
# <a name="get-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="aafeb-103">Get mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="aafeb-103">Get mdmWindowsInformationProtectionPolicy</span></span>

<span data-ttu-id="aafeb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aafeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aafeb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aafeb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aafeb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aafeb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aafeb-107">Ler propriedades e relações do objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aafeb-107">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aafeb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aafeb-108">Prerequisites</span></span>
<span data-ttu-id="aafeb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aafeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aafeb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aafeb-111">Permission type</span></span>|<span data-ttu-id="aafeb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aafeb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aafeb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aafeb-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="aafeb-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="aafeb-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="aafeb-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aafeb-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="aafeb-116">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="aafeb-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="aafeb-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aafeb-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="aafeb-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aafeb-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aafeb-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aafeb-119">Not supported.</span></span>|
|<span data-ttu-id="aafeb-120">Application</span><span class="sxs-lookup"><span data-stu-id="aafeb-120">Application</span></span>||
| <span data-ttu-id="aafeb-121">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="aafeb-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="aafeb-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aafeb-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="aafeb-123">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="aafeb-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="aafeb-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aafeb-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aafeb-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aafeb-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aafeb-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aafeb-126">Optional query parameters</span></span>
<span data-ttu-id="aafeb-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aafeb-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aafeb-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aafeb-128">Request headers</span></span>
|<span data-ttu-id="aafeb-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aafeb-129">Header</span></span>|<span data-ttu-id="aafeb-130">Valor</span><span class="sxs-lookup"><span data-stu-id="aafeb-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aafeb-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="aafeb-131">Authorization</span></span>|<span data-ttu-id="aafeb-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aafeb-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aafeb-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aafeb-133">Accept</span></span>|<span data-ttu-id="aafeb-134">application/json</span><span class="sxs-lookup"><span data-stu-id="aafeb-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aafeb-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aafeb-135">Request body</span></span>
<span data-ttu-id="aafeb-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aafeb-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aafeb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="aafeb-137">Response</span></span>
<span data-ttu-id="aafeb-138">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aafeb-138">If successful, this method returns a `200 OK` response code and [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aafeb-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aafeb-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="aafeb-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aafeb-140">Request</span></span>
<span data-ttu-id="aafeb-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aafeb-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="aafeb-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="aafeb-142">Response</span></span>
<span data-ttu-id="aafeb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aafeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







