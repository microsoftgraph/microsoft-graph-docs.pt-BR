---
title: Listar mobileAppRelationships
description: Listar propriedades e relações dos objetos mobileAppRelationship.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 463b8218ba913ffb1af6c1cd718340f12c1c32e1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139603"
---
# <a name="list-mobileapprelationships"></a><span data-ttu-id="fc7bf-103">Listar mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="fc7bf-103">List mobileAppRelationships</span></span>

<span data-ttu-id="fc7bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc7bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc7bf-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc7bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc7bf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc7bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc7bf-107">Listar propriedades e relações dos objetos [mobileAppRelationship.](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="fc7bf-107">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc7bf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fc7bf-108">Prerequisites</span></span>
<span data-ttu-id="fc7bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc7bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc7bf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc7bf-111">Permission type</span></span>|<span data-ttu-id="fc7bf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc7bf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc7bf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc7bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc7bf-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc7bf-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fc7bf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc7bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc7bf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc7bf-116">Not supported.</span></span>|
|<span data-ttu-id="fc7bf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc7bf-117">Application</span></span>|<span data-ttu-id="fc7bf-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc7bf-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc7bf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc7bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="fc7bf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc7bf-120">Request headers</span></span>
|<span data-ttu-id="fc7bf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc7bf-121">Header</span></span>|<span data-ttu-id="fc7bf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fc7bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc7bf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc7bf-123">Authorization</span></span>|<span data-ttu-id="fc7bf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc7bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc7bf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fc7bf-125">Accept</span></span>|<span data-ttu-id="fc7bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc7bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc7bf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc7bf-127">Request body</span></span>
<span data-ttu-id="fc7bf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc7bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc7bf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc7bf-129">Response</span></span>
<span data-ttu-id="fc7bf-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc7bf-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc7bf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc7bf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc7bf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc7bf-132">Request</span></span>
<span data-ttu-id="fc7bf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc7bf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

### <a name="response"></a><span data-ttu-id="fc7bf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc7bf-134">Response</span></span>
<span data-ttu-id="fc7bf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc7bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppRelationship",
      "id": "7b4b5b14-5b14-7b4b-145b-4b7b145b4b7b",
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value",
      "targetDisplayVersion": "Target Display Version value",
      "targetPublisher": "Target Publisher value",
      "targetType": "parent"
    }
  ]
}
```




