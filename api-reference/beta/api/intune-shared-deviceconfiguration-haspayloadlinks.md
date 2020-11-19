---
title: ação hasPayloadLinks
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6f3d7954e04a2eeaa1d171ffe9a20e0bc1702227
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49257363"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="6d33b-103">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="6d33b-103">hasPayloadLinks action</span></span>

<span data-ttu-id="6d33b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d33b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d33b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d33b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d33b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d33b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d33b-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6d33b-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d33b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d33b-108">Prerequisites</span></span>
<span data-ttu-id="6d33b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d33b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d33b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d33b-111">Permission type</span></span>|<span data-ttu-id="6d33b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d33b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d33b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d33b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6d33b-114">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="6d33b-114">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6d33b-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d33b-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6d33b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d33b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d33b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d33b-117">Not supported.</span></span>|
|<span data-ttu-id="6d33b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d33b-118">Application</span></span>||
| <span data-ttu-id="6d33b-119">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="6d33b-119">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6d33b-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d33b-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d33b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d33b-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="6d33b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d33b-122">Request headers</span></span>
|<span data-ttu-id="6d33b-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d33b-123">Header</span></span>|<span data-ttu-id="6d33b-124">Valor</span><span class="sxs-lookup"><span data-stu-id="6d33b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d33b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d33b-125">Authorization</span></span>|<span data-ttu-id="6d33b-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d33b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d33b-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d33b-127">Accept</span></span>|<span data-ttu-id="6d33b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6d33b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d33b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d33b-129">Request body</span></span>
<span data-ttu-id="6d33b-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6d33b-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6d33b-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="6d33b-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6d33b-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d33b-132">Property</span></span>|<span data-ttu-id="6d33b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d33b-133">Type</span></span>|<span data-ttu-id="6d33b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d33b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d33b-135">payloadIds</span><span class="sxs-lookup"><span data-stu-id="6d33b-135">payloadIds</span></span>|<span data-ttu-id="6d33b-136">String collection</span><span class="sxs-lookup"><span data-stu-id="6d33b-136">String collection</span></span>|<span data-ttu-id="6d33b-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6d33b-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6d33b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d33b-138">Response</span></span>
<span data-ttu-id="6d33b-139">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e uma coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d33b-139">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d33b-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d33b-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d33b-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d33b-141">Request</span></span>
<span data-ttu-id="6d33b-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d33b-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/hasPayloadLinks

Content-type: application/json
Content-length: 53

{
  "payloadIds": [
    "Payload Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="6d33b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d33b-143">Response</span></span>
<span data-ttu-id="6d33b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d33b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.hasPayloadLinkResultItem",
      "payloadId": "Payload Id value",
      "hasLink": true,
      "error": "Error value",
      "sources": [
        "policySets"
      ]
    }
  ]
}
```







