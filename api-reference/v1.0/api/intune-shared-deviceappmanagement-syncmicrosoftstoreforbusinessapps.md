---
title: Ação syncMicrosoftStoreForBusinessApps
description: Sincroniza a conta do Intune com o Microsoft Store para Empresas
author: tfitzmac
ms.openlocfilehash: b26b379631cf5b28594e3cf247b735d6118e9b40
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354331"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="57ff0-103">Ação syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="57ff0-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="57ff0-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="57ff0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57ff0-105">Sincroniza a conta do Intune com o Microsoft Store For Business</span><span class="sxs-lookup"><span data-stu-id="57ff0-105">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57ff0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57ff0-106">Prerequisites</span></span>
<span data-ttu-id="57ff0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57ff0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57ff0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57ff0-109">Permission type</span></span>|<span data-ttu-id="57ff0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57ff0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57ff0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57ff0-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="57ff0-112">&nbsp;&nbsp; _Onboarding_</span><span class="sxs-lookup"><span data-stu-id="57ff0-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="57ff0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57ff0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="57ff0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57ff0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57ff0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57ff0-115">Not supported.</span></span>|
|<span data-ttu-id="57ff0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57ff0-116">Application</span></span>|<span data-ttu-id="57ff0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57ff0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57ff0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57ff0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="57ff0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57ff0-119">Request headers</span></span>
|<span data-ttu-id="57ff0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57ff0-120">Header</span></span>|<span data-ttu-id="57ff0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="57ff0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57ff0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="57ff0-122">Authorization</span></span>|<span data-ttu-id="57ff0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57ff0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57ff0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="57ff0-124">Accept</span></span>|<span data-ttu-id="57ff0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57ff0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57ff0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57ff0-126">Request body</span></span>
<span data-ttu-id="57ff0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57ff0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57ff0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="57ff0-128">Response</span></span>
<span data-ttu-id="57ff0-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="57ff0-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="57ff0-130">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="57ff0-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="57ff0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="57ff0-131">Response</span></span>

<span data-ttu-id="57ff0-132">No objeto response mostrado aqui pode estar truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="57ff0-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="57ff0-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57ff0-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



