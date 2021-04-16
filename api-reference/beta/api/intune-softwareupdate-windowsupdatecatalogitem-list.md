---
title: Listar windowsUpdateCatalogItems
description: Listar propriedades e relações dos objetos windowsUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f4be6933c7218fdf4c51e2172aa7b487a7718b0
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865625"
---
# <a name="list-windowsupdatecatalogitems"></a><span data-ttu-id="a6467-103">Listar windowsUpdateCatalogItems</span><span class="sxs-lookup"><span data-stu-id="a6467-103">List windowsUpdateCatalogItems</span></span>

<span data-ttu-id="a6467-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6467-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6467-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6467-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6467-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6467-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6467-107">Listar propriedades e relações dos [objetos windowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="a6467-107">List properties and relationships of the [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6467-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6467-108">Prerequisites</span></span>
<span data-ttu-id="a6467-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6467-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6467-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6467-111">Permission type</span></span>|<span data-ttu-id="a6467-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6467-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6467-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6467-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6467-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6467-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6467-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6467-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6467-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6467-116">Not supported.</span></span>|
|<span data-ttu-id="a6467-117">Application</span><span class="sxs-lookup"><span data-stu-id="a6467-117">Application</span></span>|<span data-ttu-id="a6467-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6467-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6467-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6467-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="a6467-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6467-120">Request headers</span></span>
|<span data-ttu-id="a6467-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6467-121">Header</span></span>|<span data-ttu-id="a6467-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a6467-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6467-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6467-123">Authorization</span></span>|<span data-ttu-id="a6467-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6467-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6467-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6467-125">Accept</span></span>|<span data-ttu-id="a6467-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6467-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6467-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6467-127">Request body</span></span>
<span data-ttu-id="a6467-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6467-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6467-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6467-129">Response</span></span>
<span data-ttu-id="a6467-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6467-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6467-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6467-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6467-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6467-132">Request</span></span>
<span data-ttu-id="a6467-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6467-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
```

### <a name="response"></a><span data-ttu-id="a6467-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6467-134">Response</span></span>
<span data-ttu-id="a6467-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6467-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 327

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateCatalogItem",
      "id": "e887145d-145d-e887-5d14-87e85d1487e8",
      "displayName": "Display Name value",
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00"
    }
  ]
}
```




