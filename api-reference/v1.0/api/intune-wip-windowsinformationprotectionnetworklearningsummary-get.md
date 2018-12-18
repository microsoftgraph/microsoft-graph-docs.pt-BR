---
title: Acessar windowsInformationProtectionNetworkLearningSummary
description: Leia as propriedades e as relações do objeto windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
ms.openlocfilehash: 46c255b5e59ab4245b1945d588bc15b36b55aec8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332127"
---
# <a name="get-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="da6c3-103">Acessar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="da6c3-103">Get windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="da6c3-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="da6c3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da6c3-105">Leia as propriedades e as relações do objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="da6c3-105">Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da6c3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da6c3-106">Prerequisites</span></span>
<span data-ttu-id="da6c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da6c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da6c3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da6c3-109">Permission type</span></span>|<span data-ttu-id="da6c3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da6c3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da6c3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da6c3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="da6c3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="da6c3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="da6c3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da6c3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da6c3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da6c3-114">Not supported.</span></span>|
|<span data-ttu-id="da6c3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da6c3-115">Application</span></span>|<span data-ttu-id="da6c3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da6c3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da6c3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da6c3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da6c3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da6c3-118">Optional query parameters</span></span>
<span data-ttu-id="da6c3-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da6c3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="da6c3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da6c3-120">Request headers</span></span>
|<span data-ttu-id="da6c3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da6c3-121">Header</span></span>|<span data-ttu-id="da6c3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="da6c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da6c3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="da6c3-123">Authorization</span></span>|<span data-ttu-id="da6c3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da6c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da6c3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="da6c3-125">Accept</span></span>|<span data-ttu-id="da6c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da6c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da6c3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da6c3-127">Request body</span></span>
<span data-ttu-id="da6c3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da6c3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da6c3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="da6c3-129">Response</span></span>
<span data-ttu-id="da6c3-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da6c3-130">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da6c3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da6c3-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="da6c3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da6c3-132">Request</span></span>
<span data-ttu-id="da6c3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da6c3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="da6c3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="da6c3-134">Response</span></span>
<span data-ttu-id="da6c3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da6c3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



