---
title: ação sync
description: Inicia uma sincronização de todos os dispositivos registrados do AutoPilot da Store para Empresas e de outros portais. Se a sincronização for bem-sucedida, essa ação retornará um código de resposta 204 No Content. Se uma sincronização já estiver em andamento, a ação retornará um código de resposta conflict 409.  Se essa ação de sincronização for chamada dentro de 10 minutos da sincronização anterior, a ação retornará um código de resposta 429 Solicitações Demais.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4505bc6530a74d16ff77471992fc6a835a04320c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149853"
---
# <a name="sync-action"></a><span data-ttu-id="346f4-106">Ação sync</span><span class="sxs-lookup"><span data-stu-id="346f4-106">sync action</span></span>

<span data-ttu-id="346f4-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="346f4-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="346f4-108">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="346f4-108">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="346f4-109">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="346f4-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="346f4-110">Inicia uma sincronização de todos os dispositivos registrados do AutoPilot da Store para Empresas e de outros portais.</span><span class="sxs-lookup"><span data-stu-id="346f4-110">Initiates a sync of all AutoPilot registered devices from Store for Business and other portals.</span></span> <span data-ttu-id="346f4-111">Se a sincronização for bem-sucedida, essa ação retornará um código de resposta 204 No Content.</span><span class="sxs-lookup"><span data-stu-id="346f4-111">If the sync successful, this action returns a 204 No Content response code.</span></span> <span data-ttu-id="346f4-112">Se uma sincronização já estiver em andamento, a ação retornará um código de resposta conflict 409.</span><span class="sxs-lookup"><span data-stu-id="346f4-112">If a sync is already in progress, the action returns a 409 Conflict response code.</span></span>  <span data-ttu-id="346f4-113">Se essa ação de sincronização for chamada dentro de 10 minutos da sincronização anterior, a ação retornará um código de resposta 429 Solicitações Demais.</span><span class="sxs-lookup"><span data-stu-id="346f4-113">If this sync action is called within 10 minutes of the previous sync, the action returns a 429 Too Many Requests response code.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="346f4-114">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="346f4-114">Prerequisites</span></span>
<span data-ttu-id="346f4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="346f4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="346f4-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="346f4-117">Permission type</span></span>|<span data-ttu-id="346f4-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="346f4-118">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="346f4-119">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="346f4-119">Delegated (work or school account)</span></span>|<span data-ttu-id="346f4-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="346f4-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="346f4-121">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="346f4-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="346f4-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="346f4-122">Not supported.</span></span>|
|<span data-ttu-id="346f4-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="346f4-123">Application</span></span>|<span data-ttu-id="346f4-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="346f4-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="346f4-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="346f4-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotSettings/sync
```

## <a name="request-headers"></a><span data-ttu-id="346f4-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="346f4-126">Request headers</span></span>
|<span data-ttu-id="346f4-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="346f4-127">Header</span></span>|<span data-ttu-id="346f4-128">Valor</span><span class="sxs-lookup"><span data-stu-id="346f4-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="346f4-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="346f4-129">Authorization</span></span>|<span data-ttu-id="346f4-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="346f4-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="346f4-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="346f4-131">Accept</span></span>|<span data-ttu-id="346f4-132">application/json</span><span class="sxs-lookup"><span data-stu-id="346f4-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="346f4-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="346f4-133">Request body</span></span>
<span data-ttu-id="346f4-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="346f4-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="346f4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="346f4-135">Response</span></span>
<span data-ttu-id="346f4-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="346f4-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="346f4-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="346f4-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="346f4-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="346f4-138">Request</span></span>
<span data-ttu-id="346f4-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="346f4-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings/sync
```

### <a name="response"></a><span data-ttu-id="346f4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="346f4-140">Response</span></span>
<span data-ttu-id="346f4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="346f4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




