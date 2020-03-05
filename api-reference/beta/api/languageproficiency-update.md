---
title: Atualizar languageProficiency
description: Atualiza as propriedades de um objeto languageProficiency no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 66170677d505d235a45031a9b606f923f17ebe02
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457206"
---
# <a name="update-languageproficiency"></a><span data-ttu-id="4b051-103">Atualizar languageProficiency</span><span class="sxs-lookup"><span data-stu-id="4b051-103">Update languageProficiency</span></span>

<span data-ttu-id="4b051-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4b051-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b051-105">Atualiza as propriedades de um objeto [languageProficiency](../resources/languageproficiency.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4b051-105">Update the properties of a [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4b051-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b051-106">Permissions</span></span>

<span data-ttu-id="4b051-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b051-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b051-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b051-109">Permission type</span></span>                        | <span data-ttu-id="4b051-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b051-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b051-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b051-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b051-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4b051-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4b051-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b051-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b051-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4b051-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4b051-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b051-115">Application</span></span>                            | <span data-ttu-id="4b051-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b051-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="4b051-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b051-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4b051-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b051-118">Request headers</span></span>

| <span data-ttu-id="4b051-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4b051-119">Name</span></span>           |<span data-ttu-id="4b051-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b051-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="4b051-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b051-121">Authorization</span></span>  | <span data-ttu-id="4b051-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b051-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="4b051-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b051-124">Content-Type</span></span>   | <span data-ttu-id="4b051-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b051-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b051-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b051-127">Request body</span></span>

<span data-ttu-id="4b051-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="4b051-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4b051-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="4b051-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4b051-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4b051-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4b051-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b051-131">Property</span></span>     | <span data-ttu-id="4b051-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b051-132">Type</span></span>        | <span data-ttu-id="4b051-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b051-133">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="4b051-134">displayName</span><span class="sxs-lookup"><span data-stu-id="4b051-134">displayName</span></span>   |<span data-ttu-id="4b051-135">String</span><span class="sxs-lookup"><span data-stu-id="4b051-135">String</span></span>       | <span data-ttu-id="4b051-136">Contém o nome de formato longo do idioma em questão.</span><span class="sxs-lookup"><span data-stu-id="4b051-136">Contains the long-form name for the language in question.</span></span>                                                                                                   |
|<span data-ttu-id="4b051-137">proficiência</span><span class="sxs-lookup"><span data-stu-id="4b051-137">proficiency</span></span>   |<span data-ttu-id="4b051-138">string</span><span class="sxs-lookup"><span data-stu-id="4b051-138">string</span></span>       | <span data-ttu-id="4b051-139">Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4b051-139">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4b051-140">tag</span><span class="sxs-lookup"><span data-stu-id="4b051-140">tag</span></span>           |<span data-ttu-id="4b051-141">String</span><span class="sxs-lookup"><span data-stu-id="4b051-141">String</span></span>       | <span data-ttu-id="4b051-142">Contém o nome de BCP47 de 4 caracteres para o idioma (en-US, no-NB, en-AU)</span><span class="sxs-lookup"><span data-stu-id="4b051-142">Contains the 4 character BCP47 name for the language (en-US, no-NB, en-AU)</span></span>                                                                                  |

## <a name="response"></a><span data-ttu-id="4b051-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b051-143">Response</span></span>

<span data-ttu-id="4b051-144">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [languageProficiency](../resources/languageproficiency.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b051-144">If successful, this method returns a `200 OK` response code and an updated [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b051-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4b051-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4b051-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b051-146">Request</span></span>

<span data-ttu-id="4b051-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b051-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b051-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b051-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_languageproficiency"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/languages/{id}
Content-type: application/json

{
  "displayName": "displayName-value",
  "tag": "tag-value",
  "proficiency": "proficiency-value"
}
```
# <a name="c"></a>[<span data-ttu-id="4b051-149">C#</span><span class="sxs-lookup"><span data-stu-id="4b051-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-languageproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b051-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b051-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-languageproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b051-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b051-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-languageproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4b051-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b051-152">Response</span></span>

<span data-ttu-id="4b051-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4b051-153">The following is an example of the response.</span></span>

> <span data-ttu-id="4b051-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b051-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.languageProficiency"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "tag": "tag-value",
  "proficiency": "proficiency-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update languageproficiency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
