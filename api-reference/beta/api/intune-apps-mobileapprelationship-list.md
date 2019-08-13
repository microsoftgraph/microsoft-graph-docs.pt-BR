---
title: Listar mobileAppRelationships
description: Listar Propriedades e relações dos objetos mobileAppRelationship.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26edacdf301a43a422f50952ba1eba5c051cfdeb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329051"
---
# <a name="list-mobileapprelationships"></a><span data-ttu-id="c4a95-103">Listar mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="c4a95-103">List mobileAppRelationships</span></span>

> <span data-ttu-id="c4a95-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4a95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4a95-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4a95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4a95-106">Listar Propriedades e relações dos objetos [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) .</span><span class="sxs-lookup"><span data-stu-id="c4a95-106">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4a95-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4a95-107">Prerequisites</span></span>
<span data-ttu-id="c4a95-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4a95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4a95-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4a95-110">Permission type</span></span>|<span data-ttu-id="c4a95-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4a95-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4a95-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4a95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4a95-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4a95-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c4a95-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4a95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4a95-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4a95-115">Not supported.</span></span>|
|<span data-ttu-id="c4a95-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4a95-116">Application</span></span>|<span data-ttu-id="c4a95-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4a95-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4a95-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4a95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="c4a95-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a95-119">Request headers</span></span>
|<span data-ttu-id="c4a95-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4a95-120">Header</span></span>|<span data-ttu-id="c4a95-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c4a95-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4a95-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4a95-122">Authorization</span></span>|<span data-ttu-id="c4a95-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4a95-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4a95-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4a95-124">Accept</span></span>|<span data-ttu-id="c4a95-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4a95-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4a95-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a95-126">Request body</span></span>
<span data-ttu-id="c4a95-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4a95-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4a95-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4a95-128">Response</span></span>
<span data-ttu-id="c4a95-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4a95-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4a95-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4a95-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4a95-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a95-131">Request</span></span>
<span data-ttu-id="c4a95-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4a95-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

### <a name="response"></a><span data-ttu-id="c4a95-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4a95-133">Response</span></span>
<span data-ttu-id="c4a95-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4a95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppRelationship",
      "id": "7b4b5b14-5b14-7b4b-145b-4b7b145b4b7b",
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value"
    }
  ]
}
```






