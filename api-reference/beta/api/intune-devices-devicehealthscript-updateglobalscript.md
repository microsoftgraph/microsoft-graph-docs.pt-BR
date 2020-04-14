---
title: ação updateGlobalScript
description: Atualizar o script de integridade do dispositivo proprietário
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 42cd16873e374dfbc301674c2a7c76527311581a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43426345"
---
# <a name="updateglobalscript-action"></a><span data-ttu-id="a301e-103">ação updateGlobalScript</span><span class="sxs-lookup"><span data-stu-id="a301e-103">updateGlobalScript action</span></span>

<span data-ttu-id="a301e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a301e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a301e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a301e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a301e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a301e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a301e-107">Atualizar o script de integridade do dispositivo proprietário</span><span class="sxs-lookup"><span data-stu-id="a301e-107">Update the Proprietary Device Health Script</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a301e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a301e-108">Prerequisites</span></span>
<span data-ttu-id="a301e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a301e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a301e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a301e-111">Permission type</span></span>|<span data-ttu-id="a301e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a301e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a301e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a301e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a301e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a301e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a301e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a301e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a301e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a301e-116">Not supported.</span></span>|
|<span data-ttu-id="a301e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a301e-117">Application</span></span>|<span data-ttu-id="a301e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a301e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a301e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a301e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/updateGlobalScript
```

## <a name="request-headers"></a><span data-ttu-id="a301e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a301e-120">Request headers</span></span>
|<span data-ttu-id="a301e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a301e-121">Header</span></span>|<span data-ttu-id="a301e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a301e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a301e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a301e-123">Authorization</span></span>|<span data-ttu-id="a301e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a301e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a301e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a301e-125">Accept</span></span>|<span data-ttu-id="a301e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a301e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a301e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a301e-127">Request body</span></span>
<span data-ttu-id="a301e-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a301e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a301e-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="a301e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a301e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a301e-130">Property</span></span>|<span data-ttu-id="a301e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a301e-131">Type</span></span>|<span data-ttu-id="a301e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a301e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a301e-133">versão</span><span class="sxs-lookup"><span data-stu-id="a301e-133">version</span></span>|<span data-ttu-id="a301e-134">String</span><span class="sxs-lookup"><span data-stu-id="a301e-134">String</span></span>|<span data-ttu-id="a301e-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a301e-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a301e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a301e-136">Response</span></span>
<span data-ttu-id="a301e-137">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a301e-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a301e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a301e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a301e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a301e-139">Request</span></span>
<span data-ttu-id="a301e-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a301e-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/updateGlobalScript

Content-type: application/json
Content-length: 34

{
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="a301e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a301e-141">Response</span></span>
<span data-ttu-id="a301e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a301e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 45

{
  "value": "Update Global Script value"
}
```



