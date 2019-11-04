---
title: Criar personWebsite
description: Criar um novo personWebsite.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5fb4d4a427229c0bf727596b46520cf767cbd29f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937641"
---
# <a name="create-personwebsite"></a><span data-ttu-id="7febf-103">Criar personWebsite</span><span class="sxs-lookup"><span data-stu-id="7febf-103">Create personWebsite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7febf-104">Criar um novo objeto [personWebsite](../resources/personwebsite.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7febf-104">Create a new [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7febf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7febf-105">Permissions</span></span>

<span data-ttu-id="7febf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7febf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7febf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7febf-108">Permission type</span></span>                        | <span data-ttu-id="7febf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7febf-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7febf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7febf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7febf-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7febf-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="7febf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7febf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7febf-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7febf-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="7febf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7febf-114">Application</span></span>                            | <span data-ttu-id="7febf-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7febf-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7febf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7febf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/websites
```

## <a name="request-headers"></a><span data-ttu-id="7febf-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7febf-117">Request headers</span></span>

| <span data-ttu-id="7febf-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7febf-118">Name</span></span>      |<span data-ttu-id="7febf-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7febf-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7febf-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7febf-120">Authorization</span></span>  | <span data-ttu-id="7febf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7febf-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="7febf-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7febf-123">Content-Type</span></span>   | <span data-ttu-id="7febf-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7febf-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7febf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7febf-126">Request body</span></span>

<span data-ttu-id="7febf-127">No corpo da solicitação, forneça uma representação JSON do objeto [personWebsite](../resources/personwebsite.md) .</span><span class="sxs-lookup"><span data-stu-id="7febf-127">In the request body, supply a JSON representation of [personWebsite](../resources/personwebsite.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7febf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7febf-128">Response</span></span>

<span data-ttu-id="7febf-129">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [personWebsite](../resources/personwebsite.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7febf-129">If successful, this method returns `201, Created` response code and a new [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7febf-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7febf-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7febf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7febf-131">Request</span></span>

<span data-ttu-id="7febf-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7febf-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_personwebsite_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/websites
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

### <a name="response"></a><span data-ttu-id="7febf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7febf-133">Response</span></span>

<span data-ttu-id="7febf-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7febf-134">The following is an example of the response.</span></span>

> <span data-ttu-id="7febf-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7febf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personWebsite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
