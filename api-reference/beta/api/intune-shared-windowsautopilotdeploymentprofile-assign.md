---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b1575dbd9812073cee2e4ca88c17569074c11d83
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085497"
---
# <a name="assign-action"></a><span data-ttu-id="9cb43-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="9cb43-103">assign action</span></span>

> <span data-ttu-id="9cb43-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9cb43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cb43-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9cb43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cb43-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9cb43-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cb43-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9cb43-107">Prerequisites</span></span>
<span data-ttu-id="9cb43-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cb43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cb43-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cb43-110">Permission type</span></span>|<span data-ttu-id="9cb43-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9cb43-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cb43-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cb43-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9cb43-113">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="9cb43-113">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="9cb43-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cb43-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="9cb43-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="9cb43-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="9cb43-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cb43-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9cb43-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cb43-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cb43-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cb43-118">Not supported.</span></span>|
|<span data-ttu-id="9cb43-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cb43-119">Application</span></span>||
| <span data-ttu-id="9cb43-120">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="9cb43-120">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="9cb43-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cb43-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="9cb43-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="9cb43-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="9cb43-123">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cb43-123">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cb43-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cb43-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile/assign
```

## <a name="request-headers"></a><span data-ttu-id="9cb43-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cb43-125">Request headers</span></span>
|<span data-ttu-id="9cb43-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9cb43-126">Header</span></span>|<span data-ttu-id="9cb43-127">Valor</span><span class="sxs-lookup"><span data-stu-id="9cb43-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cb43-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cb43-128">Authorization</span></span>|<span data-ttu-id="9cb43-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cb43-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cb43-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9cb43-130">Accept</span></span>|<span data-ttu-id="9cb43-131">application/json</span><span class="sxs-lookup"><span data-stu-id="9cb43-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cb43-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cb43-132">Request body</span></span>
<span data-ttu-id="9cb43-133">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9cb43-133">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9cb43-134">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="9cb43-134">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9cb43-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cb43-135">Property</span></span>|<span data-ttu-id="9cb43-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cb43-136">Type</span></span>|<span data-ttu-id="9cb43-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cb43-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cb43-138">deviceIds</span><span class="sxs-lookup"><span data-stu-id="9cb43-138">deviceIds</span></span>|<span data-ttu-id="9cb43-139">String collection</span><span class="sxs-lookup"><span data-stu-id="9cb43-139">String collection</span></span>|<span data-ttu-id="9cb43-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9cb43-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9cb43-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cb43-141">Response</span></span>
<span data-ttu-id="9cb43-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9cb43-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9cb43-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cb43-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cb43-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cb43-144">Request</span></span>
<span data-ttu-id="9cb43-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cb43-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign

Content-type: application/json
Content-length: 51

{
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="9cb43-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cb43-146">Response</span></span>
<span data-ttu-id="9cb43-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cb43-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









