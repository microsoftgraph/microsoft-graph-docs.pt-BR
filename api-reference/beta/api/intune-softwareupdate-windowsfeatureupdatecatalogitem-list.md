---
title: Listar windowsFeatureUpdateCatalogItems
description: Listar propriedades e relações dos objetos windowsFeatureUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e23993ccedff32e9ce50e4fa210468296bca1061
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866899"
---
# <a name="list-windowsfeatureupdatecatalogitems"></a><span data-ttu-id="21f70-103">Listar windowsFeatureUpdateCatalogItems</span><span class="sxs-lookup"><span data-stu-id="21f70-103">List windowsFeatureUpdateCatalogItems</span></span>

<span data-ttu-id="21f70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21f70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21f70-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21f70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21f70-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21f70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21f70-107">Listar propriedades e relações dos [objetos windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="21f70-107">List properties and relationships of the [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21f70-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21f70-108">Prerequisites</span></span>
<span data-ttu-id="21f70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21f70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21f70-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21f70-111">Permission type</span></span>|<span data-ttu-id="21f70-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21f70-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21f70-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21f70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21f70-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21f70-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21f70-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21f70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21f70-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21f70-116">Not supported.</span></span>|
|<span data-ttu-id="21f70-117">Application</span><span class="sxs-lookup"><span data-stu-id="21f70-117">Application</span></span>|<span data-ttu-id="21f70-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21f70-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21f70-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21f70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="21f70-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21f70-120">Request headers</span></span>
|<span data-ttu-id="21f70-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21f70-121">Header</span></span>|<span data-ttu-id="21f70-122">Valor</span><span class="sxs-lookup"><span data-stu-id="21f70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21f70-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="21f70-123">Authorization</span></span>|<span data-ttu-id="21f70-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21f70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21f70-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21f70-125">Accept</span></span>|<span data-ttu-id="21f70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21f70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21f70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21f70-127">Request body</span></span>
<span data-ttu-id="21f70-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21f70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21f70-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="21f70-129">Response</span></span>
<span data-ttu-id="21f70-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21f70-130">If successful, this method returns a `200 OK` response code and a collection of [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21f70-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21f70-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="21f70-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21f70-132">Request</span></span>
<span data-ttu-id="21f70-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21f70-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
```

### <a name="response"></a><span data-ttu-id="21f70-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="21f70-134">Response</span></span>
<span data-ttu-id="21f70-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21f70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 369

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
      "id": "cbd85729-5729-cbd8-2957-d8cb2957d8cb",
      "displayName": "Display Name value",
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
      "version": "Version value"
    }
  ]
}
```




