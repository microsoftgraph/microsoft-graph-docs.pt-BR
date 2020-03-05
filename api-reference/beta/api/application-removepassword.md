---
title: 'aplicativo: removePassword'
description: Remover uma senha de um aplicativo
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bac7ed6bd5ee15cd917c8467d3b12ef696bbdf51
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441442"
---
# <a name="application-removepassword"></a><span data-ttu-id="a1d23-103">aplicativo: removePassword</span><span class="sxs-lookup"><span data-stu-id="a1d23-103">application: removePassword</span></span>

<span data-ttu-id="a1d23-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a1d23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1d23-105">Remove uma senha de um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="a1d23-105">Removes a password from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a1d23-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1d23-106">Permissions</span></span>

<span data-ttu-id="a1d23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1d23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1d23-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1d23-109">Permission type</span></span>                        | <span data-ttu-id="a1d23-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1d23-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a1d23-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1d23-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1d23-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a1d23-112">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="a1d23-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1d23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1d23-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1d23-114">Not supported.</span></span> |
| <span data-ttu-id="a1d23-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1d23-115">Application</span></span>                            | <span data-ttu-id="a1d23-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1d23-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1d23-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1d23-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="a1d23-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d23-118">Request headers</span></span>

| <span data-ttu-id="a1d23-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a1d23-119">Name</span></span>           | <span data-ttu-id="a1d23-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1d23-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="a1d23-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1d23-121">Authorization</span></span>  | <span data-ttu-id="a1d23-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1d23-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a1d23-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="a1d23-124">Content-type</span></span>   | <span data-ttu-id="a1d23-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1d23-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1d23-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d23-127">Request body</span></span>

| <span data-ttu-id="a1d23-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1d23-128">Property</span></span>  | <span data-ttu-id="a1d23-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1d23-129">Type</span></span> | <span data-ttu-id="a1d23-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1d23-130">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="a1d23-131">keyId</span><span class="sxs-lookup"><span data-stu-id="a1d23-131">keyId</span></span>     | <span data-ttu-id="a1d23-132">GUID</span><span class="sxs-lookup"><span data-stu-id="a1d23-132">GUID</span></span> | <span data-ttu-id="a1d23-133">O identificador exclusivo da senha.</span><span class="sxs-lookup"><span data-stu-id="a1d23-133">The unique identifier for the password.</span></span> <span data-ttu-id="a1d23-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1d23-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a1d23-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1d23-135">Response</span></span>

<span data-ttu-id="a1d23-136">Se tiver êxito, este método retornará um código de resposta `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="a1d23-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a1d23-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a1d23-137">Examples</span></span>

<span data-ttu-id="a1d23-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a1d23-138">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a1d23-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d23-139">Request</span></span>

<span data-ttu-id="a1d23-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1d23-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1d23-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1d23-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_removepassword"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```
# <a name="c"></a>[<span data-ttu-id="a1d23-142">C#</span><span class="sxs-lookup"><span data-stu-id="a1d23-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1d23-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1d23-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1d23-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1d23-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a1d23-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1d23-145">Response</span></span>

<span data-ttu-id="a1d23-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1d23-146">The following is an example of the response.</span></span>

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
