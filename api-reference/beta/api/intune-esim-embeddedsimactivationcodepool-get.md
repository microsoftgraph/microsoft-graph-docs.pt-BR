---
title: Obter embeddedSIMActivationCodePool
description: Leia as propriedades e as relações do objeto embeddedSIMActivationCodePool.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ed067646a7f34f52c925ad7d5d1d8463fc97f7c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960101"
---
# <a name="get-embeddedsimactivationcodepool"></a><span data-ttu-id="79275-103">Obter embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="79275-103">Get embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="79275-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79275-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79275-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79275-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79275-106">Leia as propriedades e as relações do objeto [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="79275-106">Read properties and relationships of the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79275-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79275-107">Prerequisites</span></span>
<span data-ttu-id="79275-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79275-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79275-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79275-110">Permission type</span></span>|<span data-ttu-id="79275-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="79275-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79275-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79275-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79275-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79275-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="79275-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79275-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79275-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79275-115">Not supported.</span></span>|
|<span data-ttu-id="79275-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79275-116">Application</span></span>|<span data-ttu-id="79275-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79275-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79275-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79275-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79275-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="79275-119">Optional query parameters</span></span>
<span data-ttu-id="79275-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="79275-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79275-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79275-121">Request headers</span></span>
|<span data-ttu-id="79275-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79275-122">Header</span></span>|<span data-ttu-id="79275-123">Valor</span><span class="sxs-lookup"><span data-stu-id="79275-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79275-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="79275-124">Authorization</span></span>|<span data-ttu-id="79275-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79275-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79275-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79275-126">Accept</span></span>|<span data-ttu-id="79275-127">application/json</span><span class="sxs-lookup"><span data-stu-id="79275-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79275-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79275-128">Request body</span></span>
<span data-ttu-id="79275-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79275-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79275-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="79275-130">Response</span></span>
<span data-ttu-id="79275-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79275-131">If successful, this method returns a `200 OK` response code and [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79275-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79275-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="79275-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79275-133">Request</span></span>
<span data-ttu-id="79275-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79275-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

### <a name="response"></a><span data-ttu-id="79275-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="79275-135">Response</span></span>
<span data-ttu-id="79275-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79275-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": {
    "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
    "id": "ec308741-8741-ec30-4187-30ec418730ec",
    "displayName": "Display Name value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "activationCodes": [
      {
        "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
        "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
        "matchingIdentifier": "Matching Identifier value",
        "smdpPlusServerAddress": "Smdp Plus Server Address value"
      }
    ],
    "activationCodeCount": 3
  }
}
```




