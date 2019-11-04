---
title: 'aplicativo: removePassword'
description: Remover uma senha de um aplicativo
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7cee2e459fdc9ff844688228233881f257239b0f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935071"
---
# <a name="application-removepassword"></a><span data-ttu-id="5553c-103">aplicativo: removePassword</span><span class="sxs-lookup"><span data-stu-id="5553c-103">application: removePassword</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5553c-104">Remove uma senha de um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="5553c-104">Removes a password from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5553c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5553c-105">Permissions</span></span>

<span data-ttu-id="5553c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5553c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5553c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5553c-108">Permission type</span></span>                        | <span data-ttu-id="5553c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5553c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5553c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5553c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5553c-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5553c-111">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="5553c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5553c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5553c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5553c-113">Not supported.</span></span> |
| <span data-ttu-id="5553c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5553c-114">Application</span></span>                            | <span data-ttu-id="5553c-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5553c-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5553c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5553c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="5553c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5553c-117">Request headers</span></span>

| <span data-ttu-id="5553c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5553c-118">Name</span></span>           | <span data-ttu-id="5553c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5553c-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="5553c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5553c-120">Authorization</span></span>  | <span data-ttu-id="5553c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5553c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5553c-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="5553c-123">Content-type</span></span>   | <span data-ttu-id="5553c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5553c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5553c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5553c-126">Request body</span></span>

| <span data-ttu-id="5553c-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5553c-127">Property</span></span>  | <span data-ttu-id="5553c-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="5553c-128">Type</span></span> | <span data-ttu-id="5553c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="5553c-129">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="5553c-130">keyId</span><span class="sxs-lookup"><span data-stu-id="5553c-130">keyId</span></span>     | <span data-ttu-id="5553c-131">GUID</span><span class="sxs-lookup"><span data-stu-id="5553c-131">GUID</span></span> | <span data-ttu-id="5553c-132">O identificador exclusivo da senha.</span><span class="sxs-lookup"><span data-stu-id="5553c-132">The unique identifier for the password.</span></span> <span data-ttu-id="5553c-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5553c-133">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5553c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5553c-134">Response</span></span>

<span data-ttu-id="5553c-135">Se tiver êxito, este método retornará um código de resposta `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="5553c-135">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5553c-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5553c-136">Examples</span></span>

<span data-ttu-id="5553c-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5553c-137">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5553c-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5553c-138">Request</span></span>

<span data-ttu-id="5553c-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5553c-139">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5553c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5553c-140">Response</span></span>

<span data-ttu-id="5553c-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5553c-141">The following is an example of the response.</span></span>

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
