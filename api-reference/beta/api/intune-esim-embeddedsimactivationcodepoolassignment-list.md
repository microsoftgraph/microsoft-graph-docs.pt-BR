---
title: Listar embeddedSIMActivationCodePoolAssignments
description: Listar Propriedades e relações dos objetos embeddedSIMActivationCodePoolAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 930513219b54e5e0a1de10bcfd85ab16ce6c193b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173518"
---
# <a name="list-embeddedsimactivationcodepoolassignments"></a><span data-ttu-id="95f91-103">Listar embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="95f91-103">List embeddedSIMActivationCodePoolAssignments</span></span>

> <span data-ttu-id="95f91-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="95f91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95f91-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95f91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95f91-106">Listar Propriedades e relações dos objetos [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="95f91-106">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95f91-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="95f91-107">Prerequisites</span></span>
<span data-ttu-id="95f91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="95f91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="95f91-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95f91-110">Permission type</span></span>|<span data-ttu-id="95f91-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="95f91-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95f91-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95f91-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95f91-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="95f91-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="95f91-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95f91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95f91-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95f91-115">Not supported.</span></span>|
|<span data-ttu-id="95f91-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95f91-116">Application</span></span>|<span data-ttu-id="95f91-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95f91-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95f91-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95f91-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="95f91-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95f91-119">Request headers</span></span>
|<span data-ttu-id="95f91-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95f91-120">Header</span></span>|<span data-ttu-id="95f91-121">Valor</span><span class="sxs-lookup"><span data-stu-id="95f91-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95f91-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="95f91-122">Authorization</span></span>|<span data-ttu-id="95f91-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95f91-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95f91-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="95f91-124">Accept</span></span>|<span data-ttu-id="95f91-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95f91-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95f91-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95f91-126">Request body</span></span>
<span data-ttu-id="95f91-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95f91-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95f91-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="95f91-128">Response</span></span>
<span data-ttu-id="95f91-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95f91-129">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95f91-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95f91-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="95f91-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95f91-131">Request</span></span>
<span data-ttu-id="95f91-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95f91-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

### <a name="response"></a><span data-ttu-id="95f91-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="95f91-133">Response</span></span>
<span data-ttu-id="95f91-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95f91-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




