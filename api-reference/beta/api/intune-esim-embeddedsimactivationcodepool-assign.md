---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 49ccf3cd2039b188037e44bdcb8c29c0a4736e2a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212353"
---
# <a name="assign-action"></a><span data-ttu-id="82cc8-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="82cc8-103">assign action</span></span>

<span data-ttu-id="82cc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82cc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82cc8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="82cc8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82cc8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82cc8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82cc8-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82cc8-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82cc8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82cc8-108">Prerequisites</span></span>
<span data-ttu-id="82cc8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82cc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82cc8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82cc8-111">Permission type</span></span>|<span data-ttu-id="82cc8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="82cc8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82cc8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82cc8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82cc8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82cc8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82cc8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82cc8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82cc8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82cc8-116">Not supported.</span></span>|
|<span data-ttu-id="82cc8-117">Application</span><span class="sxs-lookup"><span data-stu-id="82cc8-117">Application</span></span>|<span data-ttu-id="82cc8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82cc8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82cc8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82cc8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="82cc8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82cc8-120">Request headers</span></span>
|<span data-ttu-id="82cc8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82cc8-121">Header</span></span>|<span data-ttu-id="82cc8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="82cc8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82cc8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="82cc8-123">Authorization</span></span>|<span data-ttu-id="82cc8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82cc8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82cc8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="82cc8-125">Accept</span></span>|<span data-ttu-id="82cc8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82cc8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82cc8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82cc8-127">Request body</span></span>
<span data-ttu-id="82cc8-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="82cc8-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="82cc8-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="82cc8-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="82cc8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82cc8-130">Property</span></span>|<span data-ttu-id="82cc8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="82cc8-131">Type</span></span>|<span data-ttu-id="82cc8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="82cc8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82cc8-133">assignments</span><span class="sxs-lookup"><span data-stu-id="82cc8-133">assignments</span></span>|<span data-ttu-id="82cc8-134">coleção [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)</span><span class="sxs-lookup"><span data-stu-id="82cc8-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="82cc8-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82cc8-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="82cc8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="82cc8-136">Response</span></span>
<span data-ttu-id="82cc8-137">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e uma coleção [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82cc8-137">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82cc8-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82cc8-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="82cc8-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82cc8-139">Request</span></span>
<span data-ttu-id="82cc8-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82cc8-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign

Content-type: application/json
Content-length: 456

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="82cc8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="82cc8-141">Response</span></span>
<span data-ttu-id="82cc8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82cc8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```




