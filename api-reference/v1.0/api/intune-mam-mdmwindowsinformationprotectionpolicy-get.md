---
title: Get mdmWindowsInformationProtectionPolicy
description: Ler propriedades e relações do objeto mdmWindowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bd72742b2aa3a32adfa3b24fafb793178043f23e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938108"
---
# <a name="get-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="94fd2-103">Get mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="94fd2-103">Get mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="94fd2-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="94fd2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94fd2-105">Ler propriedades e relações do objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="94fd2-105">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94fd2-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94fd2-106">Prerequisites</span></span>
<span data-ttu-id="94fd2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94fd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94fd2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94fd2-109">Permission type</span></span>|<span data-ttu-id="94fd2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="94fd2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94fd2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94fd2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="94fd2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="94fd2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="94fd2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94fd2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94fd2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94fd2-114">Not supported.</span></span>|
|<span data-ttu-id="94fd2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94fd2-115">Application</span></span>|<span data-ttu-id="94fd2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94fd2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94fd2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94fd2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94fd2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="94fd2-118">Optional query parameters</span></span>
<span data-ttu-id="94fd2-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="94fd2-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="94fd2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94fd2-120">Request headers</span></span>
|<span data-ttu-id="94fd2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94fd2-121">Header</span></span>|<span data-ttu-id="94fd2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="94fd2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94fd2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="94fd2-123">Authorization</span></span>|<span data-ttu-id="94fd2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94fd2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94fd2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94fd2-125">Accept</span></span>|<span data-ttu-id="94fd2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94fd2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94fd2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94fd2-127">Request body</span></span>
<span data-ttu-id="94fd2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94fd2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94fd2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="94fd2-129">Response</span></span>
<span data-ttu-id="94fd2-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94fd2-130">If successful, this method returns a `200 OK` response code and [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94fd2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94fd2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="94fd2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94fd2-132">Request</span></span>
<span data-ttu-id="94fd2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94fd2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="94fd2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="94fd2-134">Response</span></span>
<span data-ttu-id="94fd2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94fd2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4346

{
  "value": {
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
}
```



