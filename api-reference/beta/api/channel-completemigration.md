---
title: 'canal: completeMigration'
description: Conclua a migração de mensagens externas, removendo o modo de migração de um canal.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 894c8353b626b1f4cebe62bd00311533933df5a7
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48783027"
---
# <a name="channel-completemigration"></a><span data-ttu-id="86aba-103">canal: completeMigration</span><span class="sxs-lookup"><span data-stu-id="86aba-103">channel: completeMigration</span></span>

<span data-ttu-id="86aba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86aba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86aba-105">Conclua o processo de migração de mensagens removendo `migration mode` de um [canal](../resources/channel.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="86aba-105">Complete the message migration process by removing `migration mode` from a [channel](../resources/channel.md) in a team.</span></span> <span data-ttu-id="86aba-106">`Migration mode` é um estado especial que impede determinadas operações, como a criação de mensagens e a adição de membros, durante o processo de migração de dados.</span><span class="sxs-lookup"><span data-stu-id="86aba-106">`Migration mode` is a special state that prevents certain operations, like creating messages and adding members, during the data migration process.</span></span>

<span data-ttu-id="86aba-107">Depois que uma solicitação **completeMigration** é feita, não é possível importar mensagens adicionais para a equipe.</span><span class="sxs-lookup"><span data-stu-id="86aba-107">After a **completeMigration** request is made, you cannot import additional messages into the team.</span></span> <span data-ttu-id="86aba-108">Você pode adicionar membros à equipe depois que a solicitação retornar uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="86aba-108">You can add members to the team after the request returns a successful response.</span></span>

## <a name="permissions"></a><span data-ttu-id="86aba-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="86aba-109">Permissions</span></span>

<span data-ttu-id="86aba-110">A seguinte permissão é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="86aba-110">The following permission is required to call this API.</span></span> <span data-ttu-id="86aba-111">Para saber mais, *Confira* [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86aba-111">To learn more, *see* [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86aba-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86aba-112">Permission type</span></span>      | <span data-ttu-id="86aba-113">Permissão</span><span class="sxs-lookup"><span data-stu-id="86aba-113">Permission</span></span>  |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="86aba-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86aba-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="86aba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86aba-115">Not supported.</span></span>|
| <span data-ttu-id="86aba-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86aba-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86aba-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86aba-117">Not supported.</span></span> |
|<span data-ttu-id="86aba-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86aba-118">Application</span></span> | <span data-ttu-id="86aba-119">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="86aba-119">Teamwork.Migrate.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86aba-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86aba-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{teamId}/channels/{channelId}/completeMigration
```

## <a name="request-headers"></a><span data-ttu-id="86aba-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86aba-121">Request headers</span></span>

| <span data-ttu-id="86aba-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86aba-122">Header</span></span>       | <span data-ttu-id="86aba-123">Valor</span><span class="sxs-lookup"><span data-stu-id="86aba-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="86aba-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="86aba-124">Authorization</span></span>  | <span data-ttu-id="86aba-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86aba-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86aba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86aba-127">Request body</span></span>

<span data-ttu-id="86aba-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86aba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86aba-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="86aba-129">Response</span></span>

<span data-ttu-id="86aba-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86aba-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86aba-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86aba-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="86aba-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86aba-133">Request</span></span>

<span data-ttu-id="86aba-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="86aba-134">The following is an example of the request.</span></span>
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->

<!-- {
  "blockType": "request",
  "name": "completeMigration_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/completeMigration
```
<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="86aba-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="86aba-135">Response</span></span>

<span data-ttu-id="86aba-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="86aba-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 5793eec6-0e5a-11eb-adc1-0242ac120002
2020-10-14 20:22:11 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "completeMigration_ channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
