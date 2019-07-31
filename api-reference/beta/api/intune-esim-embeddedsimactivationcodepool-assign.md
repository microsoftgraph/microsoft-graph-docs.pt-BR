---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b4a22bac31443f1673f1dab4f01be3de0d2ce9df
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995353"
---
# <a name="assign-action"></a><span data-ttu-id="39583-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="39583-103">assign action</span></span>

> <span data-ttu-id="39583-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="39583-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39583-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39583-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39583-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="39583-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39583-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="39583-107">Prerequisites</span></span>
<span data-ttu-id="39583-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39583-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39583-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39583-110">Permission type</span></span>|<span data-ttu-id="39583-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="39583-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39583-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39583-112">Delegated (work or school account)</span></span>|<span data-ttu-id="39583-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39583-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39583-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39583-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39583-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39583-115">Not supported.</span></span>|
|<span data-ttu-id="39583-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39583-116">Application</span></span>|<span data-ttu-id="39583-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39583-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39583-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39583-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="39583-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39583-119">Request headers</span></span>
|<span data-ttu-id="39583-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39583-120">Header</span></span>|<span data-ttu-id="39583-121">Valor</span><span class="sxs-lookup"><span data-stu-id="39583-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39583-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="39583-122">Authorization</span></span>|<span data-ttu-id="39583-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39583-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39583-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="39583-124">Accept</span></span>|<span data-ttu-id="39583-125">application/json</span><span class="sxs-lookup"><span data-stu-id="39583-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39583-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39583-126">Request body</span></span>
<span data-ttu-id="39583-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="39583-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="39583-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="39583-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="39583-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39583-129">Property</span></span>|<span data-ttu-id="39583-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="39583-130">Type</span></span>|<span data-ttu-id="39583-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="39583-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39583-132">assignments</span><span class="sxs-lookup"><span data-stu-id="39583-132">assignments</span></span>|<span data-ttu-id="39583-133">coleção [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)</span><span class="sxs-lookup"><span data-stu-id="39583-133">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="39583-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="39583-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="39583-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="39583-135">Response</span></span>
<span data-ttu-id="39583-136">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39583-136">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39583-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39583-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="39583-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39583-138">Request</span></span>
<span data-ttu-id="39583-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39583-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="39583-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="39583-140">Response</span></span>
<span data-ttu-id="39583-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39583-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





