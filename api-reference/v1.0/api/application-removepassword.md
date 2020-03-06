---
title: 'aplicativo: removePassword'
description: Remover uma senha de um aplicativo
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fe5f330bc73c7ad10cceb074b299ed08e99ed476
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518851"
---
# <a name="application-removepassword"></a><span data-ttu-id="29753-103">aplicativo: removePassword</span><span class="sxs-lookup"><span data-stu-id="29753-103">application: removePassword</span></span>

<span data-ttu-id="29753-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29753-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="29753-105">Remover uma senha de um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="29753-105">Remove a password from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="29753-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="29753-106">Permissions</span></span>

<span data-ttu-id="29753-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29753-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29753-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29753-109">Permission type</span></span>                        | <span data-ttu-id="29753-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29753-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="29753-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29753-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="29753-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29753-112">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="29753-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29753-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29753-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29753-114">Not supported.</span></span> |
| <span data-ttu-id="29753-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29753-115">Application</span></span>                            | <span data-ttu-id="29753-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29753-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29753-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29753-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="29753-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29753-118">Request headers</span></span>

| <span data-ttu-id="29753-119">Nome</span><span class="sxs-lookup"><span data-stu-id="29753-119">Name</span></span>           | <span data-ttu-id="29753-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="29753-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="29753-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="29753-121">Authorization</span></span>  | <span data-ttu-id="29753-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29753-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="29753-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="29753-124">Content-type</span></span>   | <span data-ttu-id="29753-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29753-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29753-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29753-127">Request body</span></span>

| <span data-ttu-id="29753-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29753-128">Property</span></span>  | <span data-ttu-id="29753-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="29753-129">Type</span></span> | <span data-ttu-id="29753-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="29753-130">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="29753-131">keyId</span><span class="sxs-lookup"><span data-stu-id="29753-131">keyId</span></span>     | <span data-ttu-id="29753-132">GUID</span><span class="sxs-lookup"><span data-stu-id="29753-132">GUID</span></span> | <span data-ttu-id="29753-133">O identificador exclusivo da senha.</span><span class="sxs-lookup"><span data-stu-id="29753-133">The unique identifier for the password.</span></span> <span data-ttu-id="29753-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29753-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="29753-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="29753-135">Response</span></span>

<span data-ttu-id="29753-136">Se tiver êxito, este método retornará um código de resposta `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="29753-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="29753-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="29753-137">Examples</span></span>

<span data-ttu-id="29753-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="29753-138">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="29753-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29753-139">Request</span></span>

<span data-ttu-id="29753-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="29753-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="29753-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="29753-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_removepassword"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```
# <a name="c"></a>[<span data-ttu-id="29753-142">C#</span><span class="sxs-lookup"><span data-stu-id="29753-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29753-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29753-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29753-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29753-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29753-145">Java</span><span class="sxs-lookup"><span data-stu-id="29753-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-removepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="29753-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="29753-146">Response</span></span>

<span data-ttu-id="29753-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="29753-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordCredential"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: removePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
