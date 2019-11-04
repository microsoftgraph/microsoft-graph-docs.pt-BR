---
title: Criar personAnniversary
description: Use esta API para criar um novo personAnniversary.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e6e73919913f710bee6721ec1710847cc742ba4d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937718"
---
# <a name="create-personanniversary"></a><span data-ttu-id="e7334-103">Criar personAnniversary</span><span class="sxs-lookup"><span data-stu-id="e7334-103">Create personAnniversary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7334-104">Use esta API para criar um novo objeto [personAnniversary](../resources/personanniversary.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e7334-104">Use this API to create a new [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e7334-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7334-105">Permissions</span></span>

<span data-ttu-id="e7334-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7334-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e7334-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7334-108">Permission type</span></span>                        | <span data-ttu-id="e7334-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7334-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e7334-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7334-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e7334-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e7334-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e7334-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7334-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7334-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e7334-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e7334-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7334-114">Application</span></span>                            | <span data-ttu-id="e7334-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7334-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e7334-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7334-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/anniversaries 
```

## <a name="request-headers"></a><span data-ttu-id="e7334-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7334-117">Request headers</span></span>

| <span data-ttu-id="e7334-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e7334-118">Name</span></span>      |<span data-ttu-id="e7334-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7334-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e7334-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7334-120">Authorization</span></span>  | <span data-ttu-id="e7334-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7334-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e7334-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e7334-123">Content-Type</span></span>   | <span data-ttu-id="e7334-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7334-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7334-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7334-126">Request body</span></span>

<span data-ttu-id="e7334-127">No corpo da solicitação, forneça uma representação JSON do objeto [personAnniversary](../resources/personanniversary.md) .</span><span class="sxs-lookup"><span data-stu-id="e7334-127">In the request body, supply a JSON representation of [personAnniversary](../resources/personanniversary.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e7334-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7334-128">Response</span></span>

<span data-ttu-id="e7334-129">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [personAnniversary](../resources/personanniversary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7334-129">If successful, this method returns `201, Created` response code and a new [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e7334-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e7334-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e7334-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7334-131">Request</span></span>

<span data-ttu-id="e7334-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7334-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_personanniversary_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/anniversaries
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```

### <a name="response"></a><span data-ttu-id="e7334-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7334-133">Response</span></span>

<span data-ttu-id="e7334-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7334-134">The following is an example of the response.</span></span>

> <span data-ttu-id="e7334-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7334-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personAnniversary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->