---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c8dc350b612fa2d90571fb73b933ec033665acf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167736"
---
# <a name="assign-action"></a><span data-ttu-id="f4001-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="f4001-103">assign action</span></span>

> <span data-ttu-id="f4001-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4001-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4001-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4001-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4001-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f4001-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4001-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4001-107">Prerequisites</span></span>
<span data-ttu-id="f4001-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f4001-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4001-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4001-110">Permission type</span></span>|<span data-ttu-id="f4001-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4001-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4001-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4001-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4001-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4001-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f4001-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4001-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4001-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4001-115">Not supported.</span></span>|
|<span data-ttu-id="f4001-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4001-116">Application</span></span>|<span data-ttu-id="f4001-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4001-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4001-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4001-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile/assign
```

## <a name="request-headers"></a><span data-ttu-id="f4001-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4001-119">Request headers</span></span>
|<span data-ttu-id="f4001-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4001-120">Header</span></span>|<span data-ttu-id="f4001-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f4001-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4001-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4001-122">Authorization</span></span>|<span data-ttu-id="f4001-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4001-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4001-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4001-124">Accept</span></span>|<span data-ttu-id="f4001-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4001-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4001-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4001-126">Request body</span></span>
<span data-ttu-id="f4001-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f4001-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f4001-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f4001-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f4001-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4001-129">Property</span></span>|<span data-ttu-id="f4001-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4001-130">Type</span></span>|<span data-ttu-id="f4001-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4001-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4001-132">deviceIds</span><span class="sxs-lookup"><span data-stu-id="f4001-132">deviceIds</span></span>|<span data-ttu-id="f4001-133">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f4001-133">String collection</span></span>|<span data-ttu-id="f4001-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f4001-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f4001-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4001-135">Response</span></span>
<span data-ttu-id="f4001-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f4001-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f4001-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4001-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4001-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4001-138">Request</span></span>
<span data-ttu-id="f4001-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4001-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4001-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4001-140">Response</span></span>
<span data-ttu-id="f4001-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4001-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




