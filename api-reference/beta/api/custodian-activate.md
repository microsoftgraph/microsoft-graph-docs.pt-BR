---
title: 'responsáveis: ativar'
description: Reative um dos responsáveis em uma ocorrência.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 40ac381da15065a4363471ba9c82c19080b84884
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597494"
---
# <a name="custodian-activate"></a><span data-ttu-id="95b0d-103">responsáveis: ativar</span><span class="sxs-lookup"><span data-stu-id="95b0d-103">custodian: activate</span></span>

<span data-ttu-id="95b0d-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="95b0d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95b0d-105">Ative um dos responsáveis que tenha sido liberado de um caso para torná-los parte do caso novamente.</span><span class="sxs-lookup"><span data-stu-id="95b0d-105">Activate a custodian that has been released from a case to make them part of the case again.</span></span> <span data-ttu-id="95b0d-106">Para obter detalhes, consulte [Manage responsáveis em um caso de descoberta eletrônica avançada](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian).</span><span class="sxs-lookup"><span data-stu-id="95b0d-106">For details, see [Manage custodians in an Advanced eDiscovery case](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian).</span></span>

## <a name="permissions"></a><span data-ttu-id="95b0d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="95b0d-107">Permissions</span></span>

<span data-ttu-id="95b0d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95b0d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95b0d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95b0d-110">Permission type</span></span>|<span data-ttu-id="95b0d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="95b0d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95b0d-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95b0d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95b0d-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="95b0d-113">User.Read</span></span>|
|<span data-ttu-id="95b0d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95b0d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95b0d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95b0d-115">Not supported.</span></span>|
|<span data-ttu-id="95b0d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95b0d-116">Application</span></span>|<span data-ttu-id="95b0d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95b0d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95b0d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95b0d-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/activate
```

## <a name="request-headers"></a><span data-ttu-id="95b0d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95b0d-119">Request headers</span></span>

|<span data-ttu-id="95b0d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="95b0d-120">Name</span></span>|<span data-ttu-id="95b0d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="95b0d-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="95b0d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="95b0d-122">Authorization</span></span>|<span data-ttu-id="95b0d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95b0d-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="95b0d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95b0d-125">Content-Type</span></span>|<span data-ttu-id="95b0d-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95b0d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="95b0d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95b0d-128">Request body</span></span>

<span data-ttu-id="95b0d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95b0d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95b0d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="95b0d-130">Response</span></span>

<span data-ttu-id="95b0d-131">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="95b0d-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="95b0d-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="95b0d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="95b0d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95b0d-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "custodian_activate"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/activate
```

### <a name="response"></a><span data-ttu-id="95b0d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="95b0d-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
