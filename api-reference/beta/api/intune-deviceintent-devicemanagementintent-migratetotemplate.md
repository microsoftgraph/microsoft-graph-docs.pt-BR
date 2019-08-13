---
title: ação migrateToTemplate
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 37e67efff5aef17b82a033e2b76dbeed707e072a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313269"
---
# <a name="migratetotemplate-action"></a><span data-ttu-id="e45e4-103">ação migrateToTemplate</span><span class="sxs-lookup"><span data-stu-id="e45e4-103">migrateToTemplate action</span></span>

> <span data-ttu-id="e45e4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e45e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e45e4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e45e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e45e4-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e45e4-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e45e4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e45e4-107">Prerequisites</span></span>
<span data-ttu-id="e45e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e45e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e45e4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e45e4-110">Permission type</span></span>|<span data-ttu-id="e45e4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e45e4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e45e4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e45e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e45e4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e45e4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e45e4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e45e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e45e4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e45e4-115">Not supported.</span></span>|
|<span data-ttu-id="e45e4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e45e4-116">Application</span></span>|<span data-ttu-id="e45e4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e45e4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e45e4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e45e4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/migrateToTemplate
```

## <a name="request-headers"></a><span data-ttu-id="e45e4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e45e4-119">Request headers</span></span>
|<span data-ttu-id="e45e4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e45e4-120">Header</span></span>|<span data-ttu-id="e45e4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e45e4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e45e4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e45e4-122">Authorization</span></span>|<span data-ttu-id="e45e4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e45e4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e45e4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e45e4-124">Accept</span></span>|<span data-ttu-id="e45e4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e45e4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e45e4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e45e4-126">Request body</span></span>
<span data-ttu-id="e45e4-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e45e4-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e45e4-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="e45e4-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e45e4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e45e4-129">Property</span></span>|<span data-ttu-id="e45e4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e45e4-130">Type</span></span>|<span data-ttu-id="e45e4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e45e4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e45e4-132">newTemplateId</span><span class="sxs-lookup"><span data-stu-id="e45e4-132">newTemplateId</span></span>|<span data-ttu-id="e45e4-133">String</span><span class="sxs-lookup"><span data-stu-id="e45e4-133">String</span></span>|<span data-ttu-id="e45e4-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e45e4-134">Not yet documented</span></span>|
|<span data-ttu-id="e45e4-135">preserveCustomValues</span><span class="sxs-lookup"><span data-stu-id="e45e4-135">preserveCustomValues</span></span>|<span data-ttu-id="e45e4-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="e45e4-136">Boolean</span></span>|<span data-ttu-id="e45e4-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e45e4-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e45e4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e45e4-138">Response</span></span>
<span data-ttu-id="e45e4-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e45e4-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e45e4-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e45e4-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e45e4-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e45e4-141">Request</span></span>
<span data-ttu-id="e45e4-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e45e4-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/migrateToTemplate

Content-type: application/json
Content-length: 81

{
  "newTemplateId": "New Template Id value",
  "preserveCustomValues": true
}
```

### <a name="response"></a><span data-ttu-id="e45e4-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e45e4-143">Response</span></span>
<span data-ttu-id="e45e4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e45e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






