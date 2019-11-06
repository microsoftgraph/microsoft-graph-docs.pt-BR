---
title: Atualizar tipo de recurso projectParticipation
description: Atualiza as propriedades de um objeto projectParticipation no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b18aeb9e56eb79ea2c6d2ce4b0b0160c71c47595
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997671"
---
# <a name="update-projectparticipation"></a><span data-ttu-id="582d8-103">Atualizar projectparticipation</span><span class="sxs-lookup"><span data-stu-id="582d8-103">Update projectparticipation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="582d8-104">Atualiza as propriedades de um objeto [projectParticipation](../resources/projectParticipation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="582d8-104">Update the properties of a [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="582d8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="582d8-105">Permissions</span></span>

<span data-ttu-id="582d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="582d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="582d8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="582d8-108">Permission type</span></span>                        | <span data-ttu-id="582d8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="582d8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="582d8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="582d8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="582d8-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="582d8-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="582d8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="582d8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="582d8-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="582d8-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="582d8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="582d8-114">Application</span></span>                            | <span data-ttu-id="582d8-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="582d8-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="582d8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="582d8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="582d8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="582d8-117">Request headers</span></span>

| <span data-ttu-id="582d8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="582d8-118">Name</span></span>           |<span data-ttu-id="582d8-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="582d8-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="582d8-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="582d8-120">Authorization</span></span>  | <span data-ttu-id="582d8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="582d8-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="582d8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="582d8-123">Content-Type</span></span>   | <span data-ttu-id="582d8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="582d8-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="582d8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="582d8-126">Request body</span></span>

<span data-ttu-id="582d8-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="582d8-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="582d8-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="582d8-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="582d8-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="582d8-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="582d8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="582d8-130">Property</span></span>     | <span data-ttu-id="582d8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="582d8-131">Type</span></span>                                                     | <span data-ttu-id="582d8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="582d8-132">Description</span></span>                                                                                        |
|:-------------|:---------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
|<span data-ttu-id="582d8-133">categories</span><span class="sxs-lookup"><span data-stu-id="582d8-133">categories</span></span>    |<span data-ttu-id="582d8-134">String collection</span><span class="sxs-lookup"><span data-stu-id="582d8-134">String collection</span></span>                                         | <span data-ttu-id="582d8-135">Contém categorias que um usuário associou ao projeto (por exemplo: transformação digital, Rig óleo)</span><span class="sxs-lookup"><span data-stu-id="582d8-135">Contains categories a user has associated with the project (eg: digital transformation, oil rig)</span></span>   |
|<span data-ttu-id="582d8-136">clientes</span><span class="sxs-lookup"><span data-stu-id="582d8-136">client</span></span>        |[<span data-ttu-id="582d8-137">companyDetail</span><span class="sxs-lookup"><span data-stu-id="582d8-137">companyDetail</span></span>](../resources/companydetail.md)            | <span data-ttu-id="582d8-138">Contém informações detalhadas sobre o cliente para o qual o projeto foi.</span><span class="sxs-lookup"><span data-stu-id="582d8-138">Contains detailed information about the client the project was for.</span></span>                                |
|<span data-ttu-id="582d8-139">conhecidos</span><span class="sxs-lookup"><span data-stu-id="582d8-139">colleagues</span></span>    |<span data-ttu-id="582d8-140">coleção [relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="582d8-140">[relatedPerson](../resources/relatedperson.md) collection</span></span> | <span data-ttu-id="582d8-141">Pessoas que também trabalharam no projeto.</span><span class="sxs-lookup"><span data-stu-id="582d8-141">People that also worked on the project.</span></span>                                                            |
|<span data-ttu-id="582d8-142">detalhada</span><span class="sxs-lookup"><span data-stu-id="582d8-142">detail</span></span>        |[<span data-ttu-id="582d8-143">positionDetail</span><span class="sxs-lookup"><span data-stu-id="582d8-143">positionDetail</span></span>](../resources/positiondetail.md)          | <span data-ttu-id="582d8-144">Contém detalhes sobre a função Users no projeto.</span><span class="sxs-lookup"><span data-stu-id="582d8-144">Contains detail about the users role on the project.</span></span>                                               |
|<span data-ttu-id="582d8-145">displayName</span><span class="sxs-lookup"><span data-stu-id="582d8-145">displayName</span></span>   |<span data-ttu-id="582d8-146">String</span><span class="sxs-lookup"><span data-stu-id="582d8-146">String</span></span>                                                    | <span data-ttu-id="582d8-147">Contém um nome amigável para o projeto.</span><span class="sxs-lookup"><span data-stu-id="582d8-147">Contains a friendly name for the project.</span></span>                                                          |
|<span data-ttu-id="582d8-148">responsáveis</span><span class="sxs-lookup"><span data-stu-id="582d8-148">sponsors</span></span>      |<span data-ttu-id="582d8-149">coleção [relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="582d8-149">[relatedPerson](../resources/relatedperson.md) collection</span></span> | <span data-ttu-id="582d8-150">Pessoa (pessoas) que patrocinau o projeto.</span><span class="sxs-lookup"><span data-stu-id="582d8-150">Person(People) who sponsored the project.</span></span>                                                          |

## <a name="response"></a><span data-ttu-id="582d8-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="582d8-151">Response</span></span>

<span data-ttu-id="582d8-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [projectParticipation](../resources/projectparticipation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="582d8-152">If successful, this method returns a `200 OK` response code and an updated [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="582d8-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="582d8-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="582d8-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="582d8-154">Request</span></span>

<span data-ttu-id="582d8-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="582d8-155">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="582d8-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="582d8-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_projectparticipation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/projects/{id}
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "client": {
    "displayName": "displayName-value",
    "pronunciation": "pronunciation-value",
    "department": "department-value",
    "officeLocation": "officeLocation-value",
    "address": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "displayName": "displayName-value",
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "webUrl": "webUrl-value"
    },
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  },
  "colleagues": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ],
  "sponsors": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="582d8-157">C#</span><span class="sxs-lookup"><span data-stu-id="582d8-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="582d8-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="582d8-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="582d8-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="582d8-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="582d8-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="582d8-160">Response</span></span>

<span data-ttu-id="582d8-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="582d8-161">The following is an example of the response.</span></span>

> <span data-ttu-id="582d8-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="582d8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "client": {
    "displayName": "displayName-value",
    "pronunciation": "pronunciation-value",
    "department": "department-value",
    "officeLocation": "officeLocation-value",
    "address": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "displayName": "displayName-value",
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "webUrl": "webUrl-value"
    },
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  },
  "colleagues": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ],
  "sponsors": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update projectparticipation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
