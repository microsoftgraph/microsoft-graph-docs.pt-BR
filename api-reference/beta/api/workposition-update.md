---
title: Atualizar workPosition
description: Atualiza as propriedades de um objeto workPosition no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a00e5dc77cb98ff2fad81b963f16c1b0061be22a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092913"
---
# <a name="update-workposition"></a><span data-ttu-id="661d4-103">Atualizar workPosition</span><span class="sxs-lookup"><span data-stu-id="661d4-103">Update workPosition</span></span>

<span data-ttu-id="661d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="661d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="661d4-105">Atualiza as propriedades de um objeto [workPosition](../resources/workposition.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="661d4-105">Update the properties of a [workPosition](../resources/workposition.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="661d4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="661d4-106">Permissions</span></span>

<span data-ttu-id="661d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="661d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="661d4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="661d4-109">Permission type</span></span>                        | <span data-ttu-id="661d4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="661d4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="661d4-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="661d4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="661d4-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="661d4-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="661d4-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="661d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="661d4-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="661d4-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="661d4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="661d4-115">Application</span></span>                            | <span data-ttu-id="661d4-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="661d4-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="661d4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="661d4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/positions/{id}
PATCH /users/{id | userPrincipalName}/profile/positions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="661d4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="661d4-118">Request headers</span></span>

| <span data-ttu-id="661d4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="661d4-119">Name</span></span>           |<span data-ttu-id="661d4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="661d4-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="661d4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="661d4-121">Authorization</span></span>  | <span data-ttu-id="661d4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="661d4-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="661d4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="661d4-124">Content-Type</span></span>   | <span data-ttu-id="661d4-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="661d4-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="661d4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="661d4-127">Request body</span></span>

<span data-ttu-id="661d4-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="661d4-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="661d4-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="661d4-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="661d4-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="661d4-130">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="properties"></a><span data-ttu-id="661d4-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="661d4-131">Properties</span></span>
|<span data-ttu-id="661d4-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="661d4-132">Property</span></span>|<span data-ttu-id="661d4-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="661d4-133">Type</span></span>|<span data-ttu-id="661d4-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="661d4-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="661d4-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="661d4-135">allowedAudiences</span></span>|<span data-ttu-id="661d4-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="661d4-136">String</span></span>|<span data-ttu-id="661d4-137">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="661d4-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="661d4-138">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="661d4-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="661d4-139">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="661d4-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="661d4-140">categories</span><span class="sxs-lookup"><span data-stu-id="661d4-140">categories</span></span>|<span data-ttu-id="661d4-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="661d4-141">String collection</span></span>|<span data-ttu-id="661d4-142">Categorias que o usuário tenha associado a esta posição.</span><span class="sxs-lookup"><span data-stu-id="661d4-142">Categories that the user has associated with this position.</span></span>|
|<span data-ttu-id="661d4-143">conhecidos</span><span class="sxs-lookup"><span data-stu-id="661d4-143">colleagues</span></span>|<span data-ttu-id="661d4-144">coleção [relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="661d4-144">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="661d4-145">Colegas associados a esta posição.</span><span class="sxs-lookup"><span data-stu-id="661d4-145">Colleagues that are associated with this position.</span></span>|
|<span data-ttu-id="661d4-146">detalhada</span><span class="sxs-lookup"><span data-stu-id="661d4-146">detail</span></span>|[<span data-ttu-id="661d4-147">positionDetail</span><span class="sxs-lookup"><span data-stu-id="661d4-147">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="661d4-148">Contém informações detalhadas sobre a posição.</span><span class="sxs-lookup"><span data-stu-id="661d4-148">Contains detailed information about the position.</span></span> |
|<span data-ttu-id="661d4-149">fracassa</span><span class="sxs-lookup"><span data-stu-id="661d4-149">inference</span></span>|[<span data-ttu-id="661d4-150">inferenceData</span><span class="sxs-lookup"><span data-stu-id="661d4-150">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="661d4-151">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="661d4-151">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="661d4-152">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="661d4-152">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="661d4-153">IsCurrent</span><span class="sxs-lookup"><span data-stu-id="661d4-153">isCurrent</span></span>|<span data-ttu-id="661d4-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="661d4-154">Boolean</span></span>|<span data-ttu-id="661d4-155">Indica se a posição é ou não atual.</span><span class="sxs-lookup"><span data-stu-id="661d4-155">Denotes whether or not the position is current.</span></span>|
|<span data-ttu-id="661d4-156">manager</span><span class="sxs-lookup"><span data-stu-id="661d4-156">manager</span></span>|[<span data-ttu-id="661d4-157">relatedPerson</span><span class="sxs-lookup"><span data-stu-id="661d4-157">relatedPerson</span></span>](../resources/relatedperson.md)|<span data-ttu-id="661d4-158">Contém detalhes do gerente do usuário nesta posição.</span><span class="sxs-lookup"><span data-stu-id="661d4-158">Contains detail of the user's manager in this position.</span></span>|

## <a name="response"></a><span data-ttu-id="661d4-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="661d4-159">Response</span></span>

<span data-ttu-id="661d4-160">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [workPosition](../resources/workposition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="661d4-160">If successful, this method returns a `200 OK` response code and an updated [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="661d4-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="661d4-161">Examples</span></span>

### <a name="request"></a><span data-ttu-id="661d4-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="661d4-162">Request</span></span>

<span data-ttu-id="661d4-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="661d4-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="661d4-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="661d4-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workposition"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/positions/{id}
Content-type: application/json

{
  "isCurrent": true
}
```
# <a name="c"></a>[<span data-ttu-id="661d4-165">C#</span><span class="sxs-lookup"><span data-stu-id="661d4-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="661d4-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="661d4-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="661d4-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="661d4-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="661d4-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="661d4-168">Response</span></span>

<span data-ttu-id="661d4-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="661d4-169">The following is an example of the response.</span></span>

> <span data-ttu-id="661d4-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="661d4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
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
  "categories": null,
  "detail": {
    "company": {
      "displayName": "Adventureworks Ltd.",
      "pronunciation": null,
      "department": "Consulting",
      "officeLocation": "AW23/344",
      "address": {
        "type": "business",
        "postOfficeBox": null,
        "street": "123 Patriachy Ponds",
        "city": "Moscow",
        "state": null,
        "countryOrRegion": "Russian Federation",
        "postalCode": "RU-34621"
      },
      "webUrl": "https://www.adventureworks.com"
    },
    "description": null,
    "endMonthYear": null,
    "jobTitle": "Senior Product Branding Manager II",
    "role": "consulting",
    "startMonthYear": "datetime-value",
    "summary": null
  },
  "manager": null,
  "colleagues": null,
  "isCurrent": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update workposition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


