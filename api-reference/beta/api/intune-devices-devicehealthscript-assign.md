---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1fc94fcaad313677e42014458caee51fb152d91e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945162"
---
# <a name="assign-action"></a><span data-ttu-id="c8c27-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="c8c27-103">assign action</span></span>

> <span data-ttu-id="c8c27-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8c27-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8c27-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8c27-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8c27-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c8c27-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8c27-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8c27-107">Prerequisites</span></span>
<span data-ttu-id="c8c27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8c27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8c27-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8c27-110">Permission type</span></span>|<span data-ttu-id="c8c27-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8c27-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8c27-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8c27-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8c27-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8c27-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c8c27-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8c27-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8c27-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8c27-115">Not supported.</span></span>|
|<span data-ttu-id="c8c27-116">Application</span><span class="sxs-lookup"><span data-stu-id="c8c27-116">Application</span></span>|<span data-ttu-id="c8c27-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8c27-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8c27-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8c27-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="c8c27-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8c27-119">Request headers</span></span>
|<span data-ttu-id="c8c27-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8c27-120">Header</span></span>|<span data-ttu-id="c8c27-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c8c27-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8c27-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8c27-122">Authorization</span></span>|<span data-ttu-id="c8c27-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8c27-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8c27-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8c27-124">Accept</span></span>|<span data-ttu-id="c8c27-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8c27-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8c27-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8c27-126">Request body</span></span>
<span data-ttu-id="c8c27-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c8c27-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c8c27-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c8c27-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c8c27-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8c27-129">Property</span></span>|<span data-ttu-id="c8c27-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8c27-130">Type</span></span>|<span data-ttu-id="c8c27-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8c27-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8c27-132">deviceHealthScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="c8c27-132">deviceHealthScriptAssignments</span></span>|<span data-ttu-id="c8c27-133">coleção [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c8c27-133">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="c8c27-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c8c27-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c8c27-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8c27-135">Response</span></span>
<span data-ttu-id="c8c27-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c8c27-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c8c27-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8c27-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8c27-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8c27-138">Request</span></span>
<span data-ttu-id="c8c27-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8c27-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assign

Content-type: application/json
Content-length: 419

{
  "deviceHealthScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
      "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "runRemediationScript": true,
      "runSchedule": {
        "@odata.type": "microsoft.graph.runSchedule"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c8c27-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8c27-140">Response</span></span>
<span data-ttu-id="c8c27-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8c27-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





