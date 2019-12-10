---
title: Listar mobileAppContentFiles
description: Listar propriedades e relações dos objetos mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c80821a354098b1e0ea59e061e5da14264636ed
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39935418"
---
# <a name="list-mobileappcontentfiles"></a><span data-ttu-id="96db1-103">Listar mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="96db1-103">List mobileAppContentFiles</span></span>

> <span data-ttu-id="96db1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="96db1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96db1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96db1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96db1-106">Listar propriedades e relações dos objetos [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="96db1-106">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96db1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96db1-107">Prerequisites</span></span>
<span data-ttu-id="96db1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96db1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96db1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96db1-110">Permission type</span></span>|<span data-ttu-id="96db1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96db1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96db1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96db1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96db1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="96db1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="96db1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96db1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96db1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96db1-115">Not supported.</span></span>|
|<span data-ttu-id="96db1-116">Application</span><span class="sxs-lookup"><span data-stu-id="96db1-116">Application</span></span>|<span data-ttu-id="96db1-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="96db1-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96db1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96db1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="96db1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96db1-119">Request headers</span></span>
|<span data-ttu-id="96db1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96db1-120">Header</span></span>|<span data-ttu-id="96db1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="96db1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96db1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="96db1-122">Authorization</span></span>|<span data-ttu-id="96db1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96db1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96db1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96db1-124">Accept</span></span>|<span data-ttu-id="96db1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="96db1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96db1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96db1-126">Request body</span></span>
<span data-ttu-id="96db1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96db1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96db1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="96db1-128">Response</span></span>
<span data-ttu-id="96db1-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96db1-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96db1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96db1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="96db1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96db1-131">Request</span></span>
<span data-ttu-id="96db1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96db1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### <a name="response"></a><span data-ttu-id="96db1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="96db1-133">Response</span></span>
<span data-ttu-id="96db1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96db1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 588

{
  "value": [
    {
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
  ]
}
```





