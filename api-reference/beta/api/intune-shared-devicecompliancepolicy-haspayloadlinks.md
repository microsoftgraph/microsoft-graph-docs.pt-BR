---
title: ação hasPayloadLinks
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aca08815a975a105938d146706070b0447444b75
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458767"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="48dd0-103">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="48dd0-103">hasPayloadLinks action</span></span>

<span data-ttu-id="48dd0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="48dd0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48dd0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48dd0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48dd0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48dd0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48dd0-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48dd0-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48dd0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="48dd0-108">Prerequisites</span></span>
<span data-ttu-id="48dd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48dd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48dd0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48dd0-111">Permission type</span></span>|<span data-ttu-id="48dd0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="48dd0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48dd0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48dd0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="48dd0-114">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="48dd0-114">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="48dd0-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="48dd0-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="48dd0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48dd0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48dd0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48dd0-117">Not supported.</span></span>|
|<span data-ttu-id="48dd0-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48dd0-118">Application</span></span>||
| <span data-ttu-id="48dd0-119">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="48dd0-119">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="48dd0-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="48dd0-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48dd0-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48dd0-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="48dd0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48dd0-122">Request headers</span></span>
|<span data-ttu-id="48dd0-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48dd0-123">Header</span></span>|<span data-ttu-id="48dd0-124">Valor</span><span class="sxs-lookup"><span data-stu-id="48dd0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48dd0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="48dd0-125">Authorization</span></span>|<span data-ttu-id="48dd0-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48dd0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48dd0-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="48dd0-127">Accept</span></span>|<span data-ttu-id="48dd0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="48dd0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48dd0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48dd0-129">Request body</span></span>
<span data-ttu-id="48dd0-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="48dd0-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="48dd0-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="48dd0-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="48dd0-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48dd0-132">Property</span></span>|<span data-ttu-id="48dd0-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="48dd0-133">Type</span></span>|<span data-ttu-id="48dd0-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="48dd0-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48dd0-135">payloadIds</span><span class="sxs-lookup"><span data-stu-id="48dd0-135">payloadIds</span></span>|<span data-ttu-id="48dd0-136">String collection</span><span class="sxs-lookup"><span data-stu-id="48dd0-136">String collection</span></span>|<span data-ttu-id="48dd0-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48dd0-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="48dd0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="48dd0-138">Response</span></span>
<span data-ttu-id="48dd0-139">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48dd0-139">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48dd0-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48dd0-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="48dd0-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48dd0-141">Request</span></span>
<span data-ttu-id="48dd0-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48dd0-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/hasPayloadLinks

Content-type: application/json
Content-length: 53

{
  "payloadIds": [
    "Payload Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="48dd0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="48dd0-143">Response</span></span>
<span data-ttu-id="48dd0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48dd0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








