---
title: ação migrateToTemplate
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab0ee2caf8af1e4cc91f3ca27a3e591e860eb990
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000683"
---
# <a name="migratetotemplate-action"></a><span data-ttu-id="03507-103">ação migrateToTemplate</span><span class="sxs-lookup"><span data-stu-id="03507-103">migrateToTemplate action</span></span>

<span data-ttu-id="03507-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03507-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03507-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="03507-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03507-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03507-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03507-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="03507-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03507-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03507-108">Prerequisites</span></span>
<span data-ttu-id="03507-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03507-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03507-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03507-111">Permission type</span></span>|<span data-ttu-id="03507-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="03507-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03507-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03507-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03507-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03507-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03507-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03507-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03507-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03507-116">Not supported.</span></span>|
|<span data-ttu-id="03507-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03507-117">Application</span></span>|<span data-ttu-id="03507-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03507-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03507-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03507-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/migrateToTemplate
```

## <a name="request-headers"></a><span data-ttu-id="03507-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03507-120">Request headers</span></span>
|<span data-ttu-id="03507-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03507-121">Header</span></span>|<span data-ttu-id="03507-122">Valor</span><span class="sxs-lookup"><span data-stu-id="03507-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03507-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="03507-123">Authorization</span></span>|<span data-ttu-id="03507-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03507-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03507-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03507-125">Accept</span></span>|<span data-ttu-id="03507-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03507-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03507-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03507-127">Request body</span></span>
<span data-ttu-id="03507-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="03507-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="03507-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="03507-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="03507-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03507-130">Property</span></span>|<span data-ttu-id="03507-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="03507-131">Type</span></span>|<span data-ttu-id="03507-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="03507-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03507-133">newTemplateId</span><span class="sxs-lookup"><span data-stu-id="03507-133">newTemplateId</span></span>|<span data-ttu-id="03507-134">String</span><span class="sxs-lookup"><span data-stu-id="03507-134">String</span></span>|<span data-ttu-id="03507-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="03507-135">Not yet documented</span></span>|
|<span data-ttu-id="03507-136">preserveCustomValues</span><span class="sxs-lookup"><span data-stu-id="03507-136">preserveCustomValues</span></span>|<span data-ttu-id="03507-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="03507-137">Boolean</span></span>|<span data-ttu-id="03507-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="03507-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="03507-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="03507-139">Response</span></span>
<span data-ttu-id="03507-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="03507-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="03507-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03507-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="03507-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03507-142">Request</span></span>
<span data-ttu-id="03507-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03507-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/migrateToTemplate

Content-type: application/json
Content-length: 81

{
  "newTemplateId": "New Template Id value",
  "preserveCustomValues": true
}
```

### <a name="response"></a><span data-ttu-id="03507-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="03507-144">Response</span></span>
<span data-ttu-id="03507-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03507-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






