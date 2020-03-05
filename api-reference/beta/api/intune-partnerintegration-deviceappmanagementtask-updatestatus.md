---
title: ação updateStatus
description: Definir o status da tarefa e anexar uma anotação.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c37d88f016b91e630bb8ae230dede9783fb6e5af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461225"
---
# <a name="updatestatus-action"></a><span data-ttu-id="644df-103">ação updateStatus</span><span class="sxs-lookup"><span data-stu-id="644df-103">updateStatus action</span></span>

<span data-ttu-id="644df-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="644df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="644df-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="644df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="644df-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="644df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="644df-107">Definir o status da tarefa e anexar uma anotação.</span><span class="sxs-lookup"><span data-stu-id="644df-107">Set the task's status and attach a note.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="644df-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="644df-108">Prerequisites</span></span>
<span data-ttu-id="644df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="644df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="644df-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="644df-111">Permission type</span></span>|<span data-ttu-id="644df-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="644df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="644df-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="644df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="644df-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="644df-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="644df-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="644df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="644df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="644df-116">Not supported.</span></span>|
|<span data-ttu-id="644df-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="644df-117">Application</span></span>|<span data-ttu-id="644df-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="644df-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="644df-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="644df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus
```

## <a name="request-headers"></a><span data-ttu-id="644df-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="644df-120">Request headers</span></span>
|<span data-ttu-id="644df-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="644df-121">Header</span></span>|<span data-ttu-id="644df-122">Valor</span><span class="sxs-lookup"><span data-stu-id="644df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="644df-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="644df-123">Authorization</span></span>|<span data-ttu-id="644df-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="644df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="644df-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="644df-125">Accept</span></span>|<span data-ttu-id="644df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="644df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="644df-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="644df-127">Request body</span></span>
<span data-ttu-id="644df-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="644df-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="644df-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="644df-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="644df-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="644df-130">Property</span></span>|<span data-ttu-id="644df-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="644df-131">Type</span></span>|<span data-ttu-id="644df-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="644df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="644df-133">status</span><span class="sxs-lookup"><span data-stu-id="644df-133">status</span></span>|[<span data-ttu-id="644df-134">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="644df-134">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="644df-135">O status</span><span class="sxs-lookup"><span data-stu-id="644df-135">The status</span></span>|
|<span data-ttu-id="644df-136">Observação</span><span class="sxs-lookup"><span data-stu-id="644df-136">note</span></span>|<span data-ttu-id="644df-137">String</span><span class="sxs-lookup"><span data-stu-id="644df-137">String</span></span>|<span data-ttu-id="644df-138">A observação</span><span class="sxs-lookup"><span data-stu-id="644df-138">The note</span></span>|



## <a name="response"></a><span data-ttu-id="644df-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="644df-139">Response</span></span>
<span data-ttu-id="644df-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="644df-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="644df-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="644df-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="644df-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="644df-142">Request</span></span>
<span data-ttu-id="644df-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="644df-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus

Content-type: application/json
Content-length: 52

{
  "status": "pending",
  "note": "Note value"
}
```

### <a name="response"></a><span data-ttu-id="644df-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="644df-144">Response</span></span>
<span data-ttu-id="644df-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="644df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





