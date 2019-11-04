---
title: Atualizar personWebsite
description: Atualiza as propriedades de um objeto personWebsite no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b782981d52f2092aff2d1f99d749e879910289bb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937837"
---
# <a name="update-personwebsite"></a><span data-ttu-id="43bf0-103">Atualizar personwebsite</span><span class="sxs-lookup"><span data-stu-id="43bf0-103">Update personwebsite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43bf0-104">Atualiza as propriedades do objeto [personWebsite](../resources/personwebsite.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="43bf0-104">Update the properties of [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="43bf0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="43bf0-105">Permissions</span></span>

<span data-ttu-id="43bf0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43bf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43bf0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43bf0-108">Permission type</span></span>                        | <span data-ttu-id="43bf0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43bf0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="43bf0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43bf0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="43bf0-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="43bf0-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="43bf0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43bf0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43bf0-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="43bf0-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="43bf0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43bf0-114">Application</span></span>                            | <span data-ttu-id="43bf0-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43bf0-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="43bf0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43bf0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/websites/{id}
```

## <a name="request-headers"></a><span data-ttu-id="43bf0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43bf0-117">Request headers</span></span>

| <span data-ttu-id="43bf0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="43bf0-118">Name</span></span>           |<span data-ttu-id="43bf0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="43bf0-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="43bf0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="43bf0-120">Authorization</span></span>  | <span data-ttu-id="43bf0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43bf0-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="43bf0-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="43bf0-123">Content-Type</span></span>   | <span data-ttu-id="43bf0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43bf0-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43bf0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43bf0-126">Request body</span></span>

<span data-ttu-id="43bf0-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="43bf0-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="43bf0-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="43bf0-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="43bf0-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="43bf0-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="43bf0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43bf0-130">Property</span></span>     | <span data-ttu-id="43bf0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="43bf0-131">Type</span></span>            | <span data-ttu-id="43bf0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="43bf0-132">Description</span></span>                                                                         |
|:-------------|:----------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="43bf0-133">categories</span><span class="sxs-lookup"><span data-stu-id="43bf0-133">categories</span></span>    |<span data-ttu-id="43bf0-134">String collection</span><span class="sxs-lookup"><span data-stu-id="43bf0-134">String collection</span></span>| <span data-ttu-id="43bf0-135">Contém categorias que um usuário associou ao site (por exemplo: pessoal, receitas)</span><span class="sxs-lookup"><span data-stu-id="43bf0-135">Contains categories a user has associated with the website (eg: personal, recipes)</span></span>  |
|<span data-ttu-id="43bf0-136">description</span><span class="sxs-lookup"><span data-stu-id="43bf0-136">description</span></span>   |<span data-ttu-id="43bf0-137">String</span><span class="sxs-lookup"><span data-stu-id="43bf0-137">String</span></span>           | <span data-ttu-id="43bf0-138">Contém uma descrição do site.</span><span class="sxs-lookup"><span data-stu-id="43bf0-138">Contains a description of the website.</span></span>                                              |
|<span data-ttu-id="43bf0-139">displayName</span><span class="sxs-lookup"><span data-stu-id="43bf0-139">displayName</span></span>   |<span data-ttu-id="43bf0-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43bf0-140">String</span></span>           | <span data-ttu-id="43bf0-141">Contém um nome amigável para o site.</span><span class="sxs-lookup"><span data-stu-id="43bf0-141">Contains a friendly name for the website.</span></span>                                           |
|<span data-ttu-id="43bf0-142">webUrl</span><span class="sxs-lookup"><span data-stu-id="43bf0-142">webUrl</span></span>        |<span data-ttu-id="43bf0-143">String</span><span class="sxs-lookup"><span data-stu-id="43bf0-143">String</span></span>           | <span data-ttu-id="43bf0-144">Contém um link para o próprio site.</span><span class="sxs-lookup"><span data-stu-id="43bf0-144">Contains a link to the website itself.</span></span>                                              |

## <a name="response"></a><span data-ttu-id="43bf0-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="43bf0-145">Response</span></span>

<span data-ttu-id="43bf0-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [personWebsite](../resources/personwebsite.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43bf0-146">If successful, this method returns a `200 OK` response code and an updated [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="43bf0-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="43bf0-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="43bf0-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43bf0-148">Request</span></span>

<span data-ttu-id="43bf0-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43bf0-149">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_personwebsite"
}-->

```http
PATCH https://graph.microsoft.com/beta/user/profile/websites/{id}
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

### <a name="response"></a><span data-ttu-id="43bf0-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="43bf0-150">Response</span></span>

<span data-ttu-id="43bf0-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43bf0-151">The following is an example of the response.</span></span>

> <span data-ttu-id="43bf0-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43bf0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
} -->

```http
HTTP/1.1 200 OK
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
  "description": "Update personwebsite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->