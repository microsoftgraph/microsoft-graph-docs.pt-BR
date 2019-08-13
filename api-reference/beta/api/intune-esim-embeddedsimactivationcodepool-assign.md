---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a9a698c8731028b4ec429f8546e1fda7b5caeefb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355917"
---
# <a name="assign-action"></a><span data-ttu-id="f0f74-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="f0f74-103">assign action</span></span>

> <span data-ttu-id="f0f74-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0f74-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0f74-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0f74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0f74-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f0f74-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0f74-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0f74-107">Prerequisites</span></span>
<span data-ttu-id="f0f74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0f74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0f74-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0f74-110">Permission type</span></span>|<span data-ttu-id="f0f74-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f0f74-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0f74-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0f74-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f0f74-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0f74-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0f74-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0f74-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0f74-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0f74-115">Not supported.</span></span>|
|<span data-ttu-id="f0f74-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0f74-116">Application</span></span>|<span data-ttu-id="f0f74-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0f74-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0f74-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0f74-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="f0f74-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0f74-119">Request headers</span></span>
|<span data-ttu-id="f0f74-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0f74-120">Header</span></span>|<span data-ttu-id="f0f74-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f0f74-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0f74-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0f74-122">Authorization</span></span>|<span data-ttu-id="f0f74-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0f74-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0f74-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f0f74-124">Accept</span></span>|<span data-ttu-id="f0f74-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f0f74-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0f74-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0f74-126">Request body</span></span>
<span data-ttu-id="f0f74-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f0f74-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f0f74-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f0f74-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f0f74-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0f74-129">Property</span></span>|<span data-ttu-id="f0f74-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0f74-130">Type</span></span>|<span data-ttu-id="f0f74-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0f74-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0f74-132">assignments</span><span class="sxs-lookup"><span data-stu-id="f0f74-132">assignments</span></span>|<span data-ttu-id="f0f74-133">coleção [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f0f74-133">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="f0f74-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f0f74-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f0f74-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0f74-135">Response</span></span>
<span data-ttu-id="f0f74-136">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0f74-136">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0f74-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0f74-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0f74-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0f74-138">Request</span></span>
<span data-ttu-id="f0f74-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0f74-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign

Content-type: application/json
Content-length: 287

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f0f74-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0f74-140">Response</span></span>
<span data-ttu-id="f0f74-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0f74-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 281

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```






