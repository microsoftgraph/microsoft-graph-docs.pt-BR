---
title: Listar androidStoreApps
description: Listar propriedades e relações dos objetos androidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db35dbfa796a1dabc68c1f083039dbb2106148b3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757672"
---
# <a name="list-androidstoreapps"></a><span data-ttu-id="c0d17-103">Listar androidStoreApps</span><span class="sxs-lookup"><span data-stu-id="c0d17-103">List androidStoreApps</span></span>

<span data-ttu-id="c0d17-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0d17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0d17-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0d17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0d17-106">Listar propriedades e relações dos objetos [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="c0d17-106">List properties and relationships of the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0d17-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0d17-107">Prerequisites</span></span>
<span data-ttu-id="c0d17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0d17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0d17-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0d17-110">Permission type</span></span>|<span data-ttu-id="c0d17-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0d17-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0d17-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0d17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0d17-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0d17-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c0d17-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0d17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0d17-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0d17-115">Not supported.</span></span>|
|<span data-ttu-id="c0d17-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0d17-116">Application</span></span>|<span data-ttu-id="c0d17-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0d17-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0d17-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0d17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c0d17-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0d17-119">Request headers</span></span>
|<span data-ttu-id="c0d17-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0d17-120">Header</span></span>|<span data-ttu-id="c0d17-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c0d17-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0d17-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0d17-122">Authorization</span></span>|<span data-ttu-id="c0d17-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0d17-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0d17-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0d17-124">Accept</span></span>|<span data-ttu-id="c0d17-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0d17-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0d17-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0d17-126">Request body</span></span>
<span data-ttu-id="c0d17-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0d17-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0d17-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0d17-128">Response</span></span>
<span data-ttu-id="c0d17-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidStoreApp](../resources/intune-apps-androidstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0d17-129">If successful, this method returns a `200 OK` response code and a collection of [androidStoreApp](../resources/intune-apps-androidstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0d17-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0d17-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0d17-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0d17-131">Request</span></span>
<span data-ttu-id="c0d17-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0d17-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="c0d17-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0d17-133">Response</span></span>
<span data-ttu-id="c0d17-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0d17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1319

{
  "value": [
    {
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
        "v5_1": true,
        "v10_0": true,
        "v11_0": true
      }
    }
  ]
}
```




