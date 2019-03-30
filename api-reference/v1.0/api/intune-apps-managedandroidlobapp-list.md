---
title: Listar managedAndroidLobApps
description: Listar propriedades e relações dos objetos managedAndroidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83bccc0e670db6e7ed3db144854a887514a95f00
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987136"
---
# <a name="list-managedandroidlobapps"></a><span data-ttu-id="5131e-103">Listar managedAndroidLobApps</span><span class="sxs-lookup"><span data-stu-id="5131e-103">List managedAndroidLobApps</span></span>

> <span data-ttu-id="5131e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5131e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5131e-105">Listar propriedades e relações dos objetos [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5131e-105">List properties and relationships of the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5131e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5131e-106">Prerequisites</span></span>
<span data-ttu-id="5131e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5131e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5131e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5131e-109">Permission type</span></span>|<span data-ttu-id="5131e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5131e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5131e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5131e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5131e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5131e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5131e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5131e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5131e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5131e-114">Not supported.</span></span>|
|<span data-ttu-id="5131e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5131e-115">Application</span></span>|<span data-ttu-id="5131e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5131e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5131e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5131e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5131e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5131e-118">Request headers</span></span>
|<span data-ttu-id="5131e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5131e-119">Header</span></span>|<span data-ttu-id="5131e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5131e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5131e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5131e-121">Authorization</span></span>|<span data-ttu-id="5131e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5131e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5131e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5131e-123">Accept</span></span>|<span data-ttu-id="5131e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5131e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5131e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5131e-125">Request body</span></span>
<span data-ttu-id="5131e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5131e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5131e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5131e-127">Response</span></span>
<span data-ttu-id="5131e-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5131e-128">If successful, this method returns a `200 OK` response code and a collection of [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5131e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5131e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="5131e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5131e-130">Request</span></span>
<span data-ttu-id="5131e-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5131e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="5131e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5131e-132">Response</span></span>
<span data-ttu-id="5131e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5131e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1510

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAndroidLobApp",
      "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
      "packageId": "Package Id value",
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
      },
      "versionName": "Version Name value",
      "versionCode": "Version Code value"
    }
  ]
}
```



