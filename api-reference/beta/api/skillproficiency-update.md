---
title: Atualizar skillProficiency
description: Atualiza as propriedades do objeto skillProficiency no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1fd014c397575ce6977ee2a57c61a89ac7af59a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453129"
---
# <a name="update-skillproficiency"></a><span data-ttu-id="7465f-103">Atualizar skillproficiency</span><span class="sxs-lookup"><span data-stu-id="7465f-103">Update skillproficiency</span></span>

<span data-ttu-id="7465f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7465f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7465f-105">Atualiza as propriedades de um objeto [skillProficiency](../resources/skillproficiency.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7465f-105">Update the properties of a [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7465f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7465f-106">Permissions</span></span>

<span data-ttu-id="7465f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7465f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7465f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7465f-109">Permission type</span></span>                        | <span data-ttu-id="7465f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7465f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7465f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7465f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7465f-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7465f-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="7465f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7465f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7465f-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7465f-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="7465f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7465f-115">Application</span></span>                            | <span data-ttu-id="7465f-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7465f-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="7465f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7465f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/skills/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7465f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7465f-118">Request headers</span></span>

| <span data-ttu-id="7465f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7465f-119">Name</span></span>           |<span data-ttu-id="7465f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7465f-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="7465f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7465f-121">Authorization</span></span>  | <span data-ttu-id="7465f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7465f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="7465f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7465f-124">Content-Type</span></span>   | <span data-ttu-id="7465f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7465f-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="7465f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7465f-127">Request body</span></span>

<span data-ttu-id="7465f-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="7465f-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7465f-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="7465f-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7465f-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7465f-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7465f-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7465f-131">Property</span></span>     | <span data-ttu-id="7465f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="7465f-132">Type</span></span>            | <span data-ttu-id="7465f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7465f-133">Description</span></span>                                                                                                                        |
|:-------------|:----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="7465f-134">categories</span><span class="sxs-lookup"><span data-stu-id="7465f-134">categories</span></span>    |<span data-ttu-id="7465f-135">String collection</span><span class="sxs-lookup"><span data-stu-id="7465f-135">String collection</span></span>| <span data-ttu-id="7465f-136">Contém categorias que um usuário associou à habilidade (por exemplo: pessoal, profissional, hobby)</span><span class="sxs-lookup"><span data-stu-id="7465f-136">Contains categories a user has associated with the skill (eg: personal, professional, hobby)</span></span>                                       |
|<span data-ttu-id="7465f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7465f-137">displayName</span></span>   |<span data-ttu-id="7465f-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7465f-138">String</span></span>           | <span data-ttu-id="7465f-139">Contém um nome amigável para a habilidade.</span><span class="sxs-lookup"><span data-stu-id="7465f-139">Contains a friendly name for the skill.</span></span>                                                                                            | 
|<span data-ttu-id="7465f-140">proficiência</span><span class="sxs-lookup"><span data-stu-id="7465f-140">proficiency</span></span>   |<span data-ttu-id="7465f-141">string</span><span class="sxs-lookup"><span data-stu-id="7465f-141">string</span></span>           | <span data-ttu-id="7465f-142">Os possíveis valores são: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7465f-142">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7465f-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="7465f-143">webUrl</span></span>        |<span data-ttu-id="7465f-144">String</span><span class="sxs-lookup"><span data-stu-id="7465f-144">String</span></span>           | <span data-ttu-id="7465f-145">Contém um link para uma fonte de informações sobre a habilidade.</span><span class="sxs-lookup"><span data-stu-id="7465f-145">Contains a link to an information source about the skill.</span></span>                                                                          |

## <a name="response"></a><span data-ttu-id="7465f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7465f-146">Response</span></span>

<span data-ttu-id="7465f-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [skillProficiency](../resources/skillproficiency.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7465f-147">If successful, this method returns a `200 OK` response code and an updated [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7465f-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7465f-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7465f-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7465f-149">Request</span></span>

<span data-ttu-id="7465f-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7465f-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7465f-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="7465f-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_skillproficiency"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/skills/{id}
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "displayName": "displayName-value",
  "proficiency": "proficiency-value",
  "webUrl": "webUrl-value"
}
```
# <a name="c"></a>[<span data-ttu-id="7465f-152">C#</span><span class="sxs-lookup"><span data-stu-id="7465f-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-skillproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7465f-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7465f-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-skillproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7465f-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7465f-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-skillproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7465f-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="7465f-155">Response</span></span>

<span data-ttu-id="7465f-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7465f-156">The following is an example of the response.</span></span>

> <span data-ttu-id="7465f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7465f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "displayName": "displayName-value",
  "proficiency": "proficiency-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update skillproficiency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
