---
title: Acessar iosStoreApp
description: Leia as propriedades e as relações do objeto iosStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e308798275eab9c2c38f836083c73b2d5302d187
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757343"
---
# <a name="get-iosstoreapp"></a><span data-ttu-id="fe57d-103">Acessar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="fe57d-103">Get iosStoreApp</span></span>

<span data-ttu-id="fe57d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe57d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe57d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe57d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe57d-106">Leia as propriedades e as relações do objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe57d-106">Read properties and relationships of the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe57d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe57d-107">Prerequisites</span></span>
<span data-ttu-id="fe57d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe57d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe57d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe57d-110">Permission type</span></span>|<span data-ttu-id="fe57d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe57d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe57d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe57d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe57d-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe57d-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fe57d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe57d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe57d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe57d-115">Not supported.</span></span>|
|<span data-ttu-id="fe57d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe57d-116">Application</span></span>|<span data-ttu-id="fe57d-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe57d-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe57d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe57d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe57d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe57d-119">Optional query parameters</span></span>
<span data-ttu-id="fe57d-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fe57d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe57d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe57d-121">Request headers</span></span>
|<span data-ttu-id="fe57d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe57d-122">Header</span></span>|<span data-ttu-id="fe57d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="fe57d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe57d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe57d-124">Authorization</span></span>|<span data-ttu-id="fe57d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe57d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe57d-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fe57d-126">Accept</span></span>|<span data-ttu-id="fe57d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fe57d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe57d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe57d-128">Request body</span></span>
<span data-ttu-id="fe57d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe57d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe57d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe57d-130">Response</span></span>
<span data-ttu-id="fe57d-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe57d-131">If successful, this method returns a `200 OK` response code and [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe57d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe57d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe57d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe57d-133">Request</span></span>
<span data-ttu-id="fe57d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe57d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="fe57d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe57d-135">Response</span></span>
<span data-ttu-id="fe57d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe57d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1309

{
  "value": {
    "@odata.type": "#microsoft.graph.iosStoreApp",
    "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
      "v12_0": true,
      "v13_0": true,
      "v14_0": true
    }
  }
}
```




