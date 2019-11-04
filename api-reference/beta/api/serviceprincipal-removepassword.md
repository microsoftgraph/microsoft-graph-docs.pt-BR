---
title: 'servicePrincipalName: removePassword'
description: Remover uma senha de um servicePrincipalName
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 61700e51ccc1cafd1b6d696840dfd068b632c5a5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938376"
---
# <a name="serviceprincipal-removepassword"></a><span data-ttu-id="b684e-103">servicePrincipalName: removePassword</span><span class="sxs-lookup"><span data-stu-id="b684e-103">servicePrincipal: removePassword</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b684e-104">Remover uma senha de um objeto do [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="b684e-104">Remove a password from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b684e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b684e-105">Permissions</span></span>

<span data-ttu-id="b684e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b684e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b684e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b684e-108">Permission type</span></span>                        | <span data-ttu-id="b684e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b684e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b684e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b684e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b684e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b684e-111">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="b684e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b684e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b684e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b684e-113">Not supported.</span></span> |
| <span data-ttu-id="b684e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b684e-114">Application</span></span>                            | <span data-ttu-id="b684e-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b684e-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b684e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b684e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="b684e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b684e-117">Request headers</span></span>

| <span data-ttu-id="b684e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b684e-118">Name</span></span>           | <span data-ttu-id="b684e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b684e-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="b684e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b684e-120">Authorization</span></span>  | <span data-ttu-id="b684e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b684e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b684e-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="b684e-123">Content-type</span></span>   | <span data-ttu-id="b684e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b684e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b684e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b684e-126">Request body</span></span>

| <span data-ttu-id="b684e-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b684e-127">Property</span></span>     | <span data-ttu-id="b684e-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b684e-128">Type</span></span>   |<span data-ttu-id="b684e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b684e-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b684e-130">keyId</span><span class="sxs-lookup"><span data-stu-id="b684e-130">keyId</span></span> | <span data-ttu-id="b684e-131">GUID</span><span class="sxs-lookup"><span data-stu-id="b684e-131">GUID</span></span> | <span data-ttu-id="b684e-132">O identificador exclusivo da senha.</span><span class="sxs-lookup"><span data-stu-id="b684e-132">The unique identifier for the password.</span></span> <span data-ttu-id="b684e-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b684e-133">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b684e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b684e-134">Response</span></span>

<span data-ttu-id="b684e-135">Se tiver êxito, este método retornará um código de resposta `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="b684e-135">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b684e-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b684e-136">Examples</span></span>

<span data-ttu-id="b684e-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b684e-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b684e-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b684e-138">Request</span></span>

<span data-ttu-id="b684e-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b684e-139">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b684e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b684e-140">Response</span></span>

<span data-ttu-id="b684e-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b684e-141">The following is an example of the response.</span></span>

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
