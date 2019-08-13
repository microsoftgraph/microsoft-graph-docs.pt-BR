---
title: Acessar mobileAppContentFile
description: Leia as propriedades e as relações do objeto mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ce91ccc0e7e37c34f012b3d861dc8ed589644d78
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329191"
---
# <a name="get-mobileappcontentfile"></a><span data-ttu-id="060a4-103">Acessar mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="060a4-103">Get mobileAppContentFile</span></span>

> <span data-ttu-id="060a4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="060a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="060a4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="060a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="060a4-106">Leia as propriedades e as relações do objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="060a4-106">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="060a4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="060a4-107">Prerequisites</span></span>
<span data-ttu-id="060a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="060a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="060a4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="060a4-110">Permission type</span></span>|<span data-ttu-id="060a4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="060a4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="060a4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="060a4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="060a4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="060a4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="060a4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="060a4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="060a4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="060a4-115">Not supported.</span></span>|
|<span data-ttu-id="060a4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="060a4-116">Application</span></span>|<span data-ttu-id="060a4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="060a4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="060a4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="060a4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="060a4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="060a4-119">Optional query parameters</span></span>
<span data-ttu-id="060a4-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="060a4-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="060a4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="060a4-121">Request headers</span></span>
|<span data-ttu-id="060a4-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="060a4-122">Header</span></span>|<span data-ttu-id="060a4-123">Valor</span><span class="sxs-lookup"><span data-stu-id="060a4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="060a4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="060a4-124">Authorization</span></span>|<span data-ttu-id="060a4-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="060a4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="060a4-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="060a4-126">Accept</span></span>|<span data-ttu-id="060a4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="060a4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="060a4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="060a4-128">Request body</span></span>
<span data-ttu-id="060a4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="060a4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="060a4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="060a4-130">Response</span></span>
<span data-ttu-id="060a4-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="060a4-131">If successful, this method returns a `200 OK` response code and [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="060a4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="060a4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="060a4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="060a4-133">Request</span></span>
<span data-ttu-id="060a4-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="060a4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

### <a name="response"></a><span data-ttu-id="060a4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="060a4-135">Response</span></span>
<span data-ttu-id="060a4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="060a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 548

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppContentFile",
    "azureStorageUri": "Azure Storage Uri value",
    "isCommitted": true,
    "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "name": "Name value",
    "size": 4,
    "sizeEncrypted": 13,
    "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
    "manifest": "bWFuaWZlc3Q=",
    "uploadState": "transientError",
    "isFrameworkFile": true,
    "isDependency": true
  }
}
```






