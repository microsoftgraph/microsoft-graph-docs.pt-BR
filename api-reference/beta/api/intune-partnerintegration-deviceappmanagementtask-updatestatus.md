---
title: Ação updateStatus
description: De definir o status da tarefa e anexar uma nota.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a03d26b3002e39ae27c0920bc95c5ce5f569584d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134844"
---
# <a name="updatestatus-action"></a><span data-ttu-id="b693d-103">Ação updateStatus</span><span class="sxs-lookup"><span data-stu-id="b693d-103">updateStatus action</span></span>

<span data-ttu-id="b693d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b693d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b693d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b693d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b693d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b693d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b693d-107">De definir o status da tarefa e anexar uma nota.</span><span class="sxs-lookup"><span data-stu-id="b693d-107">Set the task's status and attach a note.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b693d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b693d-108">Prerequisites</span></span>
<span data-ttu-id="b693d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b693d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b693d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b693d-111">Permission type</span></span>|<span data-ttu-id="b693d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b693d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b693d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b693d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b693d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b693d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b693d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b693d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b693d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b693d-116">Not supported.</span></span>|
|<span data-ttu-id="b693d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b693d-117">Application</span></span>|<span data-ttu-id="b693d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b693d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b693d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b693d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus
```

## <a name="request-headers"></a><span data-ttu-id="b693d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b693d-120">Request headers</span></span>
|<span data-ttu-id="b693d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b693d-121">Header</span></span>|<span data-ttu-id="b693d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b693d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b693d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b693d-123">Authorization</span></span>|<span data-ttu-id="b693d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b693d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b693d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b693d-125">Accept</span></span>|<span data-ttu-id="b693d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b693d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b693d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b693d-127">Request body</span></span>
<span data-ttu-id="b693d-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b693d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b693d-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b693d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b693d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b693d-130">Property</span></span>|<span data-ttu-id="b693d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b693d-131">Type</span></span>|<span data-ttu-id="b693d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b693d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b693d-133">status</span><span class="sxs-lookup"><span data-stu-id="b693d-133">status</span></span>|[<span data-ttu-id="b693d-134">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="b693d-134">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="b693d-135">O status</span><span class="sxs-lookup"><span data-stu-id="b693d-135">The status</span></span>|
|<span data-ttu-id="b693d-136">observação</span><span class="sxs-lookup"><span data-stu-id="b693d-136">note</span></span>|<span data-ttu-id="b693d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b693d-137">String</span></span>|<span data-ttu-id="b693d-138">A observação</span><span class="sxs-lookup"><span data-stu-id="b693d-138">The note</span></span>|



## <a name="response"></a><span data-ttu-id="b693d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b693d-139">Response</span></span>
<span data-ttu-id="b693d-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b693d-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b693d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b693d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b693d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b693d-142">Request</span></span>
<span data-ttu-id="b693d-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b693d-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus

Content-type: application/json
Content-length: 52

{
  "status": "pending",
  "note": "Note value"
}
```

### <a name="response"></a><span data-ttu-id="b693d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b693d-144">Response</span></span>
<span data-ttu-id="b693d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b693d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




