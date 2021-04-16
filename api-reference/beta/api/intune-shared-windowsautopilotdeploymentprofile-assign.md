---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2c13bd6798c6a73b953b3f273c76a9dee1365ab
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868068"
---
# <a name="assign-action"></a><span data-ttu-id="47300-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="47300-103">assign action</span></span>

<span data-ttu-id="47300-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47300-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47300-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47300-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47300-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47300-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47300-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="47300-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47300-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47300-108">Prerequisites</span></span>
<span data-ttu-id="47300-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47300-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47300-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47300-111">Permission type</span></span>|<span data-ttu-id="47300-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47300-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47300-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47300-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="47300-114">&nbsp;&nbsp; **Inscrição**</span><span class="sxs-lookup"><span data-stu-id="47300-114">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="47300-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47300-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="47300-116">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="47300-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="47300-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47300-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="47300-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47300-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47300-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47300-119">Not supported.</span></span>|
|<span data-ttu-id="47300-120">Application</span><span class="sxs-lookup"><span data-stu-id="47300-120">Application</span></span>||
| <span data-ttu-id="47300-121">&nbsp;&nbsp; **Inscrição**</span><span class="sxs-lookup"><span data-stu-id="47300-121">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="47300-122">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47300-122">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="47300-123">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="47300-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="47300-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47300-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47300-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47300-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile/assign
```

## <a name="request-headers"></a><span data-ttu-id="47300-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47300-126">Request headers</span></span>
|<span data-ttu-id="47300-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47300-127">Header</span></span>|<span data-ttu-id="47300-128">Valor</span><span class="sxs-lookup"><span data-stu-id="47300-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47300-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="47300-129">Authorization</span></span>|<span data-ttu-id="47300-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47300-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47300-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47300-131">Accept</span></span>|<span data-ttu-id="47300-132">application/json</span><span class="sxs-lookup"><span data-stu-id="47300-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47300-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47300-133">Request body</span></span>
<span data-ttu-id="47300-134">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="47300-134">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="47300-135">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="47300-135">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="47300-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47300-136">Property</span></span>|<span data-ttu-id="47300-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="47300-137">Type</span></span>|<span data-ttu-id="47300-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="47300-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47300-139">deviceIds</span><span class="sxs-lookup"><span data-stu-id="47300-139">deviceIds</span></span>|<span data-ttu-id="47300-140">String collection</span><span class="sxs-lookup"><span data-stu-id="47300-140">String collection</span></span>|<span data-ttu-id="47300-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="47300-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="47300-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="47300-142">Response</span></span>
<span data-ttu-id="47300-143">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="47300-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="47300-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47300-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="47300-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47300-145">Request</span></span>
<span data-ttu-id="47300-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47300-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47300-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="47300-147">Response</span></span>
<span data-ttu-id="47300-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47300-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







