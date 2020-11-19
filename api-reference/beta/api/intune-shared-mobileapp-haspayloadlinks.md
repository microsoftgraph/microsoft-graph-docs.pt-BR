---
title: ação hasPayloadLinks
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e3a515cb30670d5acfd86df6e91f061cd5afabb4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217526"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="a5d8e-103">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="a5d8e-103">hasPayloadLinks action</span></span>

<span data-ttu-id="a5d8e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5d8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5d8e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a5d8e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5d8e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5d8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5d8e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a5d8e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5d8e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a5d8e-108">Prerequisites</span></span>
<span data-ttu-id="a5d8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5d8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5d8e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5d8e-111">Permission type</span></span>|<span data-ttu-id="a5d8e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a5d8e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5d8e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5d8e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a5d8e-114">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="a5d8e-114">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a5d8e-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5d8e-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a5d8e-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5d8e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5d8e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5d8e-117">Not supported.</span></span>|
|<span data-ttu-id="a5d8e-118">Application</span><span class="sxs-lookup"><span data-stu-id="a5d8e-118">Application</span></span>||
| <span data-ttu-id="a5d8e-119">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="a5d8e-119">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a5d8e-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5d8e-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5d8e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5d8e-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="a5d8e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5d8e-122">Request headers</span></span>
|<span data-ttu-id="a5d8e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5d8e-123">Header</span></span>|<span data-ttu-id="a5d8e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a5d8e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5d8e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5d8e-125">Authorization</span></span>|<span data-ttu-id="a5d8e-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5d8e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5d8e-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a5d8e-127">Accept</span></span>|<span data-ttu-id="a5d8e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a5d8e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5d8e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5d8e-129">Request body</span></span>
<span data-ttu-id="a5d8e-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a5d8e-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a5d8e-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="a5d8e-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a5d8e-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5d8e-132">Property</span></span>|<span data-ttu-id="a5d8e-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5d8e-133">Type</span></span>|<span data-ttu-id="a5d8e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5d8e-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5d8e-135">payloadIds</span><span class="sxs-lookup"><span data-stu-id="a5d8e-135">payloadIds</span></span>|<span data-ttu-id="a5d8e-136">String collection</span><span class="sxs-lookup"><span data-stu-id="a5d8e-136">String collection</span></span>|<span data-ttu-id="a5d8e-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a5d8e-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a5d8e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5d8e-138">Response</span></span>
<span data-ttu-id="a5d8e-139">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e uma coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5d8e-139">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5d8e-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5d8e-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5d8e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5d8e-141">Request</span></span>
<span data-ttu-id="a5d8e-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5d8e-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a5d8e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5d8e-143">Response</span></span>
<span data-ttu-id="a5d8e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5d8e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







