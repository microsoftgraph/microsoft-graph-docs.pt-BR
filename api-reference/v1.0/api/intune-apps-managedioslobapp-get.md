---
title: Acessar managedIOSLobApp
description: Leia as propriedades e as relações do objeto managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f1cbf7f0989e1bc1c9058d7a84cee84c88c6d7a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025836"
---
# <a name="get-managedioslobapp"></a><span data-ttu-id="17903-103">Acessar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="17903-103">Get managedIOSLobApp</span></span>

<span data-ttu-id="17903-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17903-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17903-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17903-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17903-106">Leia as propriedades e as relações do objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="17903-106">Read properties and relationships of the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17903-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17903-107">Prerequisites</span></span>
<span data-ttu-id="17903-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="17903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="17903-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17903-110">Permission type</span></span>|<span data-ttu-id="17903-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17903-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17903-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17903-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17903-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="17903-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="17903-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17903-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17903-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17903-115">Not supported.</span></span>|
|<span data-ttu-id="17903-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17903-116">Application</span></span>|<span data-ttu-id="17903-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="17903-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17903-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17903-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17903-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="17903-119">Optional query parameters</span></span>
<span data-ttu-id="17903-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="17903-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17903-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17903-121">Request headers</span></span>
|<span data-ttu-id="17903-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17903-122">Header</span></span>|<span data-ttu-id="17903-123">Valor</span><span class="sxs-lookup"><span data-stu-id="17903-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17903-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="17903-124">Authorization</span></span>|<span data-ttu-id="17903-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17903-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17903-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17903-126">Accept</span></span>|<span data-ttu-id="17903-127">application/json</span><span class="sxs-lookup"><span data-stu-id="17903-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17903-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17903-128">Request body</span></span>
<span data-ttu-id="17903-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17903-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17903-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="17903-130">Response</span></span>
<span data-ttu-id="17903-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17903-131">If successful, this method returns a `200 OK` response code and [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17903-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17903-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="17903-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17903-133">Request</span></span>
<span data-ttu-id="17903-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17903-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="17903-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="17903-135">Response</span></span>
<span data-ttu-id="17903-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17903-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1582

{
  "value": {
    "@odata.type": "#microsoft.graph.managedIOSLobApp",
    "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
    "publishingState": "processing",
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "bundleId": "Bundle Id value",
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
      "v12_0": true,
      "v13_0": true
    },
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "versionNumber": "Version Number value",
    "buildNumber": "Build Number value"
  }
}
```









