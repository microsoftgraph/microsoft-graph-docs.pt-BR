---
title: ação updateStatus
description: Definir o status da tarefa e anexar uma anotação.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b41581f24612cb59cf36deda55acadb3bf519135
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002291"
---
# <a name="updatestatus-action"></a><span data-ttu-id="372b2-103">ação updateStatus</span><span class="sxs-lookup"><span data-stu-id="372b2-103">updateStatus action</span></span>

> <span data-ttu-id="372b2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="372b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="372b2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="372b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="372b2-106">Definir o status da tarefa e anexar uma anotação.</span><span class="sxs-lookup"><span data-stu-id="372b2-106">Set the task's status and attach a note.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="372b2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="372b2-107">Prerequisites</span></span>
<span data-ttu-id="372b2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="372b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="372b2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="372b2-110">Permission type</span></span>|<span data-ttu-id="372b2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="372b2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="372b2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="372b2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="372b2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="372b2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="372b2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="372b2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="372b2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="372b2-115">Not supported.</span></span>|
|<span data-ttu-id="372b2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="372b2-116">Application</span></span>|<span data-ttu-id="372b2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="372b2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="372b2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="372b2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus
```

## <a name="request-headers"></a><span data-ttu-id="372b2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="372b2-119">Request headers</span></span>
|<span data-ttu-id="372b2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="372b2-120">Header</span></span>|<span data-ttu-id="372b2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="372b2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="372b2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="372b2-122">Authorization</span></span>|<span data-ttu-id="372b2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="372b2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="372b2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="372b2-124">Accept</span></span>|<span data-ttu-id="372b2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="372b2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="372b2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="372b2-126">Request body</span></span>
<span data-ttu-id="372b2-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="372b2-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="372b2-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="372b2-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="372b2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="372b2-129">Property</span></span>|<span data-ttu-id="372b2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="372b2-130">Type</span></span>|<span data-ttu-id="372b2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="372b2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="372b2-132">status</span><span class="sxs-lookup"><span data-stu-id="372b2-132">status</span></span>|[<span data-ttu-id="372b2-133">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="372b2-133">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="372b2-134">O status</span><span class="sxs-lookup"><span data-stu-id="372b2-134">The status</span></span>|
|<span data-ttu-id="372b2-135">Observação</span><span class="sxs-lookup"><span data-stu-id="372b2-135">note</span></span>|<span data-ttu-id="372b2-136">String</span><span class="sxs-lookup"><span data-stu-id="372b2-136">String</span></span>|<span data-ttu-id="372b2-137">A observação</span><span class="sxs-lookup"><span data-stu-id="372b2-137">The note</span></span>|



## <a name="response"></a><span data-ttu-id="372b2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="372b2-138">Response</span></span>
<span data-ttu-id="372b2-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="372b2-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="372b2-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="372b2-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="372b2-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="372b2-141">Request</span></span>
<span data-ttu-id="372b2-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="372b2-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus

Content-type: application/json
Content-length: 52

{
  "status": "pending",
  "note": "Note value"
}
```

### <a name="response"></a><span data-ttu-id="372b2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="372b2-143">Response</span></span>
<span data-ttu-id="372b2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="372b2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





