---
title: Atualizar personWebsite
description: Atualiza as propriedades de um objeto personWebsite no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b93d1ea6fa1449bf6491d3ed574e709ff2c883c5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455862"
---
# <a name="update-personwebsite"></a><span data-ttu-id="0e9c3-103">Atualizar personwebsite</span><span class="sxs-lookup"><span data-stu-id="0e9c3-103">Update personwebsite</span></span>

<span data-ttu-id="0e9c3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0e9c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e9c3-105">Atualiza as propriedades do objeto [personWebsite](../resources/personwebsite.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="0e9c3-105">Update the properties of [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e9c3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e9c3-106">Permissions</span></span>

<span data-ttu-id="0e9c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e9c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e9c3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e9c3-109">Permission type</span></span>                        | <span data-ttu-id="0e9c3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e9c3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0e9c3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e9c3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e9c3-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0e9c3-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0e9c3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e9c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e9c3-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0e9c3-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0e9c3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e9c3-115">Application</span></span>                            | <span data-ttu-id="0e9c3-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e9c3-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="0e9c3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e9c3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/websites/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0e9c3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e9c3-118">Request headers</span></span>

| <span data-ttu-id="0e9c3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0e9c3-119">Name</span></span>           |<span data-ttu-id="0e9c3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e9c3-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="0e9c3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e9c3-121">Authorization</span></span>  | <span data-ttu-id="0e9c3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e9c3-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0e9c3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e9c3-124">Content-Type</span></span>   | <span data-ttu-id="0e9c3-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e9c3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e9c3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e9c3-127">Request body</span></span>

<span data-ttu-id="0e9c3-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0e9c3-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0e9c3-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="0e9c3-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0e9c3-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0e9c3-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0e9c3-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e9c3-131">Property</span></span>     | <span data-ttu-id="0e9c3-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e9c3-132">Type</span></span>            | <span data-ttu-id="0e9c3-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e9c3-133">Description</span></span>                                                                         |
|:-------------|:----------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="0e9c3-134">categories</span><span class="sxs-lookup"><span data-stu-id="0e9c3-134">categories</span></span>    |<span data-ttu-id="0e9c3-135">String collection</span><span class="sxs-lookup"><span data-stu-id="0e9c3-135">String collection</span></span>| <span data-ttu-id="0e9c3-136">Contém categorias que um usuário associou ao site (por exemplo: pessoal, receitas)</span><span class="sxs-lookup"><span data-stu-id="0e9c3-136">Contains categories a user has associated with the website (eg: personal, recipes)</span></span>  |
|<span data-ttu-id="0e9c3-137">description</span><span class="sxs-lookup"><span data-stu-id="0e9c3-137">description</span></span>   |<span data-ttu-id="0e9c3-138">String</span><span class="sxs-lookup"><span data-stu-id="0e9c3-138">String</span></span>           | <span data-ttu-id="0e9c3-139">Contém uma descrição do site.</span><span class="sxs-lookup"><span data-stu-id="0e9c3-139">Contains a description of the website.</span></span>                                              |
|<span data-ttu-id="0e9c3-140">displayName</span><span class="sxs-lookup"><span data-stu-id="0e9c3-140">displayName</span></span>   |<span data-ttu-id="0e9c3-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e9c3-141">String</span></span>           | <span data-ttu-id="0e9c3-142">Contém um nome amigável para o site.</span><span class="sxs-lookup"><span data-stu-id="0e9c3-142">Contains a friendly name for the website.</span></span>                                           |
|<span data-ttu-id="0e9c3-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="0e9c3-143">webUrl</span></span>        |<span data-ttu-id="0e9c3-144">String</span><span class="sxs-lookup"><span data-stu-id="0e9c3-144">String</span></span>           | <span data-ttu-id="0e9c3-145">Contém um link para o próprio site.</span><span class="sxs-lookup"><span data-stu-id="0e9c3-145">Contains a link to the website itself.</span></span>                                              |

## <a name="response"></a><span data-ttu-id="0e9c3-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e9c3-146">Response</span></span>

<span data-ttu-id="0e9c3-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [personWebsite](../resources/personwebsite.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e9c3-147">If successful, this method returns a `200 OK` response code and an updated [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e9c3-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0e9c3-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e9c3-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e9c3-149">Request</span></span>

<span data-ttu-id="0e9c3-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e9c3-150">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0e9c3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e9c3-151">Response</span></span>

<span data-ttu-id="0e9c3-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0e9c3-152">The following is an example of the response.</span></span>

> <span data-ttu-id="0e9c3-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e9c3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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