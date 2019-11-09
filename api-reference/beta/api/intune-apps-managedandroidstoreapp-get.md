---
title: Acessar managedAndroidStoreApp
description: Leia as propriedades e as relações do objeto managedAndroidStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c95f9368638b1af85d20139487e2eebc4efc9959
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38080046"
---
# <a name="get-managedandroidstoreapp"></a><span data-ttu-id="4744f-103">Acessar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="4744f-103">Get managedAndroidStoreApp</span></span>

> <span data-ttu-id="4744f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4744f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4744f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4744f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4744f-106">Leia as propriedades e as relações do objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4744f-106">Read properties and relationships of the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4744f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4744f-107">Prerequisites</span></span>
<span data-ttu-id="4744f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4744f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4744f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4744f-110">Permission type</span></span>|<span data-ttu-id="4744f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4744f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4744f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4744f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4744f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4744f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4744f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4744f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4744f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4744f-115">Not supported.</span></span>|
|<span data-ttu-id="4744f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4744f-116">Application</span></span>|<span data-ttu-id="4744f-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4744f-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4744f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4744f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4744f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4744f-119">Optional query parameters</span></span>
<span data-ttu-id="4744f-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4744f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4744f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4744f-121">Request headers</span></span>
|<span data-ttu-id="4744f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4744f-122">Header</span></span>|<span data-ttu-id="4744f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4744f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4744f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4744f-124">Authorization</span></span>|<span data-ttu-id="4744f-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4744f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4744f-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4744f-126">Accept</span></span>|<span data-ttu-id="4744f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4744f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4744f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4744f-128">Request body</span></span>
<span data-ttu-id="4744f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4744f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4744f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4744f-130">Response</span></span>
<span data-ttu-id="4744f-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4744f-131">If successful, this method returns a `200 OK` response code and [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4744f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4744f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4744f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4744f-133">Request</span></span>
<span data-ttu-id="4744f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4744f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="4744f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4744f-135">Response</span></span>
<span data-ttu-id="4744f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4744f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1547

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
    "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
    "packageId": "Package Id value",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true,
      "v6_0": true,
      "v7_0": true,
      "v7_1": true,
      "v8_0": true,
      "v8_1": true,
      "v9_0": true
    }
  }
}
```






