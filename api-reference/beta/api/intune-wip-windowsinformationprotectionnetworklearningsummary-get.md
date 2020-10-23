---
title: Acessar windowsInformationProtectionNetworkLearningSummary
description: Leia as propriedades e as relações do objeto windowsInformationProtectionNetworkLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fd2d4ff2c50ac0c929f32f118cb17c27a863810c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692615"
---
# <a name="get-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="a7e63-103">Acessar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="a7e63-103">Get windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="a7e63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7e63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7e63-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a7e63-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7e63-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a7e63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7e63-107">Leia as propriedades e as relações do objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a7e63-107">Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7e63-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a7e63-108">Prerequisites</span></span>
<span data-ttu-id="a7e63-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7e63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7e63-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7e63-111">Permission type</span></span>|<span data-ttu-id="a7e63-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a7e63-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7e63-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7e63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7e63-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7e63-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a7e63-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7e63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7e63-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7e63-116">Not supported.</span></span>|
|<span data-ttu-id="a7e63-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7e63-117">Application</span></span>|<span data-ttu-id="a7e63-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7e63-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7e63-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7e63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7e63-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a7e63-120">Optional query parameters</span></span>
<span data-ttu-id="a7e63-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a7e63-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7e63-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7e63-122">Request headers</span></span>
|<span data-ttu-id="a7e63-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7e63-123">Header</span></span>|<span data-ttu-id="a7e63-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a7e63-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7e63-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7e63-125">Authorization</span></span>|<span data-ttu-id="a7e63-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7e63-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7e63-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a7e63-127">Accept</span></span>|<span data-ttu-id="a7e63-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a7e63-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7e63-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7e63-129">Request body</span></span>
<span data-ttu-id="a7e63-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7e63-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7e63-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7e63-131">Response</span></span>
<span data-ttu-id="a7e63-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7e63-132">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7e63-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7e63-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7e63-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7e63-134">Request</span></span>
<span data-ttu-id="a7e63-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7e63-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="a7e63-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7e63-136">Response</span></span>
<span data-ttu-id="a7e63-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7e63-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





