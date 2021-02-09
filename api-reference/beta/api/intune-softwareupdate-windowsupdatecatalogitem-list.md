---
title: Listar windowsUpdateCatalogItems
description: Listar propriedades e relações dos objetos windowsUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8250435006295b16f841d85b0da5056e1b11b3cc
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160103"
---
# <a name="list-windowsupdatecatalogitems"></a><span data-ttu-id="13770-103">Listar windowsUpdateCatalogItems</span><span class="sxs-lookup"><span data-stu-id="13770-103">List windowsUpdateCatalogItems</span></span>

<span data-ttu-id="13770-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13770-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13770-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="13770-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13770-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13770-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13770-107">Listar propriedades e relações dos [objetos windowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="13770-107">List properties and relationships of the [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13770-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13770-108">Prerequisites</span></span>
<span data-ttu-id="13770-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13770-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13770-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13770-111">Permission type</span></span>|<span data-ttu-id="13770-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13770-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13770-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13770-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13770-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="13770-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="13770-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13770-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13770-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13770-116">Not supported.</span></span>|
|<span data-ttu-id="13770-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13770-117">Application</span></span>|<span data-ttu-id="13770-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="13770-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13770-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13770-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="13770-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13770-120">Request headers</span></span>
|<span data-ttu-id="13770-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13770-121">Header</span></span>|<span data-ttu-id="13770-122">Valor</span><span class="sxs-lookup"><span data-stu-id="13770-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13770-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="13770-123">Authorization</span></span>|<span data-ttu-id="13770-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13770-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13770-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13770-125">Accept</span></span>|<span data-ttu-id="13770-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13770-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13770-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13770-127">Request body</span></span>
<span data-ttu-id="13770-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13770-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13770-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="13770-129">Response</span></span>
<span data-ttu-id="13770-130">Se bem-sucedido, este método retorna um código de resposta e uma coleção de `200 OK` [objetos windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13770-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13770-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13770-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="13770-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13770-132">Request</span></span>
<span data-ttu-id="13770-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13770-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
```

### <a name="response"></a><span data-ttu-id="13770-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="13770-134">Response</span></span>
<span data-ttu-id="13770-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13770-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateCatalogItem",
      "id": "e887145d-145d-e887-5d14-87e85d1487e8",
      "displayName": "Display Name value",
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00"
    }
  ]
}
```




