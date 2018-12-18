---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 0264f5aff78058887e6f219d08812eb6857737ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308173"
---
# <a name="assign-action"></a><span data-ttu-id="b21cf-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="b21cf-103">assign action</span></span>

> <span data-ttu-id="b21cf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b21cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b21cf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b21cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b21cf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b21cf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b21cf-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b21cf-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b21cf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b21cf-108">Prerequisites</span></span>
<span data-ttu-id="b21cf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b21cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b21cf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b21cf-111">Permission type</span></span>|<span data-ttu-id="b21cf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b21cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b21cf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b21cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b21cf-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b21cf-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b21cf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b21cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b21cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b21cf-116">Not supported.</span></span>|
|<span data-ttu-id="b21cf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b21cf-117">Application</span></span>|<span data-ttu-id="b21cf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b21cf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b21cf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b21cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="b21cf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b21cf-120">Request headers</span></span>
|<span data-ttu-id="b21cf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b21cf-121">Header</span></span>|<span data-ttu-id="b21cf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b21cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b21cf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b21cf-123">Authorization</span></span>|<span data-ttu-id="b21cf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b21cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b21cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b21cf-125">Accept</span></span>|<span data-ttu-id="b21cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b21cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b21cf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b21cf-127">Request body</span></span>
<span data-ttu-id="b21cf-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b21cf-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b21cf-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b21cf-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b21cf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b21cf-130">Property</span></span>|<span data-ttu-id="b21cf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b21cf-131">Type</span></span>|<span data-ttu-id="b21cf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b21cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b21cf-133">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="b21cf-133">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="b21cf-134">coleção [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b21cf-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="b21cf-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b21cf-135">Not yet documented</span></span>|
|<span data-ttu-id="b21cf-136">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="b21cf-136">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="b21cf-137">coleção [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b21cf-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="b21cf-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b21cf-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b21cf-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b21cf-139">Response</span></span>
<span data-ttu-id="b21cf-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b21cf-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b21cf-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b21cf-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b21cf-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b21cf-142">Request</span></span>
<span data-ttu-id="b21cf-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b21cf-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign

Content-type: application/json
Content-length: 550

{
  "deviceManagementScriptGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
      "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
      "targetGroupId": "Target Group Id value"
    }
  ],
  "deviceManagementScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
      "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b21cf-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b21cf-144">Response</span></span>
<span data-ttu-id="b21cf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b21cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





