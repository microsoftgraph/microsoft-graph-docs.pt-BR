---
title: Listar androidStoreApps
description: Listar propriedades e relações dos objetos androidStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e0751b543c962c6f4deafb6d0ecb82c24551e818
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445796"
---
# <a name="list-androidstoreapps"></a><span data-ttu-id="ba226-103">Listar androidStoreApps</span><span class="sxs-lookup"><span data-stu-id="ba226-103">List androidStoreApps</span></span>

<span data-ttu-id="ba226-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ba226-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba226-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba226-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba226-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba226-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba226-107">Listar propriedades e relações dos objetos [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba226-107">List properties and relationships of the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba226-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba226-108">Prerequisites</span></span>
<span data-ttu-id="ba226-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba226-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba226-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba226-111">Permission type</span></span>|<span data-ttu-id="ba226-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ba226-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba226-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba226-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba226-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba226-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ba226-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba226-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba226-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba226-116">Not supported.</span></span>|
|<span data-ttu-id="ba226-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba226-117">Application</span></span>|<span data-ttu-id="ba226-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba226-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba226-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba226-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ba226-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba226-120">Request headers</span></span>
|<span data-ttu-id="ba226-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba226-121">Header</span></span>|<span data-ttu-id="ba226-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ba226-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba226-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba226-123">Authorization</span></span>|<span data-ttu-id="ba226-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba226-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba226-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba226-125">Accept</span></span>|<span data-ttu-id="ba226-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba226-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba226-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba226-127">Request body</span></span>
<span data-ttu-id="ba226-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ba226-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba226-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba226-129">Response</span></span>
<span data-ttu-id="ba226-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidStoreApp](../resources/intune-apps-androidstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba226-130">If successful, this method returns a `200 OK` response code and a collection of [androidStoreApp](../resources/intune-apps-androidstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba226-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba226-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba226-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba226-132">Request</span></span>
<span data-ttu-id="ba226-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba226-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="ba226-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba226-134">Response</span></span>
<span data-ttu-id="ba226-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba226-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1615

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
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "dependentAppCount": 1,
      "packageId": "Package Id value",
      "appIdentifier": "App Identifier value",
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
  ]
}
```





