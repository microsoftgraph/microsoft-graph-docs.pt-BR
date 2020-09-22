---
title: ação hasPayloadLinks
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5a99c1c0c38228a6a9081735076c61deee6b6cc6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024693"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="3aeb3-103">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="3aeb3-103">hasPayloadLinks action</span></span>

<span data-ttu-id="3aeb3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aeb3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3aeb3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3aeb3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3aeb3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3aeb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3aeb3-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3aeb3-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3aeb3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3aeb3-108">Prerequisites</span></span>
<span data-ttu-id="3aeb3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aeb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aeb3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3aeb3-111">Permission type</span></span>|<span data-ttu-id="3aeb3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3aeb3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3aeb3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3aeb3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3aeb3-114">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="3aeb3-114">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="3aeb3-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3aeb3-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3aeb3-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3aeb3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3aeb3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3aeb3-117">Not supported.</span></span>|
|<span data-ttu-id="3aeb3-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3aeb3-118">Application</span></span>||
| <span data-ttu-id="3aeb3-119">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="3aeb3-119">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="3aeb3-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3aeb3-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3aeb3-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3aeb3-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/androidManagedAppProtections/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="3aeb3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3aeb3-122">Request headers</span></span>
|<span data-ttu-id="3aeb3-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3aeb3-123">Header</span></span>|<span data-ttu-id="3aeb3-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3aeb3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3aeb3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3aeb3-125">Authorization</span></span>|<span data-ttu-id="3aeb3-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3aeb3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3aeb3-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3aeb3-127">Accept</span></span>|<span data-ttu-id="3aeb3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3aeb3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3aeb3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3aeb3-129">Request body</span></span>
<span data-ttu-id="3aeb3-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3aeb3-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3aeb3-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3aeb3-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3aeb3-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3aeb3-132">Property</span></span>|<span data-ttu-id="3aeb3-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="3aeb3-133">Type</span></span>|<span data-ttu-id="3aeb3-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aeb3-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3aeb3-135">payloadIds</span><span class="sxs-lookup"><span data-stu-id="3aeb3-135">payloadIds</span></span>|<span data-ttu-id="3aeb3-136">String collection</span><span class="sxs-lookup"><span data-stu-id="3aeb3-136">String collection</span></span>|<span data-ttu-id="3aeb3-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3aeb3-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3aeb3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aeb3-138">Response</span></span>
<span data-ttu-id="3aeb3-139">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e uma coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3aeb3-139">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3aeb3-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3aeb3-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="3aeb3-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3aeb3-141">Request</span></span>
<span data-ttu-id="3aeb3-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3aeb3-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/hasPayloadLinks

Content-type: application/json
Content-length: 53

{
  "payloadIds": [
    "Payload Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="3aeb3-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aeb3-143">Response</span></span>
<span data-ttu-id="3aeb3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3aeb3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









