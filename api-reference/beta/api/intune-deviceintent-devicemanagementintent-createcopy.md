---
title: ação CreateCopy
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 06d4d51a2a11b4fb4f029ff11ac40642364e1d7f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990036"
---
# <a name="createcopy-action"></a><span data-ttu-id="d3f58-103">ação CreateCopy</span><span class="sxs-lookup"><span data-stu-id="d3f58-103">createCopy action</span></span>

<span data-ttu-id="d3f58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3f58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3f58-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3f58-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3f58-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3f58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3f58-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d3f58-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3f58-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3f58-108">Prerequisites</span></span>
<span data-ttu-id="d3f58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3f58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3f58-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3f58-111">Permission type</span></span>|<span data-ttu-id="d3f58-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3f58-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3f58-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3f58-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3f58-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3f58-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3f58-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3f58-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3f58-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3f58-116">Not supported.</span></span>|
|<span data-ttu-id="d3f58-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3f58-117">Application</span></span>|<span data-ttu-id="d3f58-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3f58-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3f58-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3f58-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/createCopy
```

## <a name="request-headers"></a><span data-ttu-id="d3f58-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3f58-120">Request headers</span></span>
|<span data-ttu-id="d3f58-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3f58-121">Header</span></span>|<span data-ttu-id="d3f58-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d3f58-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3f58-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3f58-123">Authorization</span></span>|<span data-ttu-id="d3f58-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3f58-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3f58-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3f58-125">Accept</span></span>|<span data-ttu-id="d3f58-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3f58-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3f58-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3f58-127">Request body</span></span>
<span data-ttu-id="d3f58-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d3f58-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d3f58-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d3f58-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d3f58-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3f58-130">Property</span></span>|<span data-ttu-id="d3f58-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3f58-131">Type</span></span>|<span data-ttu-id="d3f58-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3f58-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3f58-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d3f58-133">displayName</span></span>|<span data-ttu-id="d3f58-134">String</span><span class="sxs-lookup"><span data-stu-id="d3f58-134">String</span></span>|<span data-ttu-id="d3f58-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d3f58-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d3f58-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3f58-136">Response</span></span>
<span data-ttu-id="d3f58-137">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e um [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3f58-137">If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3f58-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3f58-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3f58-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3f58-139">Request</span></span>
<span data-ttu-id="d3f58-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3f58-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/createCopy

Content-type: application/json
Content-length: 43

{
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="d3f58-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3f58-141">Response</span></span>
<span data-ttu-id="d3f58-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3f58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 418

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntent",
    "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
    "displayName": "Display Name value",
    "description": "Description value",
    "isAssigned": true,
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "templateId": "Template Id value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```






