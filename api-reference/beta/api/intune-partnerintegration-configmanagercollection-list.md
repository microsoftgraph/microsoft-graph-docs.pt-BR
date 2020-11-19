---
title: Listar configManagerCollections
description: Listar Propriedades e relações dos objetos configManagerCollection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 165ed79f911fb0ef8505d75029e28cdf1003eb93
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49336985"
---
# <a name="list-configmanagercollections"></a><span data-ttu-id="d7564-103">Listar configManagerCollections</span><span class="sxs-lookup"><span data-stu-id="d7564-103">List configManagerCollections</span></span>

<span data-ttu-id="d7564-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7564-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7564-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d7564-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7564-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7564-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7564-107">Listar Propriedades e relações dos objetos [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) .</span><span class="sxs-lookup"><span data-stu-id="d7564-107">List properties and relationships of the [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7564-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7564-108">Prerequisites</span></span>
<span data-ttu-id="d7564-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7564-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7564-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7564-111">Permission type</span></span>|<span data-ttu-id="d7564-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d7564-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7564-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7564-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7564-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7564-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d7564-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7564-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7564-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7564-116">Not supported.</span></span>|
|<span data-ttu-id="d7564-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7564-117">Application</span></span>|<span data-ttu-id="d7564-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7564-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7564-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7564-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configManagerCollections
```

## <a name="request-headers"></a><span data-ttu-id="d7564-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7564-120">Request headers</span></span>
|<span data-ttu-id="d7564-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7564-121">Header</span></span>|<span data-ttu-id="d7564-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d7564-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7564-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7564-123">Authorization</span></span>|<span data-ttu-id="d7564-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7564-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7564-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d7564-125">Accept</span></span>|<span data-ttu-id="d7564-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7564-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7564-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7564-127">Request body</span></span>
<span data-ttu-id="d7564-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d7564-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7564-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7564-129">Response</span></span>
<span data-ttu-id="d7564-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7564-130">If successful, this method returns a `200 OK` response code and a collection of [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7564-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7564-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7564-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7564-132">Request</span></span>
<span data-ttu-id="d7564-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7564-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configManagerCollections
```

### <a name="response"></a><span data-ttu-id="d7564-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7564-134">Response</span></span>
<span data-ttu-id="d7564-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7564-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 500

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.configManagerCollection",
      "id": "5f9d1d76-1d76-5f9d-761d-9d5f761d9d5f",
      "displayName": "Display Name value",
      "collectionIdentifier": "Collection Identifier value",
      "hierarchyName": "Hierarchy Name value",
      "hierarchyIdentifier": "Hierarchy Identifier value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




