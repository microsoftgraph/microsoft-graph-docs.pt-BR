---
title: ação hasPayloadLinks
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ab27a97418633f102f363bb4b77be109d214b36
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939778"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="eed3e-103">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="eed3e-103">hasPayloadLinks action</span></span>

> <span data-ttu-id="eed3e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eed3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eed3e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eed3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eed3e-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="eed3e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eed3e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eed3e-107">Prerequisites</span></span>
<span data-ttu-id="eed3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eed3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eed3e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eed3e-110">Permission type</span></span>|<span data-ttu-id="eed3e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eed3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eed3e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eed3e-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="eed3e-113">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="eed3e-113">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="eed3e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eed3e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="eed3e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eed3e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eed3e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eed3e-116">Not supported.</span></span>|
|<span data-ttu-id="eed3e-117">Application</span><span class="sxs-lookup"><span data-stu-id="eed3e-117">Application</span></span>||
| <span data-ttu-id="eed3e-118">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="eed3e-118">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="eed3e-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eed3e-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eed3e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eed3e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="eed3e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eed3e-121">Request headers</span></span>
|<span data-ttu-id="eed3e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eed3e-122">Header</span></span>|<span data-ttu-id="eed3e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="eed3e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eed3e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="eed3e-124">Authorization</span></span>|<span data-ttu-id="eed3e-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eed3e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eed3e-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eed3e-126">Accept</span></span>|<span data-ttu-id="eed3e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="eed3e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eed3e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eed3e-128">Request body</span></span>
<span data-ttu-id="eed3e-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="eed3e-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="eed3e-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="eed3e-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="eed3e-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eed3e-131">Property</span></span>|<span data-ttu-id="eed3e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="eed3e-132">Type</span></span>|<span data-ttu-id="eed3e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="eed3e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eed3e-134">payloadIds</span><span class="sxs-lookup"><span data-stu-id="eed3e-134">payloadIds</span></span>|<span data-ttu-id="eed3e-135">String collection</span><span class="sxs-lookup"><span data-stu-id="eed3e-135">String collection</span></span>|<span data-ttu-id="eed3e-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="eed3e-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="eed3e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="eed3e-137">Response</span></span>
<span data-ttu-id="eed3e-138">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eed3e-138">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eed3e-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eed3e-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="eed3e-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eed3e-140">Request</span></span>
<span data-ttu-id="eed3e-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eed3e-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/hasPayloadLinks

Content-type: application/json
Content-length: 53

{
  "payloadIds": [
    "Payload Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="eed3e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="eed3e-142">Response</span></span>
<span data-ttu-id="eed3e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eed3e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








