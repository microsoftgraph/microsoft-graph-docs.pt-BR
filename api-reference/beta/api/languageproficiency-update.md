---
title: Atualizar languageProficiency
description: Atualiza as propriedades de um objeto languageProficiency no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6d85263db9d54565613678d4941594e5df312d57
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998238"
---
# <a name="update-languageproficiency"></a><span data-ttu-id="e9cd6-103">Atualizar languageProficiency</span><span class="sxs-lookup"><span data-stu-id="e9cd6-103">Update languageProficiency</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9cd6-104">Atualiza as propriedades de um objeto [languageProficiency](../resources/languageproficiency.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e9cd6-104">Update the properties of a [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9cd6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9cd6-105">Permissions</span></span>

<span data-ttu-id="e9cd6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9cd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9cd6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9cd6-108">Permission type</span></span>                        | <span data-ttu-id="e9cd6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9cd6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e9cd6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9cd6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9cd6-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e9cd6-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e9cd6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9cd6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9cd6-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e9cd6-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e9cd6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9cd6-114">Application</span></span>                            | <span data-ttu-id="e9cd6-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9cd6-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e9cd6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9cd6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e9cd6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9cd6-117">Request headers</span></span>

| <span data-ttu-id="e9cd6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e9cd6-118">Name</span></span>           |<span data-ttu-id="e9cd6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9cd6-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="e9cd6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9cd6-120">Authorization</span></span>  | <span data-ttu-id="e9cd6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9cd6-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e9cd6-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9cd6-123">Content-Type</span></span>   | <span data-ttu-id="e9cd6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9cd6-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9cd6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9cd6-126">Request body</span></span>

<span data-ttu-id="e9cd6-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="e9cd6-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e9cd6-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="e9cd6-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e9cd6-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e9cd6-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e9cd6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9cd6-130">Property</span></span>     | <span data-ttu-id="e9cd6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9cd6-131">Type</span></span>        | <span data-ttu-id="e9cd6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9cd6-132">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="e9cd6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e9cd6-133">displayName</span></span>   |<span data-ttu-id="e9cd6-134">String</span><span class="sxs-lookup"><span data-stu-id="e9cd6-134">String</span></span>       | <span data-ttu-id="e9cd6-135">Contém o nome de formato longo do idioma em questão.</span><span class="sxs-lookup"><span data-stu-id="e9cd6-135">Contains the long-form name for the language in question.</span></span>                                                                                                   |
|<span data-ttu-id="e9cd6-136">proficiência</span><span class="sxs-lookup"><span data-stu-id="e9cd6-136">proficiency</span></span>   |<span data-ttu-id="e9cd6-137">string</span><span class="sxs-lookup"><span data-stu-id="e9cd6-137">string</span></span>       | <span data-ttu-id="e9cd6-138">Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e9cd6-138">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e9cd6-139">tag</span><span class="sxs-lookup"><span data-stu-id="e9cd6-139">tag</span></span>           |<span data-ttu-id="e9cd6-140">String</span><span class="sxs-lookup"><span data-stu-id="e9cd6-140">String</span></span>       | <span data-ttu-id="e9cd6-141">Contém o nome de BCP47 de 4 caracteres para o idioma (en-US, no-NB, en-AU)</span><span class="sxs-lookup"><span data-stu-id="e9cd6-141">Contains the 4 character BCP47 name for the language (en-US, no-NB, en-AU)</span></span>                                                                                  |

## <a name="response"></a><span data-ttu-id="e9cd6-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9cd6-142">Response</span></span>

<span data-ttu-id="e9cd6-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [languageProficiency](../resources/languageproficiency.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9cd6-143">If successful, this method returns a `200 OK` response code and an updated [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9cd6-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e9cd6-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9cd6-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9cd6-145">Request</span></span>

<span data-ttu-id="e9cd6-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9cd6-146">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e9cd6-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9cd6-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e9cd6-148">C#</span><span class="sxs-lookup"><span data-stu-id="e9cd6-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-languageproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9cd6-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9cd6-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-languageproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e9cd6-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9cd6-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-languageproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e9cd6-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9cd6-151">Response</span></span>

<span data-ttu-id="e9cd6-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e9cd6-152">The following is an example of the response.</span></span>

> <span data-ttu-id="e9cd6-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9cd6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
