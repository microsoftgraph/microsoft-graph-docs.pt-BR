---
title: Atualizar email
description: Atualizar as propriedades de um objeto item de email no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 7bdf72ee1499f28a220461093fc26ae64e070878
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938440"
---
# <a name="update-itememail"></a><span data-ttu-id="8ff53-103">Atualizar email</span><span class="sxs-lookup"><span data-stu-id="8ff53-103">Update itememail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ff53-104">Atualizar as propriedades de um objeto item de [email](../resources/itememail.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8ff53-104">Update the properties of an [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8ff53-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ff53-105">Permissions</span></span>

<span data-ttu-id="8ff53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ff53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ff53-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ff53-108">Permission type</span></span>                        | <span data-ttu-id="8ff53-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ff53-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8ff53-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ff53-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ff53-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8ff53-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8ff53-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ff53-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ff53-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8ff53-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8ff53-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ff53-114">Application</span></span>                            | <span data-ttu-id="8ff53-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff53-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="8ff53-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ff53-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/emails/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="8ff53-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff53-117">Request headers</span></span>

| <span data-ttu-id="8ff53-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8ff53-118">Name</span></span>           |<span data-ttu-id="8ff53-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ff53-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="8ff53-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ff53-120">Authorization</span></span>  | <span data-ttu-id="8ff53-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ff53-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8ff53-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ff53-123">Content-Type</span></span>   | <span data-ttu-id="8ff53-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ff53-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ff53-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff53-126">Request body</span></span>

<span data-ttu-id="8ff53-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="8ff53-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8ff53-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="8ff53-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8ff53-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8ff53-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8ff53-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ff53-130">Property</span></span>     | <span data-ttu-id="8ff53-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ff53-131">Type</span></span>        | <span data-ttu-id="8ff53-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ff53-132">Description</span></span>                                                              |
|:-------------|:------------|:-------------------------------------------------------------------------|
|<span data-ttu-id="8ff53-133">address</span><span class="sxs-lookup"><span data-stu-id="8ff53-133">address</span></span>       |<span data-ttu-id="8ff53-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ff53-134">String</span></span>       | <span data-ttu-id="8ff53-135">O próprio endereço de email.</span><span class="sxs-lookup"><span data-stu-id="8ff53-135">The email address itself.</span></span>                                                | 
|<span data-ttu-id="8ff53-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8ff53-136">displayName</span></span>   |<span data-ttu-id="8ff53-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ff53-137">String</span></span>       | <span data-ttu-id="8ff53-138">O nome ou rótulo que um usuário associou a um endereço de email específico.</span><span class="sxs-lookup"><span data-stu-id="8ff53-138">The name or label a user has associated with a particular email address.</span></span> |
|<span data-ttu-id="8ff53-139">type</span><span class="sxs-lookup"><span data-stu-id="8ff53-139">type</span></span>          |<span data-ttu-id="8ff53-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ff53-140">string</span></span>       | <span data-ttu-id="8ff53-141">Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="8ff53-141">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>     |

## <a name="response"></a><span data-ttu-id="8ff53-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff53-142">Response</span></span>

<span data-ttu-id="8ff53-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [MyEmail](../resources/itememail.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ff53-143">If successful, this method returns a `200 OK` response code and an updated [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ff53-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8ff53-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8ff53-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff53-145">Request</span></span>

<span data-ttu-id="8ff53-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ff53-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_itememail"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/emails/{id}
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```

### <a name="response"></a><span data-ttu-id="8ff53-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff53-147">Response</span></span>

<span data-ttu-id="8ff53-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8ff53-148">The following is an example of the response.</span></span>

> <span data-ttu-id="8ff53-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ff53-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
} -->

```http
HTTP/1.1 200 OK
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
  "description": "Update itememail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->