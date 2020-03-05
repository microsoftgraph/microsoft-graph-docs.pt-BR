---
title: Excluir deviceManagementIntentUserState
description: Exclui deviceManagementIntentUserState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4b9b3033e0efd702b448c6011c75c7808d23be9f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470788"
---
# <a name="delete-devicemanagementintentuserstate"></a><span data-ttu-id="bcccf-103">Excluir deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="bcccf-103">Delete deviceManagementIntentUserState</span></span>

<span data-ttu-id="bcccf-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bcccf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bcccf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bcccf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcccf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bcccf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcccf-107">Exclui [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span><span class="sxs-lookup"><span data-stu-id="bcccf-107">Deletes a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcccf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bcccf-108">Prerequisites</span></span>
<span data-ttu-id="bcccf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcccf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcccf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcccf-111">Permission type</span></span>|<span data-ttu-id="bcccf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bcccf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcccf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcccf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bcccf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcccf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bcccf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcccf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcccf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcccf-116">Not supported.</span></span>|
|<span data-ttu-id="bcccf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bcccf-117">Application</span></span>|<span data-ttu-id="bcccf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcccf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcccf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcccf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="bcccf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcccf-120">Request headers</span></span>
|<span data-ttu-id="bcccf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bcccf-121">Header</span></span>|<span data-ttu-id="bcccf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bcccf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcccf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcccf-123">Authorization</span></span>|<span data-ttu-id="bcccf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcccf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcccf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bcccf-125">Accept</span></span>|<span data-ttu-id="bcccf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bcccf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcccf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcccf-127">Request body</span></span>
<span data-ttu-id="bcccf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bcccf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcccf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcccf-129">Response</span></span>
<span data-ttu-id="bcccf-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bcccf-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bcccf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bcccf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcccf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcccf-132">Request</span></span>
<span data-ttu-id="bcccf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcccf-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
```

### <a name="response"></a><span data-ttu-id="bcccf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcccf-134">Response</span></span>
<span data-ttu-id="bcccf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bcccf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





