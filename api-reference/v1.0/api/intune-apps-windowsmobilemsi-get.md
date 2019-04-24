---
title: Acessar windowsMobileMSI
description: Leia as propriedades e as relações do objeto windowsMobileMSI.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dbe9088261e76cd687ed6ae2dd7cd576f0b63173
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460867"
---
# <a name="get-windowsmobilemsi"></a><span data-ttu-id="1bb9c-103">Acessar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="1bb9c-103">Get windowsMobileMSI</span></span>

> <span data-ttu-id="1bb9c-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1bb9c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bb9c-105">Leia as propriedades e as relações do objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="1bb9c-105">Read properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bb9c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1bb9c-106">Prerequisites</span></span>
<span data-ttu-id="1bb9c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bb9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bb9c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bb9c-109">Permission type</span></span>|<span data-ttu-id="1bb9c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1bb9c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bb9c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bb9c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1bb9c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bb9c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1bb9c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bb9c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bb9c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bb9c-114">Not supported.</span></span>|
|<span data-ttu-id="1bb9c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bb9c-115">Application</span></span>|<span data-ttu-id="1bb9c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bb9c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bb9c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bb9c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1bb9c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1bb9c-118">Optional query parameters</span></span>
<span data-ttu-id="1bb9c-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1bb9c-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1bb9c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb9c-120">Request headers</span></span>
|<span data-ttu-id="1bb9c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1bb9c-121">Header</span></span>|<span data-ttu-id="1bb9c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1bb9c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bb9c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bb9c-123">Authorization</span></span>|<span data-ttu-id="1bb9c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bb9c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bb9c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1bb9c-125">Accept</span></span>|<span data-ttu-id="1bb9c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bb9c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bb9c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb9c-127">Request body</span></span>
<span data-ttu-id="1bb9c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1bb9c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bb9c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bb9c-129">Response</span></span>
<span data-ttu-id="1bb9c-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bb9c-130">If successful, this method returns a `200 OK` response code and [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bb9c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bb9c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bb9c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb9c-132">Request</span></span>
<span data-ttu-id="1bb9c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bb9c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="1bb9c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bb9c-134">Response</span></span>
<span data-ttu-id="1bb9c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bb9c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1098

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsMobileMSI",
    "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
    "commandLine": "Command Line value",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "ignoreVersionDetection": true
  }
}
```



