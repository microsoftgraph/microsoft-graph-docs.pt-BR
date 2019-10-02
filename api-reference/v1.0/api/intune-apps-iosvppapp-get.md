---
title: Acessar iosVppApp
description: Leia as propriedades e as relações do objeto iosVppApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7bb5335861aa292aa5927106d49b611c6f77e128
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358820"
---
# <a name="get-iosvppapp"></a><span data-ttu-id="30271-103">Acessar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="30271-103">Get iosVppApp</span></span>

> <span data-ttu-id="30271-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30271-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30271-105">Leia as propriedades e as relações do objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="30271-105">Read properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30271-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30271-106">Prerequisites</span></span>
<span data-ttu-id="30271-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30271-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30271-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30271-109">Permission type</span></span>|<span data-ttu-id="30271-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30271-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30271-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30271-111">Delegated (work or school account)</span></span>|<span data-ttu-id="30271-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="30271-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="30271-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30271-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30271-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30271-114">Not supported.</span></span>|
|<span data-ttu-id="30271-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30271-115">Application</span></span>|<span data-ttu-id="30271-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30271-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30271-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30271-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30271-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="30271-118">Optional query parameters</span></span>
<span data-ttu-id="30271-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="30271-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30271-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30271-120">Request headers</span></span>
|<span data-ttu-id="30271-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30271-121">Header</span></span>|<span data-ttu-id="30271-122">Valor</span><span class="sxs-lookup"><span data-stu-id="30271-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30271-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="30271-123">Authorization</span></span>|<span data-ttu-id="30271-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30271-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30271-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30271-125">Accept</span></span>|<span data-ttu-id="30271-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30271-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30271-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30271-127">Request body</span></span>
<span data-ttu-id="30271-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30271-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30271-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="30271-129">Response</span></span>
<span data-ttu-id="30271-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30271-130">If successful, this method returns a `200 OK` response code and [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30271-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30271-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="30271-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30271-132">Request</span></span>
<span data-ttu-id="30271-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30271-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="30271-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="30271-134">Response</span></span>
<span data-ttu-id="30271-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30271-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1487

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppApp",
    "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "licensingType": {
      "@odata.type": "microsoft.graph.vppLicensingType",
      "supportsUserLicensing": true,
      "supportsDeviceLicensing": true
    },
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "vppTokenOrganizationName": "Vpp Token Organization Name value",
    "vppTokenAccountType": "education",
    "vppTokenAppleId": "Vpp Token Apple Id value",
    "bundleId": "Bundle Id value"
  }
}
```




