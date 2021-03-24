---
title: Acessar managedAndroidStoreApp
description: Leia as propriedades e as relações do objeto managedAndroidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b3c87e13df7f0e773e27efe1222c9435ff4de9f3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140263"
---
# <a name="get-managedandroidstoreapp"></a><span data-ttu-id="7bb68-103">Acessar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="7bb68-103">Get managedAndroidStoreApp</span></span>

<span data-ttu-id="7bb68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bb68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7bb68-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7bb68-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bb68-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7bb68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bb68-107">Leia as propriedades e as relações do objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bb68-107">Read properties and relationships of the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bb68-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7bb68-108">Prerequisites</span></span>
<span data-ttu-id="7bb68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bb68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bb68-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bb68-111">Permission type</span></span>|<span data-ttu-id="7bb68-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7bb68-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bb68-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bb68-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7bb68-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bb68-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7bb68-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bb68-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bb68-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bb68-116">Not supported.</span></span>|
|<span data-ttu-id="7bb68-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bb68-117">Application</span></span>|<span data-ttu-id="7bb68-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bb68-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bb68-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bb68-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7bb68-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7bb68-120">Optional query parameters</span></span>
<span data-ttu-id="7bb68-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7bb68-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bb68-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bb68-122">Request headers</span></span>
|<span data-ttu-id="7bb68-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7bb68-123">Header</span></span>|<span data-ttu-id="7bb68-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7bb68-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bb68-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bb68-125">Authorization</span></span>|<span data-ttu-id="7bb68-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bb68-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bb68-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7bb68-127">Accept</span></span>|<span data-ttu-id="7bb68-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7bb68-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bb68-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bb68-129">Request body</span></span>
<span data-ttu-id="7bb68-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7bb68-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bb68-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bb68-131">Response</span></span>
<span data-ttu-id="7bb68-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bb68-132">If successful, this method returns a `200 OK` response code and [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bb68-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bb68-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bb68-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bb68-134">Request</span></span>
<span data-ttu-id="7bb68-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7bb68-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="7bb68-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bb68-136">Response</span></span>
<span data-ttu-id="7bb68-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7bb68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1652

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
    "supersedingAppCount": 3,
    "supersededAppCount": 2,
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
      "v9_0": true,
      "v10_0": true,
      "v11_0": true
    }
  }
}
```




