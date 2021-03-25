---
title: 'team: completeMigration'
description: Conclua a migração de mensagens externas removendo o modo de migração de uma equipe.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6edd393475eecba7da736fe0c72571ffc244b73e
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200755"
---
# <a name="team-completemigration"></a><span data-ttu-id="732be-103">team: completeMigration</span><span class="sxs-lookup"><span data-stu-id="732be-103">team: completeMigration</span></span>

<span data-ttu-id="732be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="732be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="732be-105">Conclua o processo de migração de mensagens removendo `migration mode` de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="732be-105">Complete the message migration process by removing `migration mode` from a [team](../resources/team.md).</span></span> <span data-ttu-id="732be-106">`Migration mode` é um estado especial em que determinadas operações são barradas, como as operações postagem de mensagem e associação durante o processo de migração de dados.</span><span class="sxs-lookup"><span data-stu-id="732be-106">`Migration mode` is a special state where certain operations are barred, like message POST and membership operations during the data migration process.</span></span>

<span data-ttu-id="732be-107">Depois que **uma solicitação completeMigration** for feita, você não poderá importar mensagens adicionais para a equipe.</span><span class="sxs-lookup"><span data-stu-id="732be-107">After a **completeMigration** request is made, you cannot import additional messages into the team.</span></span> <span data-ttu-id="732be-108">Você pode adicionar membros à equipe após a solicitação retornar uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="732be-108">You can add members to the team after the request returns a successful response.</span></span>

## <a name="permissions"></a><span data-ttu-id="732be-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="732be-109">Permissions</span></span>

<span data-ttu-id="732be-110">A permissão a seguir é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="732be-110">The following permission is required to call this API.</span></span> <span data-ttu-id="732be-111">Para saber mais, confira [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="732be-111">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="732be-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="732be-112">Permission type</span></span>      | <span data-ttu-id="732be-113">Permissão</span><span class="sxs-lookup"><span data-stu-id="732be-113">Permission</span></span>  |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="732be-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="732be-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="732be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="732be-115">Not supported.</span></span>|
| <span data-ttu-id="732be-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="732be-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="732be-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="732be-117">Not supported.</span></span> |
|<span data-ttu-id="732be-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="732be-118">Application</span></span> | <span data-ttu-id="732be-119">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="732be-119">Teamwork.Migrate.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="732be-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="732be-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/completeMigration
```

## <a name="request-headers"></a><span data-ttu-id="732be-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="732be-121">Request headers</span></span>

| <span data-ttu-id="732be-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="732be-122">Header</span></span>       | <span data-ttu-id="732be-123">Valor</span><span class="sxs-lookup"><span data-stu-id="732be-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="732be-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="732be-124">Authorization</span></span>  | <span data-ttu-id="732be-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="732be-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="732be-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="732be-127">Request body</span></span>

<span data-ttu-id="732be-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="732be-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="732be-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="732be-129">Response</span></span>

<span data-ttu-id="732be-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="732be-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="732be-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="732be-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="732be-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="732be-133">Request</span></span>

<span data-ttu-id="732be-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="732be-134">The following is an example of the request.</span></span>
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->


<!-- {
  "blockType": "request",
  "name": "completeMigration_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/completeMigration
```


<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="732be-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="732be-135">Response</span></span>

<span data-ttu-id="732be-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="732be-136">The following is an example of the response.</span></span>
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
