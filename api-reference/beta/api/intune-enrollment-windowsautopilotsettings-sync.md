---
title: ação sync
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d690feeb875300e44fd8715e95ada602c2b9525
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908116"
---
# <a name="sync-action"></a><span data-ttu-id="e3037-103">Ação sync</span><span class="sxs-lookup"><span data-stu-id="e3037-103">sync action</span></span>

> <span data-ttu-id="e3037-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e3037-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3037-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3037-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3037-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e3037-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3037-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3037-107">Prerequisites</span></span>
<span data-ttu-id="e3037-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3037-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3037-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3037-110">Permission type</span></span>|<span data-ttu-id="e3037-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3037-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3037-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3037-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e3037-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3037-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e3037-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3037-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3037-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3037-115">Not supported.</span></span>|
|<span data-ttu-id="e3037-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3037-116">Application</span></span>|<span data-ttu-id="e3037-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3037-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3037-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3037-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotSettings/sync
```

## <a name="request-headers"></a><span data-ttu-id="e3037-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3037-119">Request headers</span></span>
|<span data-ttu-id="e3037-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3037-120">Header</span></span>|<span data-ttu-id="e3037-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e3037-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3037-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3037-122">Authorization</span></span>|<span data-ttu-id="e3037-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3037-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3037-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3037-124">Accept</span></span>|<span data-ttu-id="e3037-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e3037-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3037-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3037-126">Request body</span></span>
<span data-ttu-id="e3037-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3037-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3037-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3037-128">Response</span></span>
<span data-ttu-id="e3037-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e3037-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e3037-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3037-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3037-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3037-131">Request</span></span>
<span data-ttu-id="e3037-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3037-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings/sync
```

### <a name="response"></a><span data-ttu-id="e3037-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3037-133">Response</span></span>
<span data-ttu-id="e3037-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3037-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




