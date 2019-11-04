---
title: Atualizar skillProficiency
description: Atualiza as propriedades do objeto skillProficiency no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6583336fbf6391103b15e8892207129d44524873
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937592"
---
# <a name="update-skillproficiency"></a><span data-ttu-id="33429-103">Atualizar skillproficiency</span><span class="sxs-lookup"><span data-stu-id="33429-103">Update skillproficiency</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33429-104">Atualiza as propriedades de um objeto [skillProficiency](../resources/skillproficiency.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="33429-104">Update the properties of a [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="33429-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="33429-105">Permissions</span></span>

<span data-ttu-id="33429-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="33429-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33429-108">Permission type</span></span>                        | <span data-ttu-id="33429-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33429-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="33429-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33429-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="33429-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="33429-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="33429-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33429-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33429-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="33429-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="33429-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33429-114">Application</span></span>                            | <span data-ttu-id="33429-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33429-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="33429-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33429-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/skills/{id}
```

## <a name="request-headers"></a><span data-ttu-id="33429-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33429-117">Request headers</span></span>

| <span data-ttu-id="33429-118">Nome</span><span class="sxs-lookup"><span data-stu-id="33429-118">Name</span></span>           |<span data-ttu-id="33429-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="33429-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="33429-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="33429-120">Authorization</span></span>  | <span data-ttu-id="33429-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33429-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="33429-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33429-123">Content-Type</span></span>   | <span data-ttu-id="33429-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33429-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="33429-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33429-126">Request body</span></span>

<span data-ttu-id="33429-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="33429-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="33429-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="33429-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="33429-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="33429-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="33429-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33429-130">Property</span></span>     | <span data-ttu-id="33429-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="33429-131">Type</span></span>            | <span data-ttu-id="33429-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="33429-132">Description</span></span>                                                                                                                        |
|:-------------|:----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="33429-133">categories</span><span class="sxs-lookup"><span data-stu-id="33429-133">categories</span></span>    |<span data-ttu-id="33429-134">String collection</span><span class="sxs-lookup"><span data-stu-id="33429-134">String collection</span></span>| <span data-ttu-id="33429-135">Contém categorias que um usuário associou à habilidade (por exemplo: pessoal, profissional, hobby)</span><span class="sxs-lookup"><span data-stu-id="33429-135">Contains categories a user has associated with the skill (eg: personal, professional, hobby)</span></span>                                       |
|<span data-ttu-id="33429-136">displayName</span><span class="sxs-lookup"><span data-stu-id="33429-136">displayName</span></span>   |<span data-ttu-id="33429-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33429-137">String</span></span>           | <span data-ttu-id="33429-138">Contém um nome amigável para a habilidade.</span><span class="sxs-lookup"><span data-stu-id="33429-138">Contains a friendly name for the skill.</span></span>                                                                                            | 
|<span data-ttu-id="33429-139">proficiência</span><span class="sxs-lookup"><span data-stu-id="33429-139">proficiency</span></span>   |<span data-ttu-id="33429-140">string</span><span class="sxs-lookup"><span data-stu-id="33429-140">string</span></span>           | <span data-ttu-id="33429-141">Os possíveis valores são: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="33429-141">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="33429-142">webUrl</span><span class="sxs-lookup"><span data-stu-id="33429-142">webUrl</span></span>        |<span data-ttu-id="33429-143">String</span><span class="sxs-lookup"><span data-stu-id="33429-143">String</span></span>           | <span data-ttu-id="33429-144">Contém um link para uma fonte de informações sobre a habilidade.</span><span class="sxs-lookup"><span data-stu-id="33429-144">Contains a link to an information source about the skill.</span></span>                                                                          |

## <a name="response"></a><span data-ttu-id="33429-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="33429-145">Response</span></span>

<span data-ttu-id="33429-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [skillProficiency](../resources/skillproficiency.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33429-146">If successful, this method returns a `200 OK` response code and an updated [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="33429-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="33429-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="33429-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33429-148">Request</span></span>

<span data-ttu-id="33429-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="33429-149">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="33429-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="33429-150">Response</span></span>

<span data-ttu-id="33429-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="33429-151">The following is an example of the response.</span></span>

> <span data-ttu-id="33429-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33429-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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