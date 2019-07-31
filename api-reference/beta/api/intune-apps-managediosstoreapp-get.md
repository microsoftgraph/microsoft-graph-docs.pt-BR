---
title: Acessar managedIOSStoreApp
description: Leia as propriedades e as relações do objeto managedIOSStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6f5d362e0d52bbec3df82cd40ce46f4b5dcb4f22
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961312"
---
# <a name="get-managediosstoreapp"></a><span data-ttu-id="dc581-103">Acessar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="dc581-103">Get managedIOSStoreApp</span></span>

> <span data-ttu-id="dc581-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc581-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc581-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc581-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc581-106">Leia as propriedades e as relações do objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="dc581-106">Read properties and relationships of the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc581-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc581-107">Prerequisites</span></span>
<span data-ttu-id="dc581-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc581-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc581-110">Permission type</span></span>|<span data-ttu-id="dc581-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc581-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc581-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc581-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc581-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc581-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dc581-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc581-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc581-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc581-115">Not supported.</span></span>|
|<span data-ttu-id="dc581-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc581-116">Application</span></span>|<span data-ttu-id="dc581-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc581-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc581-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc581-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dc581-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dc581-119">Optional query parameters</span></span>
<span data-ttu-id="dc581-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dc581-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc581-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc581-121">Request headers</span></span>
|<span data-ttu-id="dc581-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc581-122">Header</span></span>|<span data-ttu-id="dc581-123">Valor</span><span class="sxs-lookup"><span data-stu-id="dc581-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc581-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc581-124">Authorization</span></span>|<span data-ttu-id="dc581-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc581-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc581-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc581-126">Accept</span></span>|<span data-ttu-id="dc581-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dc581-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc581-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc581-128">Request body</span></span>
<span data-ttu-id="dc581-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc581-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc581-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc581-130">Response</span></span>
<span data-ttu-id="dc581-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc581-131">If successful, this method returns a `200 OK` response code and [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc581-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc581-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc581-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc581-133">Request</span></span>
<span data-ttu-id="dc581-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc581-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="dc581-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc581-135">Response</span></span>
<span data-ttu-id="dc581-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc581-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1493

{
  "value": {
    "@odata.type": "#microsoft.graph.managedIOSStoreApp",
    "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
    "bundleId": "Bundle Id value",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
      "v8_0": true,
      "v9_0": true,
      "v10_0": true,
      "v11_0": true,
      "v12_0": true
    }
  }
}
```





