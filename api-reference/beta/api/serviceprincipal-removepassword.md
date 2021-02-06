---
title: 'servicePrincipal: removePassword'
description: Remover uma senha de uma servicePrincipal
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: be45dacbb123c93d7670d3f01f9b7444e561300a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134096"
---
# <a name="serviceprincipal-removepassword"></a><span data-ttu-id="f83ce-103">servicePrincipal: removePassword</span><span class="sxs-lookup"><span data-stu-id="f83ce-103">servicePrincipal: removePassword</span></span>

<span data-ttu-id="f83ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f83ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f83ce-105">Remover uma senha de um [objeto servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="f83ce-105">Remove a password from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f83ce-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f83ce-106">Permissions</span></span>

<span data-ttu-id="f83ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f83ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f83ce-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f83ce-109">Permission type</span></span>                        | <span data-ttu-id="f83ce-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f83ce-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f83ce-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f83ce-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f83ce-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f83ce-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="f83ce-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f83ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f83ce-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f83ce-114">Not supported.</span></span> |
| <span data-ttu-id="f83ce-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f83ce-115">Application</span></span>                            | <span data-ttu-id="f83ce-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f83ce-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f83ce-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f83ce-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="f83ce-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f83ce-118">Request headers</span></span>

| <span data-ttu-id="f83ce-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f83ce-119">Name</span></span>           | <span data-ttu-id="f83ce-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f83ce-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f83ce-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f83ce-121">Authorization</span></span>  | <span data-ttu-id="f83ce-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f83ce-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f83ce-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="f83ce-124">Content-type</span></span>   | <span data-ttu-id="f83ce-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f83ce-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f83ce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f83ce-127">Request body</span></span>

| <span data-ttu-id="f83ce-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f83ce-128">Property</span></span>     | <span data-ttu-id="f83ce-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f83ce-129">Type</span></span>   |<span data-ttu-id="f83ce-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f83ce-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f83ce-131">keyId</span><span class="sxs-lookup"><span data-stu-id="f83ce-131">keyId</span></span> | <span data-ttu-id="f83ce-132">GUID</span><span class="sxs-lookup"><span data-stu-id="f83ce-132">GUID</span></span> | <span data-ttu-id="f83ce-133">O identificador exclusivo da senha.</span><span class="sxs-lookup"><span data-stu-id="f83ce-133">The unique identifier for the password.</span></span> <span data-ttu-id="f83ce-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f83ce-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f83ce-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f83ce-135">Response</span></span>

<span data-ttu-id="f83ce-136">Se tiver êxito, este método retornará um código de resposta `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="f83ce-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f83ce-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f83ce-137">Examples</span></span>

<span data-ttu-id="f83ce-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f83ce-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f83ce-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f83ce-139">Request</span></span>

<span data-ttu-id="f83ce-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f83ce-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f83ce-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="f83ce-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_removepassword"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```
# <a name="javascript"></a>[<span data-ttu-id="f83ce-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f83ce-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f83ce-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f83ce-143">Response</span></span>

<span data-ttu-id="f83ce-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f83ce-144">The following is an example of the response.</span></span>

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
  "description": "servicePrincipal: removePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



