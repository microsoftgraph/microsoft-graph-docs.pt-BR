---
title: Listar mdmWindowsInformationProtectionPolicies
description: Listar propriedades e relações dos objetos mdmWindowsInformationProtectionPolicy.
author: tfitzmac
ms.openlocfilehash: fbdf6a180940018744d5026893c71f8a2e414985
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322208"
---
# <a name="list-mdmwindowsinformationprotectionpolicies"></a><span data-ttu-id="38114-103">Listar mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="38114-103">List mdmWindowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="38114-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="38114-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38114-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="38114-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38114-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="38114-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38114-107">Listar propriedades e relações dos objetos [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="38114-107">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38114-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38114-108">Prerequisites</span></span>
<span data-ttu-id="38114-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38114-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38114-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38114-111">Permission type</span></span>|<span data-ttu-id="38114-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38114-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38114-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38114-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38114-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="38114-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="38114-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38114-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38114-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38114-116">Not supported.</span></span>|
|<span data-ttu-id="38114-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38114-117">Application</span></span>|<span data-ttu-id="38114-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38114-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38114-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38114-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="38114-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38114-120">Request headers</span></span>
|<span data-ttu-id="38114-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38114-121">Header</span></span>|<span data-ttu-id="38114-122">Valor</span><span class="sxs-lookup"><span data-stu-id="38114-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38114-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="38114-123">Authorization</span></span>|<span data-ttu-id="38114-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38114-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38114-125">Accept</span><span class="sxs-lookup"><span data-stu-id="38114-125">Accept</span></span>|<span data-ttu-id="38114-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38114-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38114-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38114-127">Request body</span></span>
<span data-ttu-id="38114-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38114-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38114-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="38114-129">Response</span></span>
<span data-ttu-id="38114-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38114-130">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38114-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38114-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="38114-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38114-132">Request</span></span>
<span data-ttu-id="38114-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38114-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="38114-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="38114-134">Response</span></span>
<span data-ttu-id="38114-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38114-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





