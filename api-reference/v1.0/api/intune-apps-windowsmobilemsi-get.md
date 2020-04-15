---
title: Acessar windowsMobileMSI
description: Leia as propriedades e as relações do objeto windowsMobileMSI.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 862f0b076ea93a7260e00411f18a1980f8a3e074
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464522"
---
# <a name="get-windowsmobilemsi"></a><span data-ttu-id="d49ec-103">Acessar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="d49ec-103">Get windowsMobileMSI</span></span>

<span data-ttu-id="d49ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d49ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d49ec-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d49ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d49ec-106">Leia as propriedades e as relações do objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="d49ec-106">Read properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d49ec-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d49ec-107">Prerequisites</span></span>
<span data-ttu-id="d49ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d49ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d49ec-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d49ec-110">Permission type</span></span>|<span data-ttu-id="d49ec-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d49ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d49ec-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d49ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d49ec-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d49ec-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d49ec-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d49ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d49ec-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d49ec-115">Not supported.</span></span>|
|<span data-ttu-id="d49ec-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d49ec-116">Application</span></span>|<span data-ttu-id="d49ec-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d49ec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d49ec-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d49ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d49ec-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d49ec-119">Optional query parameters</span></span>
<span data-ttu-id="d49ec-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d49ec-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d49ec-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d49ec-121">Request headers</span></span>
|<span data-ttu-id="d49ec-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d49ec-122">Header</span></span>|<span data-ttu-id="d49ec-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d49ec-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d49ec-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d49ec-124">Authorization</span></span>|<span data-ttu-id="d49ec-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d49ec-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d49ec-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d49ec-126">Accept</span></span>|<span data-ttu-id="d49ec-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d49ec-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d49ec-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d49ec-128">Request body</span></span>
<span data-ttu-id="d49ec-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d49ec-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d49ec-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d49ec-130">Response</span></span>
<span data-ttu-id="d49ec-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d49ec-131">If successful, this method returns a `200 OK` response code and [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d49ec-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d49ec-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d49ec-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d49ec-133">Request</span></span>
<span data-ttu-id="d49ec-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d49ec-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="d49ec-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d49ec-135">Response</span></span>
<span data-ttu-id="d49ec-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d49ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






