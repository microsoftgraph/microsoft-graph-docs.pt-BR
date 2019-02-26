---
title: Ação syncMicrosoftStoreForBusinessApps
description: Sincroniza a conta do Intune com o Microsoft Store para Empresas
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e71bfb1e4ac6d4ce6c31344289eab7fb15b65594
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254265"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="839f6-103">Ação syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="839f6-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="839f6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="839f6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="839f6-105">Sincroniza a conta do Intune com o Microsoft Store For Business</span><span class="sxs-lookup"><span data-stu-id="839f6-105">Syncs Intune account with Microsoft Store For Business</span></span>

## <a name="prerequisites"></a><span data-ttu-id="839f6-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="839f6-106">Prerequisites</span></span>
<span data-ttu-id="839f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="839f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="839f6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="839f6-109">Permission type</span></span>|<span data-ttu-id="839f6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="839f6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="839f6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="839f6-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="839f6-112">&nbsp; &nbsp; _Integração_</span><span class="sxs-lookup"><span data-stu-id="839f6-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="839f6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="839f6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="839f6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="839f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="839f6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="839f6-115">Not supported.</span></span>|
|<span data-ttu-id="839f6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="839f6-116">Application</span></span>|<span data-ttu-id="839f6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="839f6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="839f6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="839f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="839f6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="839f6-119">Request headers</span></span>
|<span data-ttu-id="839f6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="839f6-120">Header</span></span>|<span data-ttu-id="839f6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="839f6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="839f6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="839f6-122">Authorization</span></span>|<span data-ttu-id="839f6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="839f6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="839f6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="839f6-124">Accept</span></span>|<span data-ttu-id="839f6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="839f6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="839f6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="839f6-126">Request body</span></span>
<span data-ttu-id="839f6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="839f6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="839f6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="839f6-128">Response</span></span>
<span data-ttu-id="839f6-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="839f6-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="839f6-130">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="839f6-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="839f6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="839f6-131">Response</span></span>

<span data-ttu-id="839f6-132">O objeto de resposta mostrado aqui pode estar truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="839f6-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="839f6-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="839f6-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



