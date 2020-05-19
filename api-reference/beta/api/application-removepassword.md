---
title: 'aplicativo: removePassword'
description: Remover uma senha de um aplicativo
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a98f932150532e4ee844b1cc243e068157e32585
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289128"
---
# <a name="application-removepassword"></a><span data-ttu-id="ee643-103">aplicativo: removePassword</span><span class="sxs-lookup"><span data-stu-id="ee643-103">application: removePassword</span></span>

<span data-ttu-id="ee643-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee643-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee643-105">Remove uma senha de um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="ee643-105">Removes a password from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ee643-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee643-106">Permissions</span></span>

<span data-ttu-id="ee643-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee643-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee643-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee643-109">Permission type</span></span>                        | <span data-ttu-id="ee643-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee643-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ee643-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee643-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee643-112">Application. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="ee643-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="ee643-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee643-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee643-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee643-114">Not supported.</span></span> |
| <span data-ttu-id="ee643-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee643-115">Application</span></span>                            | <span data-ttu-id="ee643-116">Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ee643-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee643-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee643-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="ee643-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee643-118">Request headers</span></span>

| <span data-ttu-id="ee643-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ee643-119">Name</span></span>           | <span data-ttu-id="ee643-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee643-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="ee643-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee643-121">Authorization</span></span>  | <span data-ttu-id="ee643-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee643-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ee643-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee643-124">Content-Type</span></span>   | <span data-ttu-id="ee643-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee643-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee643-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee643-127">Request body</span></span>

| <span data-ttu-id="ee643-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee643-128">Property</span></span>  | <span data-ttu-id="ee643-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee643-129">Type</span></span> | <span data-ttu-id="ee643-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee643-130">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="ee643-131">keyId</span><span class="sxs-lookup"><span data-stu-id="ee643-131">keyId</span></span>     | <span data-ttu-id="ee643-132">GUID</span><span class="sxs-lookup"><span data-stu-id="ee643-132">GUID</span></span> | <span data-ttu-id="ee643-133">O identificador exclusivo da senha.</span><span class="sxs-lookup"><span data-stu-id="ee643-133">The unique identifier for the password.</span></span> <span data-ttu-id="ee643-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee643-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ee643-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee643-135">Response</span></span>

<span data-ttu-id="ee643-136">Se tiver êxito, este método retornará um código de resposta `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="ee643-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ee643-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ee643-137">Examples</span></span>

<span data-ttu-id="ee643-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="ee643-138">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ee643-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee643-139">Request</span></span>

<span data-ttu-id="ee643-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee643-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ee643-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee643-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ee643-142">C#</span><span class="sxs-lookup"><span data-stu-id="ee643-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee643-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee643-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee643-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee643-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ee643-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee643-145">Response</span></span>

<span data-ttu-id="ee643-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ee643-146">The following is an example of the response.</span></span>

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
