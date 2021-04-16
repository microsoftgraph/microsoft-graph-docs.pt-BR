---
title: Ação hasPayloadLinks
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3e9f2642e41f116b1554ac636c66adce9246765
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867760"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="f40ca-103">Ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="f40ca-103">hasPayloadLinks action</span></span>

<span data-ttu-id="f40ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f40ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f40ca-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f40ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f40ca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f40ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f40ca-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f40ca-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f40ca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f40ca-108">Prerequisites</span></span>
<span data-ttu-id="f40ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f40ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f40ca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f40ca-111">Permission type</span></span>|<span data-ttu-id="f40ca-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f40ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f40ca-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f40ca-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f40ca-114">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="f40ca-114">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f40ca-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f40ca-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f40ca-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f40ca-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f40ca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f40ca-117">Not supported.</span></span>|
|<span data-ttu-id="f40ca-118">Application</span><span class="sxs-lookup"><span data-stu-id="f40ca-118">Application</span></span>||
| <span data-ttu-id="f40ca-119">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="f40ca-119">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f40ca-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f40ca-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f40ca-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f40ca-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="f40ca-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f40ca-122">Request headers</span></span>
|<span data-ttu-id="f40ca-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f40ca-123">Header</span></span>|<span data-ttu-id="f40ca-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f40ca-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f40ca-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f40ca-125">Authorization</span></span>|<span data-ttu-id="f40ca-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f40ca-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f40ca-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f40ca-127">Accept</span></span>|<span data-ttu-id="f40ca-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f40ca-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f40ca-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f40ca-129">Request body</span></span>
<span data-ttu-id="f40ca-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f40ca-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f40ca-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f40ca-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f40ca-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f40ca-132">Property</span></span>|<span data-ttu-id="f40ca-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="f40ca-133">Type</span></span>|<span data-ttu-id="f40ca-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f40ca-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f40ca-135">payloadIds</span><span class="sxs-lookup"><span data-stu-id="f40ca-135">payloadIds</span></span>|<span data-ttu-id="f40ca-136">String collection</span><span class="sxs-lookup"><span data-stu-id="f40ca-136">String collection</span></span>|<span data-ttu-id="f40ca-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f40ca-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f40ca-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f40ca-138">Response</span></span>
<span data-ttu-id="f40ca-139">Se tiver êxito, essa ação retornará um código de resposta e uma coleção `200 OK` [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f40ca-139">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f40ca-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f40ca-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f40ca-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f40ca-141">Request</span></span>
<span data-ttu-id="f40ca-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f40ca-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f40ca-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f40ca-143">Response</span></span>
<span data-ttu-id="f40ca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f40ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







