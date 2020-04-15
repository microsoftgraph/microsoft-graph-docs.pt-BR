---
title: Ação syncMicrosoftStoreForBusinessApps
description: Sincroniza a conta do Intune com o Microsoft Store For Business
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6dc04dc9148446da1f51f83fad688d1a9d2ee6b9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465828"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="961ec-103">Ação syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="961ec-103">syncMicrosoftStoreForBusinessApps action</span></span>

<span data-ttu-id="961ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="961ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="961ec-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="961ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="961ec-106">Sincroniza a conta do Intune com o Microsoft Store For Business</span><span class="sxs-lookup"><span data-stu-id="961ec-106">Syncs Intune account with Microsoft Store For Business</span></span>

## <a name="prerequisites"></a><span data-ttu-id="961ec-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="961ec-107">Prerequisites</span></span>
<span data-ttu-id="961ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="961ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="961ec-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="961ec-110">Permission type</span></span>|<span data-ttu-id="961ec-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="961ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="961ec-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="961ec-112">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="961ec-113">&nbsp; &nbsp; _Integração_</span><span class="sxs-lookup"><span data-stu-id="961ec-113">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="961ec-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="961ec-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="961ec-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="961ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="961ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="961ec-116">Not supported.</span></span>|
|<span data-ttu-id="961ec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="961ec-117">Application</span></span>|<span data-ttu-id="961ec-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="961ec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="961ec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="961ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="961ec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="961ec-120">Request headers</span></span>
|<span data-ttu-id="961ec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="961ec-121">Header</span></span>|<span data-ttu-id="961ec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="961ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="961ec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="961ec-123">Authorization</span></span>|<span data-ttu-id="961ec-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="961ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="961ec-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="961ec-125">Accept</span></span>|<span data-ttu-id="961ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="961ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="961ec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="961ec-127">Request body</span></span>
<span data-ttu-id="961ec-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="961ec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="961ec-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="961ec-129">Response</span></span>
<span data-ttu-id="961ec-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="961ec-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="961ec-131">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="961ec-131">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="961ec-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="961ec-132">Response</span></span>

<span data-ttu-id="961ec-133">O objeto de resposta mostrado aqui pode estar truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="961ec-133">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="961ec-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="961ec-134">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






