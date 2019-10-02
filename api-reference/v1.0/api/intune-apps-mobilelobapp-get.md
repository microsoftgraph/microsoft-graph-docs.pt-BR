---
title: Acessar mobileLobApp
description: Leia as propriedades e as relações do objeto mobileLobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9e777471e47dcc6a5e47121568f9afb02111e080
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358183"
---
# <a name="get-mobilelobapp"></a><span data-ttu-id="a5ed2-103">Acessar mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="a5ed2-103">Get mobileLobApp</span></span>

> <span data-ttu-id="a5ed2-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5ed2-105">Leia as propriedades e as relações do objeto [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a5ed2-105">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5ed2-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a5ed2-106">Prerequisites</span></span>
<span data-ttu-id="a5ed2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5ed2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5ed2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5ed2-109">Permission type</span></span>|<span data-ttu-id="a5ed2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a5ed2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5ed2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5ed2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a5ed2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5ed2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a5ed2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5ed2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5ed2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-114">Not supported.</span></span>|
|<span data-ttu-id="a5ed2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5ed2-115">Application</span></span>|<span data-ttu-id="a5ed2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5ed2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5ed2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5ed2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a5ed2-118">Optional query parameters</span></span>
<span data-ttu-id="a5ed2-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5ed2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ed2-120">Request headers</span></span>
|<span data-ttu-id="a5ed2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5ed2-121">Header</span></span>|<span data-ttu-id="a5ed2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a5ed2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5ed2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5ed2-123">Authorization</span></span>|<span data-ttu-id="a5ed2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5ed2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a5ed2-125">Accept</span></span>|<span data-ttu-id="a5ed2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5ed2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5ed2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ed2-127">Request body</span></span>
<span data-ttu-id="a5ed2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5ed2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5ed2-129">Response</span></span>
<span data-ttu-id="a5ed2-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileLobApp](../resources/intune-apps-mobilelobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-130">If successful, this method returns a `200 OK` response code and [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5ed2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5ed2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5ed2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ed2-132">Request</span></span>
<span data-ttu-id="a5ed2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="a5ed2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5ed2-134">Response</span></span>
<span data-ttu-id="a5ed2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 925

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileLobApp",
    "id": "2fc11935-1935-2fc1-3519-c12f3519c12f",
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
    "size": 4
  }
}
```




