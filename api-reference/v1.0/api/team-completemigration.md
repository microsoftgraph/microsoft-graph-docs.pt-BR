---
title: 'team: completeMigration'
description: Conclua a migração de mensagens externas removendo o modo de migração de uma equipe.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3faec85b08d8d0ed340f29985574d05a804c061f
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507911"
---
# <a name="team-completemigration"></a><span data-ttu-id="fe597-103">team: completeMigration</span><span class="sxs-lookup"><span data-stu-id="fe597-103">team: completeMigration</span></span>

<span data-ttu-id="fe597-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe597-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe597-105">Conclua o processo de migração de mensagens removendo `migration mode` de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="fe597-105">Complete the message migration process by removing `migration mode` from a [team](../resources/team.md).</span></span> <span data-ttu-id="fe597-106">`Migration mode` é um estado especial em que determinadas operações são barradas, como as operações postagem de mensagem e associação durante o processo de migração de dados.</span><span class="sxs-lookup"><span data-stu-id="fe597-106">`Migration mode` is a special state where certain operations are barred, like message POST and membership operations during the data migration process.</span></span>

<span data-ttu-id="fe597-107">Depois que **uma solicitação completeMigration** for feita, você não poderá importar mensagens adicionais para a equipe.</span><span class="sxs-lookup"><span data-stu-id="fe597-107">After a **completeMigration** request is made, you cannot import additional messages into the team.</span></span> <span data-ttu-id="fe597-108">Você pode adicionar membros à equipe após a solicitação retornar uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="fe597-108">You can add members to the team after the request returns a successful response.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe597-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe597-109">Permissions</span></span>

<span data-ttu-id="fe597-110">A permissão a seguir é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="fe597-110">The following permission is required to call this API.</span></span> <span data-ttu-id="fe597-111">Para saber mais, confira [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe597-111">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe597-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe597-112">Permission type</span></span>      | <span data-ttu-id="fe597-113">Permissão</span><span class="sxs-lookup"><span data-stu-id="fe597-113">Permission</span></span>  |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="fe597-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe597-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="fe597-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe597-115">Not supported.</span></span>|
| <span data-ttu-id="fe597-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe597-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe597-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe597-117">Not supported.</span></span> |
|<span data-ttu-id="fe597-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe597-118">Application</span></span> | <span data-ttu-id="fe597-119">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="fe597-119">Teamwork.Migrate.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe597-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe597-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/completeMigration
```

## <a name="request-headers"></a><span data-ttu-id="fe597-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe597-121">Request headers</span></span>

| <span data-ttu-id="fe597-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe597-122">Header</span></span>       | <span data-ttu-id="fe597-123">Valor</span><span class="sxs-lookup"><span data-stu-id="fe597-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fe597-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe597-124">Authorization</span></span>  | <span data-ttu-id="fe597-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe597-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe597-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe597-127">Request body</span></span>

<span data-ttu-id="fe597-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe597-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe597-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe597-129">Response</span></span>

<span data-ttu-id="fe597-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe597-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe597-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe597-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe597-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe597-133">Request</span></span>

<span data-ttu-id="fe597-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe597-134">The following is an example of the request.</span></span>
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->



# <a name="http"></a>[<span data-ttu-id="fe597-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe597-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "completeMigration_team"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/completeMigration
```
# <a name="c"></a>[<span data-ttu-id="fe597-136">C#</span><span class="sxs-lookup"><span data-stu-id="fe597-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/completemigration-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe597-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe597-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/completemigration-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe597-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe597-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/completemigration-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe597-139">Java</span><span class="sxs-lookup"><span data-stu-id="fe597-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/completemigration-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="fe597-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe597-140">Response</span></span>

<span data-ttu-id="fe597-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fe597-141">The following is an example of the response.</span></span>
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
