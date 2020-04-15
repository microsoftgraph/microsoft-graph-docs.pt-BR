---
title: Acessar windowsInformationProtectionNetworkLearningSummary
description: Leia as propriedades e as relações do objeto windowsInformationProtectionNetworkLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bc5fbd9585c591b4171d7f26c92fca0660e36929
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461122"
---
# <a name="get-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="25b83-103">Acessar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="25b83-103">Get windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="25b83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25b83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25b83-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25b83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25b83-106">Leia as propriedades e as relações do objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="25b83-106">Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25b83-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25b83-107">Prerequisites</span></span>
<span data-ttu-id="25b83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25b83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25b83-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25b83-110">Permission type</span></span>|<span data-ttu-id="25b83-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="25b83-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25b83-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25b83-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25b83-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="25b83-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="25b83-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25b83-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25b83-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25b83-115">Not supported.</span></span>|
|<span data-ttu-id="25b83-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25b83-116">Application</span></span>|<span data-ttu-id="25b83-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25b83-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25b83-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25b83-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="25b83-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="25b83-119">Optional query parameters</span></span>
<span data-ttu-id="25b83-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="25b83-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25b83-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25b83-121">Request headers</span></span>
|<span data-ttu-id="25b83-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25b83-122">Header</span></span>|<span data-ttu-id="25b83-123">Valor</span><span class="sxs-lookup"><span data-stu-id="25b83-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25b83-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="25b83-124">Authorization</span></span>|<span data-ttu-id="25b83-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25b83-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25b83-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="25b83-126">Accept</span></span>|<span data-ttu-id="25b83-127">application/json</span><span class="sxs-lookup"><span data-stu-id="25b83-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25b83-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25b83-128">Request body</span></span>
<span data-ttu-id="25b83-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25b83-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25b83-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="25b83-130">Response</span></span>
<span data-ttu-id="25b83-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25b83-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25b83-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25b83-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="25b83-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25b83-133">Request</span></span>
<span data-ttu-id="25b83-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25b83-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="25b83-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="25b83-135">Response</span></span>
<span data-ttu-id="25b83-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25b83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






