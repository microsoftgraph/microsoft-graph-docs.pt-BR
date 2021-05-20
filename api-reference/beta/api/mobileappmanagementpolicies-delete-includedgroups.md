---
title: Excluir includedGroup
description: Exclua um grupo da lista de grupos incluídos em uma política de gerenciamento de aplicativo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7fb2c501ca1d052a6a97361faee79b06ddcb9671
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547348"
---
# <a name="delete-includedgroup"></a><span data-ttu-id="6a96e-103">Excluir includedGroup</span><span class="sxs-lookup"><span data-stu-id="6a96e-103">Delete includedGroup</span></span>

<span data-ttu-id="6a96e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a96e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a96e-105">Exclua um grupo da lista de grupos incluídos em uma política de gerenciamento de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="6a96e-105">Delete a group from the list of groups included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a96e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a96e-106">Permissions</span></span>

<span data-ttu-id="6a96e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a96e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a96e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a96e-109">Permission type</span></span>|<span data-ttu-id="6a96e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a96e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a96e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a96e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a96e-112">Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a96e-112">Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="6a96e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a96e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a96e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a96e-114">Not supported.</span></span>|
|<span data-ttu-id="6a96e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a96e-115">Application</span></span> | <span data-ttu-id="6a96e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a96e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a96e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a96e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileAppManagementPolicies/{id}/includedGroups/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6a96e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a96e-118">Request headers</span></span>

|<span data-ttu-id="6a96e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6a96e-119">Name</span></span>|<span data-ttu-id="6a96e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a96e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6a96e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a96e-121">Authorization</span></span>|<span data-ttu-id="6a96e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a96e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a96e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a96e-124">Request body</span></span>

<span data-ttu-id="6a96e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a96e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a96e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a96e-126">Response</span></span>

<span data-ttu-id="6a96e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a96e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a96e-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6a96e-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a96e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a96e-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_group"
}
-->

```http
DELETE https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/1a9db3ab-0acf-4808-99ae-e8ed581cb2e0/$ref
```

### <a name="response"></a><span data-ttu-id="6a96e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a96e-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
