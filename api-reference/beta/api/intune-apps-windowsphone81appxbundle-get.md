---
title: Obter windowsPhone81AppXBundle
description: Leia propriedades e relações do objeto windowsPhone81AppXBundle.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e6225f4732229e174a6bf6aa3b751782bc99ef51
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133378"
---
# <a name="get-windowsphone81appxbundle"></a><span data-ttu-id="00be4-103">Obter windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="00be4-103">Get windowsPhone81AppXBundle</span></span>

<span data-ttu-id="00be4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00be4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00be4-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="00be4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00be4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00be4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00be4-107">Leia propriedades e relações do [objeto windowsPhone81AppXBundle.](../resources/intune-apps-windowsphone81appxbundle.md)</span><span class="sxs-lookup"><span data-stu-id="00be4-107">Read properties and relationships of the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00be4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="00be4-108">Prerequisites</span></span>
<span data-ttu-id="00be4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00be4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00be4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00be4-111">Permission type</span></span>|<span data-ttu-id="00be4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00be4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00be4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00be4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00be4-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00be4-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="00be4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00be4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00be4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00be4-116">Not supported.</span></span>|
|<span data-ttu-id="00be4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00be4-117">Application</span></span>|<span data-ttu-id="00be4-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00be4-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00be4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00be4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00be4-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="00be4-120">Optional query parameters</span></span>
<span data-ttu-id="00be4-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="00be4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00be4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00be4-122">Request headers</span></span>
|<span data-ttu-id="00be4-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00be4-123">Header</span></span>|<span data-ttu-id="00be4-124">Valor</span><span class="sxs-lookup"><span data-stu-id="00be4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00be4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="00be4-125">Authorization</span></span>|<span data-ttu-id="00be4-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00be4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00be4-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="00be4-127">Accept</span></span>|<span data-ttu-id="00be4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="00be4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00be4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00be4-129">Request body</span></span>
<span data-ttu-id="00be4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00be4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00be4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="00be4-131">Response</span></span>
<span data-ttu-id="00be4-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00be4-132">If successful, this method returns a `200 OK` response code and [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00be4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00be4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="00be4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00be4-134">Request</span></span>
<span data-ttu-id="00be4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00be4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="00be4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="00be4-136">Response</span></span>
<span data-ttu-id="00be4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00be4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2811

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
      "v10_1903": true,
      "v10_1909": true,
      "v10_2004": true
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
          "v10_1903": true,
          "v10_1909": true,
          "v10_2004": true
        }
      }
    ]
  }
}
```




