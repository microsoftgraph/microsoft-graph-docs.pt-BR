---
title: Ação beginOnboarding
description: Uma solicitação para iniciar a integração.  Deve ser associado às informações de conta do TeamViewer apropriadas
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36fa3b2d27bbcad94ad2427c5a248a3ae5360fc8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789868"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="7c6f7-104">Ação beginOnboarding</span><span class="sxs-lookup"><span data-stu-id="7c6f7-104">beginOnboarding action</span></span>

> <span data-ttu-id="7c6f7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c6f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c6f7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c6f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c6f7-107">Uma solicitação para iniciar a integração.</span><span class="sxs-lookup"><span data-stu-id="7c6f7-107">A request to start onboarding.</span></span>  <span data-ttu-id="7c6f7-108">Deve ser associado às informações de conta do TeamViewer apropriadas</span><span class="sxs-lookup"><span data-stu-id="7c6f7-108">Must be coupled with the appropriate TeamViewer account information</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c6f7-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c6f7-109">Prerequisites</span></span>
<span data-ttu-id="7c6f7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c6f7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c6f7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c6f7-112">Permission type</span></span>|<span data-ttu-id="7c6f7-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7c6f7-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c6f7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c6f7-114">Delegated (work or school account)</span></span>|<span data-ttu-id="7c6f7-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c6f7-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7c6f7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c6f7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c6f7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c6f7-117">Not supported.</span></span>|
|<span data-ttu-id="7c6f7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c6f7-118">Application</span></span>|<span data-ttu-id="7c6f7-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c6f7-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c6f7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c6f7-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="7c6f7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c6f7-121">Request headers</span></span>
|<span data-ttu-id="7c6f7-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c6f7-122">Header</span></span>|<span data-ttu-id="7c6f7-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7c6f7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c6f7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c6f7-124">Authorization</span></span>|<span data-ttu-id="7c6f7-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c6f7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c6f7-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c6f7-126">Accept</span></span>|<span data-ttu-id="7c6f7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7c6f7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c6f7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c6f7-128">Request body</span></span>
<span data-ttu-id="7c6f7-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c6f7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c6f7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c6f7-130">Response</span></span>
<span data-ttu-id="7c6f7-131">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7c6f7-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7c6f7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c6f7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c6f7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c6f7-133">Request</span></span>
<span data-ttu-id="7c6f7-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c6f7-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="7c6f7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c6f7-135">Response</span></span>
<span data-ttu-id="7c6f7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c6f7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





