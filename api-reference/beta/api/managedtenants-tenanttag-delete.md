---
title: Excluir tenantTag
description: Exclui um objeto tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 6bfecf4ff74b3e942536a07ca3dda129b44e86b3
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441095"
---
# <a name="delete-tenanttag"></a><span data-ttu-id="22138-103">Excluir tenantTag</span><span class="sxs-lookup"><span data-stu-id="22138-103">Delete tenantTag</span></span>
<span data-ttu-id="22138-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="22138-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22138-105">Exclui um [objeto tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="22138-105">Deletes a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22138-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="22138-106">Permissions</span></span>
<span data-ttu-id="22138-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22138-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22138-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22138-109">Permission type</span></span>|<span data-ttu-id="22138-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22138-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22138-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22138-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22138-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="22138-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="22138-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22138-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22138-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22138-114">Not supported.</span></span>|
|<span data-ttu-id="22138-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22138-115">Application</span></span>|<span data-ttu-id="22138-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22138-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22138-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22138-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="request-headers"></a><span data-ttu-id="22138-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22138-118">Request headers</span></span>
|<span data-ttu-id="22138-119">Nome</span><span class="sxs-lookup"><span data-stu-id="22138-119">Name</span></span>|<span data-ttu-id="22138-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="22138-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="22138-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="22138-121">Authorization</span></span>|<span data-ttu-id="22138-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22138-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22138-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22138-124">Request body</span></span>
<span data-ttu-id="22138-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22138-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22138-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="22138-126">Response</span></span>

<span data-ttu-id="22138-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="22138-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="22138-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="22138-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22138-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22138-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="22138-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="22138-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tenanttag"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```
# <a name="c"></a>[<span data-ttu-id="22138-131">C#</span><span class="sxs-lookup"><span data-stu-id="22138-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tenanttag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22138-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22138-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tenanttag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22138-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22138-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tenanttag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22138-134">Java</span><span class="sxs-lookup"><span data-stu-id="22138-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tenanttag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="22138-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="22138-135">Response</span></span>
><span data-ttu-id="22138-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="22138-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
