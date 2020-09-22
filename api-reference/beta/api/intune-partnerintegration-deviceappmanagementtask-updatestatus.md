---
title: ação updateStatus
description: Definir o status da tarefa e anexar uma anotação.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cdd3de9ba71e9e88307b8e90975851400dbb6a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053885"
---
# <a name="updatestatus-action"></a><span data-ttu-id="a13b2-103">ação updateStatus</span><span class="sxs-lookup"><span data-stu-id="a13b2-103">updateStatus action</span></span>

<span data-ttu-id="a13b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a13b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a13b2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a13b2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a13b2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a13b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a13b2-107">Definir o status da tarefa e anexar uma anotação.</span><span class="sxs-lookup"><span data-stu-id="a13b2-107">Set the task's status and attach a note.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a13b2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a13b2-108">Prerequisites</span></span>
<span data-ttu-id="a13b2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a13b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a13b2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a13b2-111">Permission type</span></span>|<span data-ttu-id="a13b2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a13b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a13b2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a13b2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a13b2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a13b2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a13b2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a13b2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a13b2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a13b2-116">Not supported.</span></span>|
|<span data-ttu-id="a13b2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a13b2-117">Application</span></span>|<span data-ttu-id="a13b2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a13b2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a13b2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a13b2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus
```

## <a name="request-headers"></a><span data-ttu-id="a13b2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a13b2-120">Request headers</span></span>
|<span data-ttu-id="a13b2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a13b2-121">Header</span></span>|<span data-ttu-id="a13b2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a13b2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a13b2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a13b2-123">Authorization</span></span>|<span data-ttu-id="a13b2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a13b2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a13b2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a13b2-125">Accept</span></span>|<span data-ttu-id="a13b2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a13b2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a13b2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a13b2-127">Request body</span></span>
<span data-ttu-id="a13b2-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a13b2-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a13b2-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="a13b2-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a13b2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a13b2-130">Property</span></span>|<span data-ttu-id="a13b2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a13b2-131">Type</span></span>|<span data-ttu-id="a13b2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a13b2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a13b2-133">status</span><span class="sxs-lookup"><span data-stu-id="a13b2-133">status</span></span>|[<span data-ttu-id="a13b2-134">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="a13b2-134">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="a13b2-135">O status</span><span class="sxs-lookup"><span data-stu-id="a13b2-135">The status</span></span>|
|<span data-ttu-id="a13b2-136">Observação</span><span class="sxs-lookup"><span data-stu-id="a13b2-136">note</span></span>|<span data-ttu-id="a13b2-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a13b2-137">String</span></span>|<span data-ttu-id="a13b2-138">A observação</span><span class="sxs-lookup"><span data-stu-id="a13b2-138">The note</span></span>|



## <a name="response"></a><span data-ttu-id="a13b2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a13b2-139">Response</span></span>
<span data-ttu-id="a13b2-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a13b2-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a13b2-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a13b2-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="a13b2-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a13b2-142">Request</span></span>
<span data-ttu-id="a13b2-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a13b2-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus

Content-type: application/json
Content-length: 52

{
  "status": "pending",
  "note": "Note value"
}
```

### <a name="response"></a><span data-ttu-id="a13b2-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a13b2-144">Response</span></span>
<span data-ttu-id="a13b2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a13b2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






