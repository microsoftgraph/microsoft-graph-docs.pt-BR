---
title: 'aplicativo: removePassword'
description: Remover uma senha de um aplicativo
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d09b98c8fbf3a9367ecd2c1f64b6a544c9baa7d5
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192411"
---
# <a name="application-removepassword"></a><span data-ttu-id="c6108-103">aplicativo: removePassword</span><span class="sxs-lookup"><span data-stu-id="c6108-103">application: removePassword</span></span>

<span data-ttu-id="c6108-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6108-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6108-105">Remove uma senha de um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="c6108-105">Removes a password from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c6108-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6108-106">Permissions</span></span>

<span data-ttu-id="c6108-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6108-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c6108-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6108-109">Permission type</span></span>                        | <span data-ttu-id="c6108-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6108-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c6108-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6108-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6108-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c6108-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="c6108-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6108-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6108-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6108-114">Application.ReadWrite.All</span></span> |
| <span data-ttu-id="c6108-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6108-115">Application</span></span>                            | <span data-ttu-id="c6108-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6108-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6108-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6108-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="c6108-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6108-118">Request headers</span></span>

| <span data-ttu-id="c6108-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c6108-119">Name</span></span>           | <span data-ttu-id="c6108-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6108-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="c6108-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6108-121">Authorization</span></span>  | <span data-ttu-id="c6108-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6108-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c6108-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6108-124">Content-Type</span></span>   | <span data-ttu-id="c6108-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6108-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6108-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6108-127">Request body</span></span>

| <span data-ttu-id="c6108-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6108-128">Property</span></span>  | <span data-ttu-id="c6108-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6108-129">Type</span></span> | <span data-ttu-id="c6108-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6108-130">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="c6108-131">keyId</span><span class="sxs-lookup"><span data-stu-id="c6108-131">keyId</span></span>     | <span data-ttu-id="c6108-132">GUID</span><span class="sxs-lookup"><span data-stu-id="c6108-132">GUID</span></span> | <span data-ttu-id="c6108-133">O identificador exclusivo da senha.</span><span class="sxs-lookup"><span data-stu-id="c6108-133">The unique identifier for the password.</span></span> <span data-ttu-id="c6108-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6108-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c6108-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6108-135">Response</span></span>

<span data-ttu-id="c6108-136">Se tiver êxito, este método retornará um código de resposta `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="c6108-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c6108-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c6108-137">Examples</span></span>

<span data-ttu-id="c6108-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="c6108-138">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c6108-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6108-139">Request</span></span>

<span data-ttu-id="c6108-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6108-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c6108-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6108-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c6108-142">C#</span><span class="sxs-lookup"><span data-stu-id="c6108-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6108-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6108-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6108-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6108-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c6108-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6108-145">Response</span></span>

<span data-ttu-id="c6108-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c6108-146">The following is an example of the response.</span></span>

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


