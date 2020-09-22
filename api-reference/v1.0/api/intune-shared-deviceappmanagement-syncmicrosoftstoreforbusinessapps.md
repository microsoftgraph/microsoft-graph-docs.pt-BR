---
title: Ação syncMicrosoftStoreForBusinessApps
description: Sincroniza a conta do Intune com o Microsoft Store For Business
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7a9deb0ab2e84a4debf11040010bc65fad01f65b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019247"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="d5bbd-103">Ação syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="d5bbd-103">syncMicrosoftStoreForBusinessApps action</span></span>

<span data-ttu-id="d5bbd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5bbd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5bbd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5bbd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5bbd-106">Sincroniza a conta do Intune com o Microsoft Store For Business</span><span class="sxs-lookup"><span data-stu-id="d5bbd-106">Syncs Intune account with Microsoft Store For Business</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5bbd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5bbd-107">Prerequisites</span></span>
<span data-ttu-id="d5bbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5bbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5bbd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5bbd-110">Permission type</span></span>|<span data-ttu-id="d5bbd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5bbd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5bbd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5bbd-112">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="d5bbd-113">&nbsp; &nbsp; _Integração_</span><span class="sxs-lookup"><span data-stu-id="d5bbd-113">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="d5bbd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5bbd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d5bbd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5bbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5bbd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5bbd-116">Not supported.</span></span>|
|<span data-ttu-id="d5bbd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5bbd-117">Application</span></span>|<span data-ttu-id="d5bbd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5bbd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5bbd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5bbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="d5bbd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bbd-120">Request headers</span></span>
|<span data-ttu-id="d5bbd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5bbd-121">Header</span></span>|<span data-ttu-id="d5bbd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d5bbd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5bbd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5bbd-123">Authorization</span></span>|<span data-ttu-id="d5bbd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5bbd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5bbd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d5bbd-125">Accept</span></span>|<span data-ttu-id="d5bbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5bbd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5bbd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bbd-127">Request body</span></span>
<span data-ttu-id="d5bbd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d5bbd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5bbd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5bbd-129">Response</span></span>
<span data-ttu-id="d5bbd-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d5bbd-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="d5bbd-131">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bbd-131">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="d5bbd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5bbd-132">Response</span></span>

<span data-ttu-id="d5bbd-133">O objeto de resposta mostrado aqui pode estar truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="d5bbd-133">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d5bbd-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5bbd-134">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









