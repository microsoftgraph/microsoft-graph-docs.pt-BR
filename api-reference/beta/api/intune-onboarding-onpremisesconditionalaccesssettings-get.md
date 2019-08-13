---
title: Obter onPremisesConditionalAccessSettings
description: Ler propriedades e relações do objeto onPremisesConditionalAccessSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b92de88137ceb80802e5cdb51346ccea7758fb9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352550"
---
# <a name="get-onpremisesconditionalaccesssettings"></a><span data-ttu-id="7a835-103">Obter onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="7a835-103">Get onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="7a835-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7a835-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a835-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a835-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a835-106">Ler propriedades e relações do objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="7a835-106">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a835-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7a835-107">Prerequisites</span></span>
<span data-ttu-id="7a835-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a835-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a835-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a835-110">Permission type</span></span>|<span data-ttu-id="7a835-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7a835-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a835-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a835-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7a835-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a835-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7a835-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a835-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a835-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a835-115">Not supported.</span></span>|
|<span data-ttu-id="7a835-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a835-116">Application</span></span>|<span data-ttu-id="7a835-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a835-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a835-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a835-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/conditionalAccessSettings
GET /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a835-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7a835-119">Optional query parameters</span></span>
<span data-ttu-id="7a835-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7a835-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a835-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a835-121">Request headers</span></span>
|<span data-ttu-id="7a835-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a835-122">Header</span></span>|<span data-ttu-id="7a835-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7a835-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a835-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a835-124">Authorization</span></span>|<span data-ttu-id="7a835-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a835-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a835-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7a835-126">Accept</span></span>|<span data-ttu-id="7a835-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7a835-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a835-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a835-128">Request body</span></span>
<span data-ttu-id="7a835-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a835-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a835-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a835-130">Response</span></span>
<span data-ttu-id="7a835-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a835-131">If successful, this method returns a `200 OK` response code and [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a835-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a835-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a835-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a835-133">Request</span></span>
<span data-ttu-id="7a835-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a835-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
```

### <a name="response"></a><span data-ttu-id="7a835-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a835-135">Response</span></span>
<span data-ttu-id="7a835-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a835-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
    "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
    "enabled": true,
    "includedGroups": [
      "77c9d466-d466-77c9-66d4-c97766d4c977"
    ],
    "excludedGroups": [
      "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
    ],
    "overrideDefaultRule": true
  }
}
```






