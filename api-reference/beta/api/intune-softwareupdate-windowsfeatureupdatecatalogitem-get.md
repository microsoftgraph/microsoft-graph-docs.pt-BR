---
title: Obter windowsFeatureUpdateCatalogItem
description: Ler propriedades e relações do objeto windowsFeatureUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3007fdf3fff4b1670e217e8e0e7c60a1d827a331
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866927"
---
# <a name="get-windowsfeatureupdatecatalogitem"></a><span data-ttu-id="61063-103">Obter windowsFeatureUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="61063-103">Get windowsFeatureUpdateCatalogItem</span></span>

<span data-ttu-id="61063-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61063-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61063-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61063-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61063-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61063-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61063-107">Ler propriedades e relações do [objeto windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="61063-107">Read properties and relationships of the [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61063-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61063-108">Prerequisites</span></span>
<span data-ttu-id="61063-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61063-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61063-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61063-111">Permission type</span></span>|<span data-ttu-id="61063-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61063-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61063-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61063-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61063-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61063-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="61063-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61063-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61063-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61063-116">Not supported.</span></span>|
|<span data-ttu-id="61063-117">Application</span><span class="sxs-lookup"><span data-stu-id="61063-117">Application</span></span>|<span data-ttu-id="61063-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61063-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61063-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61063-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61063-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="61063-120">Optional query parameters</span></span>
<span data-ttu-id="61063-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="61063-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61063-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61063-122">Request headers</span></span>
|<span data-ttu-id="61063-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61063-123">Header</span></span>|<span data-ttu-id="61063-124">Valor</span><span class="sxs-lookup"><span data-stu-id="61063-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61063-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="61063-125">Authorization</span></span>|<span data-ttu-id="61063-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61063-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61063-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61063-127">Accept</span></span>|<span data-ttu-id="61063-128">application/json</span><span class="sxs-lookup"><span data-stu-id="61063-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61063-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61063-129">Request body</span></span>
<span data-ttu-id="61063-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61063-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61063-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="61063-131">Response</span></span>
<span data-ttu-id="61063-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61063-132">If successful, this method returns a `200 OK` response code and [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61063-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61063-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="61063-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61063-134">Request</span></span>
<span data-ttu-id="61063-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61063-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

### <a name="response"></a><span data-ttu-id="61063-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="61063-136">Response</span></span>
<span data-ttu-id="61063-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61063-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 343

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
    "id": "cbd85729-5729-cbd8-2957-d8cb2957d8cb",
    "displayName": "Display Name value",
    "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
    "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
    "version": "Version value"
  }
}
```




