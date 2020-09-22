---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6c138dea3c36f11fb60f834a91fae23293307a0d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085560"
---
# <a name="assign-action"></a><span data-ttu-id="a08c0-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="a08c0-103">assign action</span></span>

<span data-ttu-id="a08c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a08c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a08c0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a08c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a08c0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a08c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a08c0-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a08c0-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a08c0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a08c0-108">Prerequisites</span></span>
<span data-ttu-id="a08c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a08c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a08c0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a08c0-111">Permission type</span></span>|<span data-ttu-id="a08c0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a08c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a08c0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a08c0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a08c0-114">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="a08c0-114">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="a08c0-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a08c0-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="a08c0-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="a08c0-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a08c0-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a08c0-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a08c0-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a08c0-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a08c0-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a08c0-119">Not supported.</span></span>|
|<span data-ttu-id="a08c0-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a08c0-120">Application</span></span>||
| <span data-ttu-id="a08c0-121">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="a08c0-121">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="a08c0-122">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a08c0-122">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="a08c0-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="a08c0-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a08c0-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a08c0-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a08c0-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a08c0-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile/assign
```

## <a name="request-headers"></a><span data-ttu-id="a08c0-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a08c0-126">Request headers</span></span>
|<span data-ttu-id="a08c0-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a08c0-127">Header</span></span>|<span data-ttu-id="a08c0-128">Valor</span><span class="sxs-lookup"><span data-stu-id="a08c0-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a08c0-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="a08c0-129">Authorization</span></span>|<span data-ttu-id="a08c0-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a08c0-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a08c0-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a08c0-131">Accept</span></span>|<span data-ttu-id="a08c0-132">application/json</span><span class="sxs-lookup"><span data-stu-id="a08c0-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a08c0-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a08c0-133">Request body</span></span>
<span data-ttu-id="a08c0-134">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a08c0-134">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a08c0-135">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="a08c0-135">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a08c0-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a08c0-136">Property</span></span>|<span data-ttu-id="a08c0-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="a08c0-137">Type</span></span>|<span data-ttu-id="a08c0-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="a08c0-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a08c0-139">deviceIds</span><span class="sxs-lookup"><span data-stu-id="a08c0-139">deviceIds</span></span>|<span data-ttu-id="a08c0-140">String collection</span><span class="sxs-lookup"><span data-stu-id="a08c0-140">String collection</span></span>|<span data-ttu-id="a08c0-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a08c0-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a08c0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a08c0-142">Response</span></span>
<span data-ttu-id="a08c0-143">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a08c0-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a08c0-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a08c0-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="a08c0-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a08c0-145">Request</span></span>
<span data-ttu-id="a08c0-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a08c0-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a08c0-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="a08c0-147">Response</span></span>
<span data-ttu-id="a08c0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a08c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









