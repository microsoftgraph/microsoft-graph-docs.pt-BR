---
title: ação setScheduledRetireState
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0cb0a0fed1e720734a86b114b1bccd2bdcec35a9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42755942"
---
# <a name="setscheduledretirestate-action"></a><span data-ttu-id="ebbe9-103">ação setScheduledRetireState</span><span class="sxs-lookup"><span data-stu-id="ebbe9-103">setScheduledRetireState action</span></span>

> <span data-ttu-id="ebbe9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ebbe9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebbe9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebbe9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebbe9-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ebbe9-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebbe9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ebbe9-107">Prerequisites</span></span>
<span data-ttu-id="ebbe9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebbe9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebbe9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebbe9-110">Permission type</span></span>|<span data-ttu-id="ebbe9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ebbe9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebbe9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebbe9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebbe9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebbe9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ebbe9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebbe9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebbe9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebbe9-115">Not supported.</span></span>|
|<span data-ttu-id="ebbe9-116">Application</span><span class="sxs-lookup"><span data-stu-id="ebbe9-116">Application</span></span>|<span data-ttu-id="ebbe9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebbe9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebbe9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebbe9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/setScheduledRetireState
```

## <a name="request-headers"></a><span data-ttu-id="ebbe9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebbe9-119">Request headers</span></span>
|<span data-ttu-id="ebbe9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebbe9-120">Header</span></span>|<span data-ttu-id="ebbe9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ebbe9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebbe9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebbe9-122">Authorization</span></span>|<span data-ttu-id="ebbe9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebbe9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebbe9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ebbe9-124">Accept</span></span>|<span data-ttu-id="ebbe9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ebbe9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebbe9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebbe9-126">Request body</span></span>
<span data-ttu-id="ebbe9-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ebbe9-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ebbe9-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ebbe9-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ebbe9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebbe9-129">Property</span></span>|<span data-ttu-id="ebbe9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebbe9-130">Type</span></span>|<span data-ttu-id="ebbe9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebbe9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebbe9-132">state</span><span class="sxs-lookup"><span data-stu-id="ebbe9-132">state</span></span>|[<span data-ttu-id="ebbe9-133">scheduledRetireState</span><span class="sxs-lookup"><span data-stu-id="ebbe9-133">scheduledRetireState</span></span>](../resources/intune-deviceconfig-scheduledretirestate.md)|<span data-ttu-id="ebbe9-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ebbe9-134">Not yet documented</span></span>|
|<span data-ttu-id="ebbe9-135">managedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="ebbe9-135">managedDeviceIds</span></span>|<span data-ttu-id="ebbe9-136">String collection</span><span class="sxs-lookup"><span data-stu-id="ebbe9-136">String collection</span></span>|<span data-ttu-id="ebbe9-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ebbe9-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ebbe9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebbe9-138">Response</span></span>
<span data-ttu-id="ebbe9-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ebbe9-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ebbe9-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebbe9-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebbe9-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebbe9-141">Request</span></span>
<span data-ttu-id="ebbe9-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebbe9-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/setScheduledRetireState

Content-type: application/json
Content-length: 95

{
  "state": "comfirmRetire",
  "managedDeviceIds": [
    "Managed Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ebbe9-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebbe9-143">Response</span></span>
<span data-ttu-id="ebbe9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebbe9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




