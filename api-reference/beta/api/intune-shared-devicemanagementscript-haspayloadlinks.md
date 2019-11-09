---
title: ação hasPayloadLinks
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 347824d165e286d3649a9fbb1887aee5b3ba2d9d
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085959"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="b7242-103">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="b7242-103">hasPayloadLinks action</span></span>

> <span data-ttu-id="b7242-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b7242-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7242-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7242-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7242-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b7242-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7242-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7242-107">Prerequisites</span></span>
<span data-ttu-id="b7242-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7242-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7242-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7242-110">Permission type</span></span>|<span data-ttu-id="b7242-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b7242-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7242-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7242-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b7242-113">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="b7242-113">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b7242-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7242-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b7242-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7242-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7242-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7242-116">Not supported.</span></span>|
|<span data-ttu-id="b7242-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7242-117">Application</span></span>||
| <span data-ttu-id="b7242-118">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="b7242-118">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b7242-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7242-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7242-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7242-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="b7242-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7242-121">Request headers</span></span>
|<span data-ttu-id="b7242-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7242-122">Header</span></span>|<span data-ttu-id="b7242-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b7242-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7242-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7242-124">Authorization</span></span>|<span data-ttu-id="b7242-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7242-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7242-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7242-126">Accept</span></span>|<span data-ttu-id="b7242-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b7242-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7242-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7242-128">Request body</span></span>
<span data-ttu-id="b7242-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b7242-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b7242-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b7242-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b7242-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7242-131">Property</span></span>|<span data-ttu-id="b7242-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7242-132">Type</span></span>|<span data-ttu-id="b7242-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7242-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7242-134">payloadIds</span><span class="sxs-lookup"><span data-stu-id="b7242-134">payloadIds</span></span>|<span data-ttu-id="b7242-135">String collection</span><span class="sxs-lookup"><span data-stu-id="b7242-135">String collection</span></span>|<span data-ttu-id="b7242-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b7242-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b7242-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7242-137">Response</span></span>
<span data-ttu-id="b7242-138">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7242-138">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7242-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7242-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7242-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7242-140">Request</span></span>
<span data-ttu-id="b7242-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7242-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/hasPayloadLinks

Content-type: application/json
Content-length: 53

{
  "payloadIds": [
    "Payload Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b7242-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7242-142">Response</span></span>
<span data-ttu-id="b7242-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7242-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









