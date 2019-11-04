---
title: Criar email
description: Criar um novo email.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 25f81760c4d4320474027d0f3d7f5113007ae94d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937704"
---
# <a name="create-itememail"></a><span data-ttu-id="b7bbe-103">Criar email</span><span class="sxs-lookup"><span data-stu-id="b7bbe-103">Create itemEmail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7bbe-104">Criar um novo [email](../resources/itememail.md).</span><span class="sxs-lookup"><span data-stu-id="b7bbe-104">Create a new [itemEmail](../resources/itememail.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b7bbe-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7bbe-105">Permissions</span></span>

<span data-ttu-id="b7bbe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7bbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7bbe-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7bbe-108">Permission type</span></span>                        | <span data-ttu-id="b7bbe-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7bbe-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b7bbe-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7bbe-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7bbe-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b7bbe-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b7bbe-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7bbe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7bbe-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b7bbe-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b7bbe-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7bbe-114">Application</span></span>                            | <span data-ttu-id="b7bbe-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7bbe-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7bbe-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7bbe-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/emails
```

## <a name="request-headers"></a><span data-ttu-id="b7bbe-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7bbe-117">Request headers</span></span>

| <span data-ttu-id="b7bbe-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b7bbe-118">Name</span></span>      |<span data-ttu-id="b7bbe-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7bbe-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b7bbe-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7bbe-120">Authorization</span></span>  | <span data-ttu-id="b7bbe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7bbe-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b7bbe-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7bbe-123">Content-Type</span></span>   | <span data-ttu-id="b7bbe-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7bbe-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7bbe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7bbe-126">Request body</span></span>

<span data-ttu-id="b7bbe-127">No corpo da solicitação, forneça uma representação JSON de um objeto de [email](../resources/itememail.md) .</span><span class="sxs-lookup"><span data-stu-id="b7bbe-127">In the request body, supply a JSON representation of an [itemEmail](../resources/itememail.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b7bbe-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7bbe-128">Response</span></span>

<span data-ttu-id="b7bbe-129">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto de [email](../resources/itememail.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7bbe-129">If successful, this method returns a `201 Created` response code and a new [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7bbe-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b7bbe-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7bbe-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7bbe-131">Request</span></span>

<span data-ttu-id="b7bbe-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7bbe-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_itememail_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/user/profile/emails
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```

### <a name="response"></a><span data-ttu-id="b7bbe-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7bbe-133">Response</span></span>

<span data-ttu-id="b7bbe-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b7bbe-134">The following is an example of the response.</span></span>

> <span data-ttu-id="b7bbe-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7bbe-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create itemEmail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
