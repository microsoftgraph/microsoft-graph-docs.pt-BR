---
title: Acessar windowsInformationProtectionNetworkLearningSummary
description: Leia as propriedades e as relações do objeto windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dbe9f7e9a5d7989b8741d92b5692ebd0fd28643
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792878"
---
# <a name="get-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="6a60e-103">Acessar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="6a60e-103">Get windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="6a60e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a60e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a60e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a60e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a60e-106">Leia as propriedades e as relações do objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="6a60e-106">Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a60e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a60e-107">Prerequisites</span></span>
<span data-ttu-id="6a60e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a60e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a60e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a60e-110">Permission type</span></span>|<span data-ttu-id="6a60e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a60e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a60e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a60e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a60e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a60e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6a60e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a60e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a60e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a60e-115">Not supported.</span></span>|
|<span data-ttu-id="6a60e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a60e-116">Application</span></span>|<span data-ttu-id="6a60e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a60e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a60e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a60e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a60e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a60e-119">Optional query parameters</span></span>
<span data-ttu-id="6a60e-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a60e-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a60e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a60e-121">Request headers</span></span>
|<span data-ttu-id="6a60e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a60e-122">Header</span></span>|<span data-ttu-id="6a60e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6a60e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a60e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a60e-124">Authorization</span></span>|<span data-ttu-id="6a60e-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a60e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a60e-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a60e-126">Accept</span></span>|<span data-ttu-id="6a60e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6a60e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a60e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a60e-128">Request body</span></span>
<span data-ttu-id="6a60e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a60e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a60e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a60e-130">Response</span></span>
<span data-ttu-id="6a60e-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a60e-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a60e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a60e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a60e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a60e-133">Request</span></span>
<span data-ttu-id="6a60e-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a60e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="6a60e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a60e-135">Response</span></span>
<span data-ttu-id="6a60e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a60e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 213

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
    "id": "242108f7-08f7-2421-f708-2124f7082124",
    "url": "Url value",
    "deviceCount": 11
  }
}
```





