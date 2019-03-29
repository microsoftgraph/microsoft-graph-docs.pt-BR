---
title: Acessar windowsInformationProtectionNetworkLearningSummary
description: Leia as propriedades e as relações do objeto windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4d10d3ec64a19a97c8dfbe3467eb25f3c950728
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971938"
---
# <a name="get-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="c0640-103">Acessar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="c0640-103">Get windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="c0640-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0640-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0640-105">Leia as propriedades e as relações do objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c0640-105">Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0640-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0640-106">Prerequisites</span></span>
<span data-ttu-id="c0640-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0640-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0640-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0640-109">Permission type</span></span>|<span data-ttu-id="c0640-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0640-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0640-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0640-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c0640-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0640-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c0640-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0640-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0640-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0640-114">Not supported.</span></span>|
|<span data-ttu-id="c0640-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0640-115">Application</span></span>|<span data-ttu-id="c0640-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0640-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0640-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0640-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0640-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c0640-118">Optional query parameters</span></span>
<span data-ttu-id="c0640-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c0640-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0640-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0640-120">Request headers</span></span>
|<span data-ttu-id="c0640-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0640-121">Header</span></span>|<span data-ttu-id="c0640-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c0640-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0640-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0640-123">Authorization</span></span>|<span data-ttu-id="c0640-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0640-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0640-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0640-125">Accept</span></span>|<span data-ttu-id="c0640-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0640-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0640-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0640-127">Request body</span></span>
<span data-ttu-id="c0640-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0640-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0640-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0640-129">Response</span></span>
<span data-ttu-id="c0640-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0640-130">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0640-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0640-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0640-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0640-132">Request</span></span>
<span data-ttu-id="c0640-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0640-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="c0640-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0640-134">Response</span></span>
<span data-ttu-id="c0640-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0640-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



