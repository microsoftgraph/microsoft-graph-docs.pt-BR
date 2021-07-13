---
title: Excluir includedGroup
description: Exclua um grupo da lista de grupos incluídos em uma política de gerenciamento de aplicativo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 00f49c6c0ccb34fd18de68b65fc9f6ce7ff94605
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401360"
---
# <a name="delete-includedgroup"></a><span data-ttu-id="a738d-103">Excluir includedGroup</span><span class="sxs-lookup"><span data-stu-id="a738d-103">Delete includedGroup</span></span>

<span data-ttu-id="a738d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a738d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a738d-105">Exclua um grupo da lista de grupos incluídos em uma política de gerenciamento de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="a738d-105">Delete a group from the list of groups included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="a738d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a738d-106">Permissions</span></span>

<span data-ttu-id="a738d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a738d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a738d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a738d-109">Permission type</span></span>|<span data-ttu-id="a738d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a738d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a738d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a738d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a738d-112">Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="a738d-112">Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="a738d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a738d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a738d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a738d-114">Not supported.</span></span>|
|<span data-ttu-id="a738d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a738d-115">Application</span></span> | <span data-ttu-id="a738d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a738d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a738d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a738d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileAppManagementPolicies/{id}/includedGroups/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a738d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a738d-118">Request headers</span></span>

|<span data-ttu-id="a738d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a738d-119">Name</span></span>|<span data-ttu-id="a738d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a738d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a738d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a738d-121">Authorization</span></span>|<span data-ttu-id="a738d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a738d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a738d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a738d-124">Request body</span></span>

<span data-ttu-id="a738d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a738d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a738d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a738d-126">Response</span></span>

<span data-ttu-id="a738d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a738d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a738d-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a738d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a738d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a738d-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a738d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="a738d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group"
}
-->

```http
DELETE https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/1a9db3ab-0acf-4808-99ae-e8ed581cb2e0/$ref
```
# <a name="c"></a>[<span data-ttu-id="a738d-132">C#</span><span class="sxs-lookup"><span data-stu-id="a738d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a738d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a738d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a738d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a738d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a738d-135">Java</span><span class="sxs-lookup"><span data-stu-id="a738d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a738d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a738d-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
