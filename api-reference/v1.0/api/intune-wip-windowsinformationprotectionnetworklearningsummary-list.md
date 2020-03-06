---
title: Listar windowsInformationProtectionNetworkLearningSummaries
description: Listar propriedades e relações de objetos de windowsInformationProtectionNetworkLearningSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f3172f7d07deeb8d1131dd2d97bf5b79e9ab9c09
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511772"
---
# <a name="list-windowsinformationprotectionnetworklearningsummaries"></a><span data-ttu-id="a47ef-103">Listar windowsInformationProtectionNetworkLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="a47ef-103">List windowsInformationProtectionNetworkLearningSummaries</span></span>

<span data-ttu-id="a47ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a47ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a47ef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a47ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a47ef-106">Listar propriedades e relações de objetos de [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a47ef-106">List properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a47ef-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a47ef-107">Prerequisites</span></span>
<span data-ttu-id="a47ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a47ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a47ef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a47ef-110">Permission type</span></span>|<span data-ttu-id="a47ef-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a47ef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a47ef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a47ef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a47ef-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a47ef-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a47ef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a47ef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a47ef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a47ef-115">Not supported.</span></span>|
|<span data-ttu-id="a47ef-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a47ef-116">Application</span></span>|<span data-ttu-id="a47ef-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a47ef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a47ef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a47ef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="a47ef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a47ef-119">Request headers</span></span>
|<span data-ttu-id="a47ef-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a47ef-120">Header</span></span>|<span data-ttu-id="a47ef-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a47ef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a47ef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a47ef-122">Authorization</span></span>|<span data-ttu-id="a47ef-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a47ef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a47ef-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a47ef-124">Accept</span></span>|<span data-ttu-id="a47ef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a47ef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a47ef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a47ef-126">Request body</span></span>
<span data-ttu-id="a47ef-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a47ef-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a47ef-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a47ef-128">Response</span></span>
<span data-ttu-id="a47ef-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a47ef-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a47ef-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a47ef-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a47ef-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a47ef-131">Request</span></span>
<span data-ttu-id="a47ef-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a47ef-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

### <a name="response"></a><span data-ttu-id="a47ef-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a47ef-133">Response</span></span>
<span data-ttu-id="a47ef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a47ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 235

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
      "id": "242108f7-08f7-2421-f708-2124f7082124",
      "url": "Url value",
      "deviceCount": 11
    }
  ]
}
```




