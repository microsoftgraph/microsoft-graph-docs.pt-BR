---
title: Obter embeddedSIMActivationCodePool
description: Leia as propriedades e as relações do objeto embeddedSIMActivationCodePool.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d1846aca8ed6c4498460a181657015e7b8d6ce54
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709422"
---
# <a name="get-embeddedsimactivationcodepool"></a><span data-ttu-id="b9c83-103">Obter embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="b9c83-103">Get embeddedSIMActivationCodePool</span></span>

<span data-ttu-id="b9c83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9c83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9c83-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9c83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9c83-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9c83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9c83-107">Leia as propriedades e as relações do objeto [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="b9c83-107">Read properties and relationships of the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9c83-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9c83-108">Prerequisites</span></span>
<span data-ttu-id="b9c83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9c83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9c83-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9c83-111">Permission type</span></span>|<span data-ttu-id="b9c83-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9c83-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9c83-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9c83-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9c83-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9c83-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b9c83-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9c83-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9c83-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9c83-116">Not supported.</span></span>|
|<span data-ttu-id="b9c83-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9c83-117">Application</span></span>|<span data-ttu-id="b9c83-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9c83-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9c83-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9c83-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9c83-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9c83-120">Optional query parameters</span></span>
<span data-ttu-id="b9c83-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9c83-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9c83-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9c83-122">Request headers</span></span>
|<span data-ttu-id="b9c83-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9c83-123">Header</span></span>|<span data-ttu-id="b9c83-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b9c83-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9c83-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9c83-125">Authorization</span></span>|<span data-ttu-id="b9c83-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9c83-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9c83-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9c83-127">Accept</span></span>|<span data-ttu-id="b9c83-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b9c83-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9c83-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9c83-129">Request body</span></span>
<span data-ttu-id="b9c83-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9c83-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9c83-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9c83-131">Response</span></span>
<span data-ttu-id="b9c83-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9c83-132">If successful, this method returns a `200 OK` response code and [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9c83-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9c83-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9c83-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9c83-134">Request</span></span>
<span data-ttu-id="b9c83-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9c83-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

### <a name="response"></a><span data-ttu-id="b9c83-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9c83-136">Response</span></span>
<span data-ttu-id="b9c83-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9c83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





