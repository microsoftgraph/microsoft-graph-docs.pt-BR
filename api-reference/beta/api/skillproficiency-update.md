---
title: Atualizar skillProficiency
description: Atualize as propriedades do objeto skillProficiency no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9da18f3fc53cac80fc4f357083c6dea3c95d5c84
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048985"
---
# <a name="update-skillproficiency"></a><span data-ttu-id="34b6f-103">Atualizar a qualificação</span><span class="sxs-lookup"><span data-stu-id="34b6f-103">Update skillproficiency</span></span>

<span data-ttu-id="34b6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34b6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34b6f-105">Atualize as propriedades de [um objeto skillProficiency](../resources/skillproficiency.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="34b6f-105">Update the properties of a [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="34b6f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="34b6f-106">Permissions</span></span>

<span data-ttu-id="34b6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34b6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34b6f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34b6f-109">Permission type</span></span>                        | <span data-ttu-id="34b6f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34b6f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="34b6f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34b6f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="34b6f-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34b6f-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="34b6f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34b6f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34b6f-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34b6f-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="34b6f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34b6f-115">Application</span></span>                            | <span data-ttu-id="34b6f-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34b6f-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="34b6f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34b6f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/skills/{id}
PATCH /users/{id | userPrincipalName}/profile/skills/{id}
```

## <a name="request-headers"></a><span data-ttu-id="34b6f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34b6f-118">Request headers</span></span>

| <span data-ttu-id="34b6f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="34b6f-119">Name</span></span>           |<span data-ttu-id="34b6f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="34b6f-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="34b6f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="34b6f-121">Authorization</span></span>  | <span data-ttu-id="34b6f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34b6f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="34b6f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34b6f-124">Content-Type</span></span>   | <span data-ttu-id="34b6f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34b6f-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="34b6f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34b6f-127">Request body</span></span>

<span data-ttu-id="34b6f-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="34b6f-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="34b6f-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="34b6f-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="34b6f-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="34b6f-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="34b6f-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34b6f-131">Property</span></span>|<span data-ttu-id="34b6f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="34b6f-132">Type</span></span>|<span data-ttu-id="34b6f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="34b6f-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34b6f-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="34b6f-134">allowedAudiences</span></span>|<span data-ttu-id="34b6f-135">String</span><span class="sxs-lookup"><span data-stu-id="34b6f-135">String</span></span>|<span data-ttu-id="34b6f-136">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="34b6f-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="34b6f-137">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="34b6f-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="34b6f-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="34b6f-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="34b6f-139">categories</span><span class="sxs-lookup"><span data-stu-id="34b6f-139">categories</span></span>|<span data-ttu-id="34b6f-140">String collection</span><span class="sxs-lookup"><span data-stu-id="34b6f-140">String collection</span></span>|<span data-ttu-id="34b6f-141">Contém categorias que um usuário associou à habilidade (por exemplo, pessoal, profissional, hobby).</span><span class="sxs-lookup"><span data-stu-id="34b6f-141">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span> |
|<span data-ttu-id="34b6f-142">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="34b6f-142">collaborationTags</span></span>|<span data-ttu-id="34b6f-143">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="34b6f-143">String collection</span></span>|<span data-ttu-id="34b6f-144">Contém marcas de cenário de experiência que um usuário associou aos juros.</span><span class="sxs-lookup"><span data-stu-id="34b6f-144">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="34b6f-145">Os valores permitidos na coleção são: `askMeAbout` `ableToMentor` , , , `wantsToLearn` `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="34b6f-145">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="34b6f-146">displayName</span><span class="sxs-lookup"><span data-stu-id="34b6f-146">displayName</span></span>|<span data-ttu-id="34b6f-147">String</span><span class="sxs-lookup"><span data-stu-id="34b6f-147">String</span></span>|<span data-ttu-id="34b6f-148">Contém um nome amigável para a habilidade.</span><span class="sxs-lookup"><span data-stu-id="34b6f-148">Contains a friendly name for the skill.</span></span> |
|<span data-ttu-id="34b6f-149">inferência</span><span class="sxs-lookup"><span data-stu-id="34b6f-149">inference</span></span>|[<span data-ttu-id="34b6f-150">inferenceData</span><span class="sxs-lookup"><span data-stu-id="34b6f-150">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="34b6f-151">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="34b6f-151">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="34b6f-152">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="34b6f-152">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="34b6f-153">proficiência</span><span class="sxs-lookup"><span data-stu-id="34b6f-153">proficiency</span></span>|<span data-ttu-id="34b6f-154">skillProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="34b6f-154">skillProficiencyLevel</span></span>|<span data-ttu-id="34b6f-155">Detalhes da proficiência dos usuários com essa habilidade.</span><span class="sxs-lookup"><span data-stu-id="34b6f-155">Detail of the users proficiency with this skill.</span></span> <span data-ttu-id="34b6f-156">Os possíveis valores são: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="34b6f-156">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="34b6f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="34b6f-157">Response</span></span>

<span data-ttu-id="34b6f-158">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto skillProficiency](../resources/skillproficiency.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34b6f-158">If successful, this method returns a `200 OK` response code and an updated [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="34b6f-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="34b6f-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="34b6f-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34b6f-160">Request</span></span>

<span data-ttu-id="34b6f-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="34b6f-161">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="34b6f-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="34b6f-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_skillproficiency"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/skills/{id}
Content-type: application/json

{
  "categories": [
    "Professional"
  ],
  "proficiency": "advancedProfessional"
}
```
# <a name="c"></a>[<span data-ttu-id="34b6f-163">C#</span><span class="sxs-lookup"><span data-stu-id="34b6f-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-skillproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34b6f-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34b6f-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-skillproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34b6f-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34b6f-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-skillproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="34b6f-166">Java</span><span class="sxs-lookup"><span data-stu-id="34b6f-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-skillproficiency-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="34b6f-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="34b6f-167">Response</span></span>

<span data-ttu-id="34b6f-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="34b6f-168">The following is an example of the response.</span></span>

> <span data-ttu-id="34b6f-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="34b6f-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "categories": [
    "Professional"
  ],
  "displayName": "API Design",
  "proficiency": "advancedProfessional",
  "webUrl": null,
  "collaborationTags": [
    "ableToMentor"
  ]
}
```


