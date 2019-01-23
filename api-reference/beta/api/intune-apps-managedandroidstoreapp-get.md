---
title: Acessar managedAndroidStoreApp
description: Leia as propriedades e as relações do objeto managedAndroidStoreApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0c39ae96e58440dae8dcaf8ce32ec038e31b1289
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417130"
---
# <a name="get-managedandroidstoreapp"></a><span data-ttu-id="5cfca-103">Acessar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="5cfca-103">Get managedAndroidStoreApp</span></span>

> <span data-ttu-id="5cfca-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5cfca-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5cfca-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5cfca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5cfca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5cfca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cfca-107">Leia as propriedades e as relações do objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cfca-107">Read properties and relationships of the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cfca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5cfca-108">Prerequisites</span></span>
<span data-ttu-id="5cfca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5cfca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5cfca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5cfca-111">Permission type</span></span>|<span data-ttu-id="5cfca-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5cfca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cfca-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5cfca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5cfca-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cfca-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5cfca-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5cfca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cfca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5cfca-116">Not supported.</span></span>|
|<span data-ttu-id="5cfca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5cfca-117">Application</span></span>|<span data-ttu-id="5cfca-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5cfca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cfca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5cfca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5cfca-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5cfca-120">Optional query parameters</span></span>
<span data-ttu-id="5cfca-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5cfca-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5cfca-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5cfca-122">Request headers</span></span>
|<span data-ttu-id="5cfca-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5cfca-123">Header</span></span>|<span data-ttu-id="5cfca-124">Valor</span><span class="sxs-lookup"><span data-stu-id="5cfca-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cfca-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5cfca-125">Authorization</span></span>|<span data-ttu-id="5cfca-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5cfca-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cfca-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5cfca-127">Accept</span></span>|<span data-ttu-id="5cfca-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5cfca-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cfca-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5cfca-129">Request body</span></span>
<span data-ttu-id="5cfca-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5cfca-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cfca-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cfca-131">Response</span></span>
<span data-ttu-id="5cfca-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5cfca-132">If successful, this method returns a `200 OK` response code and [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cfca-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5cfca-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cfca-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5cfca-134">Request</span></span>
<span data-ttu-id="5cfca-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5cfca-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="5cfca-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cfca-136">Response</span></span>
<span data-ttu-id="5cfca-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5cfca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1518

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




