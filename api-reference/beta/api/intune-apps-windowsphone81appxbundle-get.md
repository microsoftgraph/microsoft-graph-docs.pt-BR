---
title: Obter windowsPhone81AppXBundle
description: Leia as propriedades e as relações do objeto windowsPhone81AppXBundle.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1bd1c9b3c1725138c9672ec61b0c69eed23236e8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697123"
---
# <a name="get-windowsphone81appxbundle"></a><span data-ttu-id="92162-103">Obter windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="92162-103">Get windowsPhone81AppXBundle</span></span>

<span data-ttu-id="92162-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92162-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92162-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92162-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92162-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92162-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92162-107">Leia as propriedades e as relações do objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="92162-107">Read properties and relationships of the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92162-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92162-108">Prerequisites</span></span>
<span data-ttu-id="92162-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92162-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92162-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92162-111">Permission type</span></span>|<span data-ttu-id="92162-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92162-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92162-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92162-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92162-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="92162-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="92162-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92162-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92162-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92162-116">Not supported.</span></span>|
|<span data-ttu-id="92162-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92162-117">Application</span></span>|<span data-ttu-id="92162-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="92162-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92162-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92162-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92162-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="92162-120">Optional query parameters</span></span>
<span data-ttu-id="92162-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="92162-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92162-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92162-122">Request headers</span></span>
|<span data-ttu-id="92162-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92162-123">Header</span></span>|<span data-ttu-id="92162-124">Valor</span><span class="sxs-lookup"><span data-stu-id="92162-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92162-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="92162-125">Authorization</span></span>|<span data-ttu-id="92162-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92162-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92162-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92162-127">Accept</span></span>|<span data-ttu-id="92162-128">application/json</span><span class="sxs-lookup"><span data-stu-id="92162-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92162-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92162-129">Request body</span></span>
<span data-ttu-id="92162-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92162-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92162-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="92162-131">Response</span></span>
<span data-ttu-id="92162-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92162-132">If successful, this method returns a `200 OK` response code and [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92162-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92162-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="92162-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92162-134">Request</span></span>
<span data-ttu-id="92162-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92162-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="92162-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="92162-136">Response</span></span>
<span data-ttu-id="92162-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92162-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2703

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
    "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "uploadState": 11,
    "publishingState": "processing",
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "dependentAppCount": 1,
    "supersedingAppCount": 3,
    "supersededAppCount": 2,
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "applicableArchitectures": "x86",
    "identityName": "Identity Name value",
    "identityPublisherHash": "Identity Publisher Hash value",
    "identityResourceIdentifier": "Identity Resource Identifier value",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
      "v8_0": true,
      "v8_1": true,
      "v10_0": true,
      "v10_1607": true,
      "v10_1703": true,
      "v10_1709": true,
      "v10_1803": true,
      "v10_1809": true,
      "v10_1903": true
    },
    "phoneProductIdentifier": "Phone Product Identifier value",
    "phonePublisherId": "Phone Publisher Id value",
    "identityVersion": "Identity Version value",
    "appXPackageInformationList": [
      {
        "@odata.type": "microsoft.graph.windowsPackageInformation",
        "applicableArchitecture": "x86",
        "displayName": "Display Name value",
        "identityName": "Identity Name value",
        "identityPublisher": "Identity Publisher value",
        "identityResourceIdentifier": "Identity Resource Identifier value",
        "identityVersion": "Identity Version value",
        "minimumSupportedOperatingSystem": {
          "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
          "v8_0": true,
          "v8_1": true,
          "v10_0": true,
          "v10_1607": true,
          "v10_1703": true,
          "v10_1709": true,
          "v10_1803": true,
          "v10_1809": true,
          "v10_1903": true
        }
      }
    ]
  }
}
```





