---
title: Acessar androidLobApp
description: Leia as propriedades e as relações do objeto androidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b412e7675ad4a5af77207af6514364419de1ab18
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983846"
---
# <a name="get-androidlobapp"></a><span data-ttu-id="8f2b3-103">Acessar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="8f2b3-103">Get androidLobApp</span></span>

> <span data-ttu-id="8f2b3-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8f2b3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f2b3-105">Leia as propriedades e as relações do objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f2b3-105">Read properties and relationships of the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f2b3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8f2b3-106">Prerequisites</span></span>
<span data-ttu-id="8f2b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f2b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f2b3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f2b3-109">Permission type</span></span>|<span data-ttu-id="8f2b3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8f2b3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f2b3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f2b3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8f2b3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f2b3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8f2b3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f2b3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f2b3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f2b3-114">Not supported.</span></span>|
|<span data-ttu-id="8f2b3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f2b3-115">Application</span></span>|<span data-ttu-id="8f2b3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f2b3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f2b3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f2b3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f2b3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8f2b3-118">Optional query parameters</span></span>
<span data-ttu-id="8f2b3-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8f2b3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8f2b3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f2b3-120">Request headers</span></span>
|<span data-ttu-id="8f2b3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f2b3-121">Header</span></span>|<span data-ttu-id="8f2b3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8f2b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f2b3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f2b3-123">Authorization</span></span>|<span data-ttu-id="8f2b3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f2b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f2b3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8f2b3-125">Accept</span></span>|<span data-ttu-id="8f2b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f2b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f2b3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f2b3-127">Request body</span></span>
<span data-ttu-id="8f2b3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f2b3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f2b3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f2b3-129">Response</span></span>
<span data-ttu-id="8f2b3-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f2b3-130">If successful, this method returns a `200 OK` response code and [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f2b3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f2b3-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f2b3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f2b3-132">Request</span></span>
<span data-ttu-id="8f2b3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f2b3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="8f2b3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f2b3-134">Response</span></span>
<span data-ttu-id="8f2b3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f2b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1338

{
  "value": {
    "@odata.type": "#microsoft.graph.androidLobApp",
    "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
}
```



