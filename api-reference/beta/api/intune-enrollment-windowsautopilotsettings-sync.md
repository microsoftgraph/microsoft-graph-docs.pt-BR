---
title: ação sync
description: Inicia uma sincronização de todos os dispositivos registrados do AutoPilot na Loja para Empresas e em outros portais. Se a sincronização for bem-sucedida, essa ação retornará um código de resposta 204 No Content. Se uma sincronização já estiver em andamento, a ação retornará um código de resposta de conflito 409.  Se essa ação de sincronização for chamada dentro de 10 minutos após a sincronização anterior, a ação retornará um código de resposta 429 Solicitações Demais.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 047d03ac938dabf185173a6fea3e01c8b17e3a9c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158797"
---
# <a name="sync-action"></a><span data-ttu-id="564f3-106">Ação sync</span><span class="sxs-lookup"><span data-stu-id="564f3-106">sync action</span></span>

<span data-ttu-id="564f3-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="564f3-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="564f3-108">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="564f3-108">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="564f3-109">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="564f3-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="564f3-110">Inicia uma sincronização de todos os dispositivos registrados do AutoPilot na Loja para Empresas e em outros portais.</span><span class="sxs-lookup"><span data-stu-id="564f3-110">Initiates a sync of all AutoPilot registered devices from Store for Business and other portals.</span></span> <span data-ttu-id="564f3-111">Se a sincronização for bem-sucedida, essa ação retornará um código de resposta 204 No Content.</span><span class="sxs-lookup"><span data-stu-id="564f3-111">If the sync successful, this action returns a 204 No Content response code.</span></span> <span data-ttu-id="564f3-112">Se uma sincronização já estiver em andamento, a ação retornará um código de resposta de conflito 409.</span><span class="sxs-lookup"><span data-stu-id="564f3-112">If a sync is already in progress, the action returns a 409 Conflict response code.</span></span>  <span data-ttu-id="564f3-113">Se essa ação de sincronização for chamada dentro de 10 minutos após a sincronização anterior, a ação retornará um código de resposta 429 Solicitações Demais.</span><span class="sxs-lookup"><span data-stu-id="564f3-113">If this sync action is called within 10 minutes of the previous sync, the action returns a 429 Too Many Requests response code.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="564f3-114">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="564f3-114">Prerequisites</span></span>
<span data-ttu-id="564f3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="564f3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="564f3-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="564f3-117">Permission type</span></span>|<span data-ttu-id="564f3-118">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="564f3-118">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="564f3-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="564f3-119">Delegated (work or school account)</span></span>|<span data-ttu-id="564f3-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="564f3-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="564f3-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="564f3-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="564f3-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="564f3-122">Not supported.</span></span>|
|<span data-ttu-id="564f3-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="564f3-123">Application</span></span>|<span data-ttu-id="564f3-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="564f3-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="564f3-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="564f3-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotSettings/sync
```

## <a name="request-headers"></a><span data-ttu-id="564f3-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="564f3-126">Request headers</span></span>
|<span data-ttu-id="564f3-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="564f3-127">Header</span></span>|<span data-ttu-id="564f3-128">Valor</span><span class="sxs-lookup"><span data-stu-id="564f3-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="564f3-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="564f3-129">Authorization</span></span>|<span data-ttu-id="564f3-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="564f3-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="564f3-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="564f3-131">Accept</span></span>|<span data-ttu-id="564f3-132">application/json</span><span class="sxs-lookup"><span data-stu-id="564f3-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="564f3-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="564f3-133">Request body</span></span>
<span data-ttu-id="564f3-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="564f3-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="564f3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="564f3-135">Response</span></span>
<span data-ttu-id="564f3-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="564f3-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="564f3-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="564f3-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="564f3-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="564f3-138">Request</span></span>
<span data-ttu-id="564f3-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="564f3-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings/sync
```

### <a name="response"></a><span data-ttu-id="564f3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="564f3-140">Response</span></span>
<span data-ttu-id="564f3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="564f3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




