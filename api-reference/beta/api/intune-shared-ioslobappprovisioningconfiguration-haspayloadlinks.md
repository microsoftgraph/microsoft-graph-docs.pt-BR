---
title: ação hasPayloadLinks
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d890135cf6305535ea23ebc9ee58db1cfd6b95d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939834"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="3c792-103">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="3c792-103">hasPayloadLinks action</span></span>

> <span data-ttu-id="3c792-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c792-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c792-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c792-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c792-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3c792-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c792-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c792-107">Prerequisites</span></span>
<span data-ttu-id="3c792-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c792-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c792-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c792-110">Permission type</span></span>|<span data-ttu-id="3c792-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c792-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c792-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c792-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3c792-113">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="3c792-113">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="3c792-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c792-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3c792-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c792-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c792-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c792-116">Not supported.</span></span>|
|<span data-ttu-id="3c792-117">Application</span><span class="sxs-lookup"><span data-stu-id="3c792-117">Application</span></span>||
| <span data-ttu-id="3c792-118">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="3c792-118">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="3c792-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c792-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c792-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c792-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="3c792-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c792-121">Request headers</span></span>
|<span data-ttu-id="3c792-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c792-122">Header</span></span>|<span data-ttu-id="3c792-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3c792-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c792-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c792-124">Authorization</span></span>|<span data-ttu-id="3c792-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c792-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c792-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c792-126">Accept</span></span>|<span data-ttu-id="3c792-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3c792-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c792-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c792-128">Request body</span></span>
<span data-ttu-id="3c792-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3c792-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3c792-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3c792-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3c792-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c792-131">Property</span></span>|<span data-ttu-id="3c792-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c792-132">Type</span></span>|<span data-ttu-id="3c792-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c792-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c792-134">payloadIds</span><span class="sxs-lookup"><span data-stu-id="3c792-134">payloadIds</span></span>|<span data-ttu-id="3c792-135">String collection</span><span class="sxs-lookup"><span data-stu-id="3c792-135">String collection</span></span>|<span data-ttu-id="3c792-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3c792-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3c792-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c792-137">Response</span></span>
<span data-ttu-id="3c792-138">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c792-138">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c792-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c792-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c792-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c792-140">Request</span></span>
<span data-ttu-id="3c792-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c792-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/hasPayloadLinks

Content-type: application/json
Content-length: 53

{
  "payloadIds": [
    "Payload Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="3c792-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c792-142">Response</span></span>
<span data-ttu-id="3c792-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c792-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








