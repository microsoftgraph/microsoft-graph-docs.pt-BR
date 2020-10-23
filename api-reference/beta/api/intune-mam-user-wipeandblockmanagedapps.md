---
title: ação wipeAndBlockManagedApps
description: Bloqueia o usuário do aplicativo gerenciado do check-in do aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0727ef1dd86159f0a70d31e2d84b914ba4f89cca
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694414"
---
# <a name="wipeandblockmanagedapps-action"></a><span data-ttu-id="2cb67-103">ação wipeAndBlockManagedApps</span><span class="sxs-lookup"><span data-stu-id="2cb67-103">wipeAndBlockManagedApps action</span></span>

<span data-ttu-id="2cb67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cb67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cb67-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2cb67-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cb67-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2cb67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cb67-107">Bloqueia o usuário do aplicativo gerenciado do check-in do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2cb67-107">Blocks the managed app user from app check-in.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cb67-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2cb67-108">Prerequisites</span></span>
<span data-ttu-id="2cb67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cb67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cb67-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2cb67-111">Permission type</span></span>|<span data-ttu-id="2cb67-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2cb67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cb67-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2cb67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2cb67-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cb67-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2cb67-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2cb67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cb67-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cb67-116">Not supported.</span></span>|
|<span data-ttu-id="2cb67-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2cb67-117">Application</span></span>|<span data-ttu-id="2cb67-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cb67-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cb67-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2cb67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeAndBlockManagedApps
```

## <a name="request-headers"></a><span data-ttu-id="2cb67-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2cb67-120">Request headers</span></span>
|<span data-ttu-id="2cb67-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2cb67-121">Header</span></span>|<span data-ttu-id="2cb67-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2cb67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cb67-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2cb67-123">Authorization</span></span>|<span data-ttu-id="2cb67-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2cb67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cb67-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2cb67-125">Accept</span></span>|<span data-ttu-id="2cb67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cb67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cb67-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2cb67-127">Request body</span></span>
<span data-ttu-id="2cb67-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2cb67-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cb67-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cb67-129">Response</span></span>
<span data-ttu-id="2cb67-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2cb67-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2cb67-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2cb67-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cb67-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2cb67-132">Request</span></span>
<span data-ttu-id="2cb67-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2cb67-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeAndBlockManagedApps
```

### <a name="response"></a><span data-ttu-id="2cb67-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cb67-134">Response</span></span>
<span data-ttu-id="2cb67-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2cb67-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





