---
title: Ação setPriority
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 296c3ba32d2460e1e6a47b37e8ee8908e5d0423e
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191674"
---
# <a name="setpriority-action"></a><span data-ttu-id="f4312-103">ação setPriority</span><span class="sxs-lookup"><span data-stu-id="f4312-103">setPriority action</span></span>

> <span data-ttu-id="f4312-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4312-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4312-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4312-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4312-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f4312-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4312-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4312-107">Prerequisites</span></span>
<span data-ttu-id="f4312-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4312-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4312-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4312-110">Permission type</span></span>|<span data-ttu-id="f4312-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4312-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4312-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4312-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4312-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4312-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f4312-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4312-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4312-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4312-115">Not supported.</span></span>|
|<span data-ttu-id="f4312-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4312-116">Application</span></span>|<span data-ttu-id="f4312-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4312-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4312-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4312-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="f4312-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4312-119">Request headers</span></span>
|<span data-ttu-id="f4312-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4312-120">Header</span></span>|<span data-ttu-id="f4312-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f4312-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4312-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4312-122">Authorization</span></span>|<span data-ttu-id="f4312-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4312-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4312-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4312-124">Accept</span></span>|<span data-ttu-id="f4312-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4312-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4312-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4312-126">Request body</span></span>
<span data-ttu-id="f4312-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f4312-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f4312-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f4312-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f4312-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4312-129">Property</span></span>|<span data-ttu-id="f4312-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4312-130">Type</span></span>|<span data-ttu-id="f4312-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4312-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4312-132">Prioridade</span><span class="sxs-lookup"><span data-stu-id="f4312-132">priority</span></span>|<span data-ttu-id="f4312-133">Int32</span><span class="sxs-lookup"><span data-stu-id="f4312-133">Int32</span></span>|<span data-ttu-id="f4312-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f4312-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f4312-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4312-135">Response</span></span>
<span data-ttu-id="f4312-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f4312-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f4312-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4312-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4312-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4312-138">Request</span></span>
<span data-ttu-id="f4312-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4312-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="f4312-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4312-140">Response</span></span>
<span data-ttu-id="f4312-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4312-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




