---
title: Obter androidManagedStoreApp
description: Leia as propriedades e os relacionamentos do objeto androidManagedStoreApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f8f17d04de751ab0bb7d70e46db0827c2a35ea6c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406231"
---
# <a name="get-androidmanagedstoreapp"></a><span data-ttu-id="bebad-103">Obter androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="bebad-103">Get androidManagedStoreApp</span></span>

> <span data-ttu-id="bebad-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="bebad-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bebad-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bebad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bebad-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="bebad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bebad-107">Leia as propriedades e os relacionamentos do objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="bebad-107">Read properties and relationships of the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bebad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bebad-108">Prerequisites</span></span>
<span data-ttu-id="bebad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bebad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bebad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bebad-111">Permission type</span></span>|<span data-ttu-id="bebad-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bebad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bebad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bebad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bebad-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bebad-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bebad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bebad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bebad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bebad-116">Not supported.</span></span>|
|<span data-ttu-id="bebad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bebad-117">Application</span></span>|<span data-ttu-id="bebad-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bebad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bebad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bebad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bebad-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bebad-120">Optional query parameters</span></span>
<span data-ttu-id="bebad-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bebad-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bebad-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bebad-122">Request headers</span></span>
|<span data-ttu-id="bebad-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bebad-123">Header</span></span>|<span data-ttu-id="bebad-124">Valor</span><span class="sxs-lookup"><span data-stu-id="bebad-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bebad-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="bebad-125">Authorization</span></span>|<span data-ttu-id="bebad-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bebad-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bebad-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bebad-127">Accept</span></span>|<span data-ttu-id="bebad-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bebad-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bebad-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bebad-129">Request body</span></span>
<span data-ttu-id="bebad-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bebad-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bebad-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="bebad-131">Response</span></span>
<span data-ttu-id="bebad-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bebad-132">If successful, this method returns a `200 OK` response code and [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bebad-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bebad-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bebad-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bebad-134">Request</span></span>
<span data-ttu-id="bebad-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bebad-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="bebad-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bebad-136">Response</span></span>
<span data-ttu-id="bebad-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bebad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1130

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreApp",
    "id": "87247525-7525-8724-2575-248725752487",
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
    "packageId": "Package Id value",
    "appIdentifier": "App Identifier value",
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "appStoreUrl": "https://example.com/appStoreUrl/"
  }
}
```




