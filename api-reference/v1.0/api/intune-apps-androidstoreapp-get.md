---
title: Get androidStoreApp
description: Ler propriedades e relações do objeto androidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e1158b9d56c7f4a095b2216c720a138e923d9728
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466657"
---
# <a name="get-androidstoreapp"></a><span data-ttu-id="a0148-103">Get androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="a0148-103">Get androidStoreApp</span></span>

<span data-ttu-id="a0148-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0148-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0148-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0148-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0148-106">Ler propriedades e relações do objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="a0148-106">Read properties and relationships of the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0148-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0148-107">Prerequisites</span></span>
<span data-ttu-id="a0148-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0148-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0148-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0148-110">Permission type</span></span>|<span data-ttu-id="a0148-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0148-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0148-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0148-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0148-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0148-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a0148-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0148-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0148-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0148-115">Not supported.</span></span>|
|<span data-ttu-id="a0148-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0148-116">Application</span></span>|<span data-ttu-id="a0148-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0148-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0148-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0148-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0148-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0148-119">Optional query parameters</span></span>
<span data-ttu-id="a0148-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a0148-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0148-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0148-121">Request headers</span></span>
|<span data-ttu-id="a0148-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0148-122">Header</span></span>|<span data-ttu-id="a0148-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a0148-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0148-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0148-124">Authorization</span></span>|<span data-ttu-id="a0148-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0148-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0148-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0148-126">Accept</span></span>|<span data-ttu-id="a0148-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a0148-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0148-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0148-128">Request body</span></span>
<span data-ttu-id="a0148-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0148-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0148-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0148-130">Response</span></span>
<span data-ttu-id="a0148-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0148-131">If successful, this method returns a `200 OK` response code and [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0148-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0148-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0148-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0148-133">Request</span></span>
<span data-ttu-id="a0148-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0148-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="a0148-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0148-135">Response</span></span>
<span data-ttu-id="a0148-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0148-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1193

{
  "value": {
    "@odata.type": "#microsoft.graph.androidStoreApp",
    "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
      "v5_1": true
    }
  }
}
```






