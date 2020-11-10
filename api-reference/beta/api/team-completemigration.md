---
title: 'equipe: completeMigration'
description: Concluir a migração de mensagens externas, removendo o modo de migração de uma equipe.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3422c67c34c62fd037b2acf214c4664b21f83900
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951483"
---
# <a name="team-completemigration"></a><span data-ttu-id="31e7f-103">equipe: completeMigration</span><span class="sxs-lookup"><span data-stu-id="31e7f-103">team: completeMigration</span></span>

<span data-ttu-id="31e7f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31e7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31e7f-105">Conclua o processo de migração de mensagens removendo `migration mode` de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="31e7f-105">Complete the message migration process by removing `migration mode` from a [team](../resources/team.md).</span></span> <span data-ttu-id="31e7f-106">`Migration mode` é um estado especial em que determinadas operações são bloqueadas, como a POSTAgem de mensagens e operações de associação durante o processo de migração de dados.</span><span class="sxs-lookup"><span data-stu-id="31e7f-106">`Migration mode` is a special state where certain operations are barred, like message POST and membership operations during the data migration process.</span></span>

<span data-ttu-id="31e7f-107">Depois que uma solicitação **completeMigration** é feita, não é possível importar mensagens adicionais para a equipe.</span><span class="sxs-lookup"><span data-stu-id="31e7f-107">After a **completeMigration** request is made, you cannot import additional messages into the team.</span></span> <span data-ttu-id="31e7f-108">Você pode adicionar membros à equipe depois que a solicitação retornar uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="31e7f-108">You can add members to the team after the request returns a successful response.</span></span>

## <a name="permissions"></a><span data-ttu-id="31e7f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="31e7f-109">Permissions</span></span>

<span data-ttu-id="31e7f-110">A seguinte permissão é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="31e7f-110">The following permission is required to call this API.</span></span> <span data-ttu-id="31e7f-111">Para saber mais, confira [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31e7f-111">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31e7f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31e7f-112">Permission type</span></span>      | <span data-ttu-id="31e7f-113">Permissão</span><span class="sxs-lookup"><span data-stu-id="31e7f-113">Permission</span></span>  |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="31e7f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31e7f-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="31e7f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31e7f-115">Not supported.</span></span>|
| <span data-ttu-id="31e7f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31e7f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31e7f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31e7f-117">Not supported.</span></span> |
|<span data-ttu-id="31e7f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31e7f-118">Application</span></span> | <span data-ttu-id="31e7f-119">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="31e7f-119">Teamwork.Migrate.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31e7f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31e7f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{teamId}/completeMigration
```

## <a name="request-headers"></a><span data-ttu-id="31e7f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31e7f-121">Request headers</span></span>

| <span data-ttu-id="31e7f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31e7f-122">Header</span></span>       | <span data-ttu-id="31e7f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="31e7f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="31e7f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="31e7f-124">Authorization</span></span>  | <span data-ttu-id="31e7f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31e7f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="31e7f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31e7f-127">Request body</span></span>

<span data-ttu-id="31e7f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31e7f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31e7f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="31e7f-129">Response</span></span>

<span data-ttu-id="31e7f-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31e7f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31e7f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31e7f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="31e7f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31e7f-133">Request</span></span>

<span data-ttu-id="31e7f-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="31e7f-134">The following is an example of the request.</span></span>
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->


# <a name="http"></a>[<span data-ttu-id="31e7f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="31e7f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "completeMigration_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/completeMigration
```
# <a name="c"></a>[<span data-ttu-id="31e7f-136">C#</span><span class="sxs-lookup"><span data-stu-id="31e7f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/completemigration-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31e7f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31e7f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/completemigration-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31e7f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31e7f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/completemigration-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31e7f-139">Java</span><span class="sxs-lookup"><span data-stu-id="31e7f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/completemigration-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="31e7f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="31e7f-140">Response</span></span>

<span data-ttu-id="31e7f-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="31e7f-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: d945a9a4-0e5b-11eb-adc1-0242ac120002
2020-10-14 20:22:11 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "completeMigration_ team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
