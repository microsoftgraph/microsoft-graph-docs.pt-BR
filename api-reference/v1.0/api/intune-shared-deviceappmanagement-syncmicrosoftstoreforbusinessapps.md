---
title: Ação syncMicrosoftStoreForBusinessApps
description: Sincroniza a conta do Intune com o Microsoft Store para Empresas
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0c2537ac8b093a94b22969d6e1cb776fc061a365
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941636"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="76361-103">Ação syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="76361-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="76361-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="76361-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76361-105">Sincroniza a conta do Intune com o Microsoft Store For Business</span><span class="sxs-lookup"><span data-stu-id="76361-105">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="76361-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76361-106">Prerequisites</span></span>
<span data-ttu-id="76361-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76361-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76361-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76361-109">Permission type</span></span>|<span data-ttu-id="76361-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="76361-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76361-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76361-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="76361-112">&nbsp;&nbsp; _Onboarding_</span><span class="sxs-lookup"><span data-stu-id="76361-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="76361-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76361-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="76361-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76361-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76361-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76361-115">Not supported.</span></span>|
|<span data-ttu-id="76361-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76361-116">Application</span></span>|<span data-ttu-id="76361-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76361-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76361-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76361-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="76361-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76361-119">Request headers</span></span>
|<span data-ttu-id="76361-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76361-120">Header</span></span>|<span data-ttu-id="76361-121">Valor</span><span class="sxs-lookup"><span data-stu-id="76361-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76361-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="76361-122">Authorization</span></span>|<span data-ttu-id="76361-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76361-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76361-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76361-124">Accept</span></span>|<span data-ttu-id="76361-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76361-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76361-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76361-126">Request body</span></span>
<span data-ttu-id="76361-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="76361-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76361-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="76361-128">Response</span></span>
<span data-ttu-id="76361-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="76361-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="76361-130">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="76361-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="76361-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="76361-131">Response</span></span>

<span data-ttu-id="76361-132">No objeto response mostrado aqui pode estar truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="76361-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="76361-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76361-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



