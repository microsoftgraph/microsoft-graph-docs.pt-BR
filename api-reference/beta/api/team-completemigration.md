---
title: 'equipe: completeMigration'
description: Concluir a migração de mensagens externas, removendo o modo de migração de uma equipe.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0a3f26727e3e084b3fb0bb95467ffae61f6190a0
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48783023"
---
# <a name="team-completemigration"></a><span data-ttu-id="4c58b-103">equipe: completeMigration</span><span class="sxs-lookup"><span data-stu-id="4c58b-103">team: completeMigration</span></span>

<span data-ttu-id="4c58b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c58b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c58b-105">Conclua o processo de migração de mensagens removendo `migration mode` de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="4c58b-105">Complete the message migration process by removing `migration mode` from a [team](../resources/team.md).</span></span> <span data-ttu-id="4c58b-106">`Migration mode` é um estado especial em que determinadas operações são bloqueadas, como a POSTAgem de mensagens e operações de associação durante o processo de migração de dados.</span><span class="sxs-lookup"><span data-stu-id="4c58b-106">`Migration mode` is a special state where certain operations are barred, like message POST and membership operations during the data migration process.</span></span>

<span data-ttu-id="4c58b-107">Depois que uma solicitação **completeMigration** é feita, não é possível importar mensagens adicionais para a equipe.</span><span class="sxs-lookup"><span data-stu-id="4c58b-107">After a **completeMigration** request is made, you cannot import additional messages into the team.</span></span> <span data-ttu-id="4c58b-108">Você pode adicionar membros à equipe depois que a solicitação retornar uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="4c58b-108">You can add members to the team after the request returns a successful response.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c58b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c58b-109">Permissions</span></span>

<span data-ttu-id="4c58b-110">A seguinte permissão é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4c58b-110">The following permission is required to call this API.</span></span> <span data-ttu-id="4c58b-111">Para saber mais, confira [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c58b-111">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c58b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c58b-112">Permission type</span></span>      | <span data-ttu-id="4c58b-113">Permissão</span><span class="sxs-lookup"><span data-stu-id="4c58b-113">Permission</span></span>  |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="4c58b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c58b-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="4c58b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c58b-115">Not supported.</span></span>|
| <span data-ttu-id="4c58b-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c58b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c58b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c58b-117">Not supported.</span></span> |
|<span data-ttu-id="4c58b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c58b-118">Application</span></span> | <span data-ttu-id="4c58b-119">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="4c58b-119">Teamwork.Migrate.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c58b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c58b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{teamId}/completeMigration
```

## <a name="request-headers"></a><span data-ttu-id="4c58b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c58b-121">Request headers</span></span>

| <span data-ttu-id="4c58b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c58b-122">Header</span></span>       | <span data-ttu-id="4c58b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4c58b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4c58b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c58b-124">Authorization</span></span>  | <span data-ttu-id="4c58b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c58b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4c58b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c58b-127">Request body</span></span>

<span data-ttu-id="4c58b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c58b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c58b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c58b-129">Response</span></span>

<span data-ttu-id="4c58b-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c58b-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c58b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c58b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c58b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c58b-133">Request</span></span>

<span data-ttu-id="4c58b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c58b-134">The following is an example of the request.</span></span>
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->

<!-- {
  "blockType": "request",
  "name": "completeMigration_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/completeMigration
```
<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="4c58b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c58b-135">Response</span></span>

<span data-ttu-id="4c58b-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c58b-136">The following is an example of the response.</span></span>
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
