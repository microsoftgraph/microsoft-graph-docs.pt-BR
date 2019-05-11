---
title: Listar mobileAppContentFiles
description: Listar propriedades e relações dos objetos mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b9116a0eafd6cb8dca6268a2c09e3707838e833
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935164"
---
# <a name="list-mobileappcontentfiles"></a><span data-ttu-id="9de26-103">Listar mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="9de26-103">List mobileAppContentFiles</span></span>

> <span data-ttu-id="9de26-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9de26-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9de26-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9de26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9de26-106">Listar propriedades e relações dos objetos [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="9de26-106">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9de26-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9de26-107">Prerequisites</span></span>
<span data-ttu-id="9de26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9de26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9de26-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9de26-110">Permission type</span></span>|<span data-ttu-id="9de26-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9de26-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9de26-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9de26-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9de26-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9de26-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9de26-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9de26-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9de26-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9de26-115">Not supported.</span></span>|
|<span data-ttu-id="9de26-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9de26-116">Application</span></span>|<span data-ttu-id="9de26-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9de26-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9de26-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9de26-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="9de26-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9de26-119">Request headers</span></span>
|<span data-ttu-id="9de26-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9de26-120">Header</span></span>|<span data-ttu-id="9de26-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9de26-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9de26-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9de26-122">Authorization</span></span>|<span data-ttu-id="9de26-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9de26-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9de26-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9de26-124">Accept</span></span>|<span data-ttu-id="9de26-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9de26-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9de26-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9de26-126">Request body</span></span>
<span data-ttu-id="9de26-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9de26-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9de26-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9de26-128">Response</span></span>
<span data-ttu-id="9de26-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9de26-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9de26-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9de26-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9de26-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9de26-131">Request</span></span>
<span data-ttu-id="9de26-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9de26-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### <a name="response"></a><span data-ttu-id="9de26-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9de26-133">Response</span></span>
<span data-ttu-id="9de26-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9de26-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




