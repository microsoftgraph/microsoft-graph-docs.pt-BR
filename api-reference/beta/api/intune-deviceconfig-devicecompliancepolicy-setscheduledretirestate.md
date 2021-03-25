---
title: ação setScheduledRetireState
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8e84d14c0161acc19966dba828b55828550e91b7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155537"
---
# <a name="setscheduledretirestate-action"></a><span data-ttu-id="127f4-103">ação setScheduledRetireState</span><span class="sxs-lookup"><span data-stu-id="127f4-103">setScheduledRetireState action</span></span>

<span data-ttu-id="127f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="127f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="127f4-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="127f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="127f4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="127f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="127f4-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="127f4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="127f4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="127f4-108">Prerequisites</span></span>
<span data-ttu-id="127f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="127f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="127f4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="127f4-111">Permission type</span></span>|<span data-ttu-id="127f4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="127f4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="127f4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="127f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="127f4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="127f4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="127f4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="127f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="127f4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="127f4-116">Not supported.</span></span>|
|<span data-ttu-id="127f4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="127f4-117">Application</span></span>|<span data-ttu-id="127f4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="127f4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="127f4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="127f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/setScheduledRetireState
```

## <a name="request-headers"></a><span data-ttu-id="127f4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="127f4-120">Request headers</span></span>
|<span data-ttu-id="127f4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="127f4-121">Header</span></span>|<span data-ttu-id="127f4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="127f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="127f4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="127f4-123">Authorization</span></span>|<span data-ttu-id="127f4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="127f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="127f4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="127f4-125">Accept</span></span>|<span data-ttu-id="127f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="127f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="127f4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="127f4-127">Request body</span></span>
<span data-ttu-id="127f4-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="127f4-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="127f4-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="127f4-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="127f4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="127f4-130">Property</span></span>|<span data-ttu-id="127f4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="127f4-131">Type</span></span>|<span data-ttu-id="127f4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="127f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="127f4-133">state</span><span class="sxs-lookup"><span data-stu-id="127f4-133">state</span></span>|[<span data-ttu-id="127f4-134">scheduledRetireState</span><span class="sxs-lookup"><span data-stu-id="127f4-134">scheduledRetireState</span></span>](../resources/intune-deviceconfig-scheduledretirestate.md)|<span data-ttu-id="127f4-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="127f4-135">Not yet documented</span></span>|
|<span data-ttu-id="127f4-136">managedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="127f4-136">managedDeviceIds</span></span>|<span data-ttu-id="127f4-137">String collection</span><span class="sxs-lookup"><span data-stu-id="127f4-137">String collection</span></span>|<span data-ttu-id="127f4-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="127f4-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="127f4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="127f4-139">Response</span></span>
<span data-ttu-id="127f4-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="127f4-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="127f4-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="127f4-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="127f4-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="127f4-142">Request</span></span>
<span data-ttu-id="127f4-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="127f4-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="127f4-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="127f4-144">Response</span></span>
<span data-ttu-id="127f4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="127f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




