---
title: Atualizar tipo de recurso projectParticipation
description: Atualiza as propriedades de um objeto projectParticipation no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b0aa9353a9e16929bd71f41f5328c0fdaf12c531
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454922"
---
# <a name="update-projectparticipation"></a><span data-ttu-id="bbc64-103">Atualizar projectparticipation</span><span class="sxs-lookup"><span data-stu-id="bbc64-103">Update projectparticipation</span></span>

<span data-ttu-id="bbc64-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bbc64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbc64-105">Atualiza as propriedades de um objeto [projectParticipation](../resources/projectParticipation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="bbc64-105">Update the properties of a [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bbc64-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbc64-106">Permissions</span></span>

<span data-ttu-id="bbc64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbc64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bbc64-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbc64-109">Permission type</span></span>                        | <span data-ttu-id="bbc64-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbc64-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bbc64-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbc64-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbc64-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bbc64-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="bbc64-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbc64-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbc64-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bbc64-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="bbc64-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbc64-115">Application</span></span>                            | <span data-ttu-id="bbc64-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbc64-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="bbc64-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbc64-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bbc64-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbc64-118">Request headers</span></span>

| <span data-ttu-id="bbc64-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bbc64-119">Name</span></span>           |<span data-ttu-id="bbc64-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbc64-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="bbc64-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbc64-121">Authorization</span></span>  | <span data-ttu-id="bbc64-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbc64-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="bbc64-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bbc64-124">Content-Type</span></span>   | <span data-ttu-id="bbc64-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbc64-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="bbc64-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbc64-127">Request body</span></span>

<span data-ttu-id="bbc64-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="bbc64-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bbc64-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="bbc64-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bbc64-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bbc64-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bbc64-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbc64-131">Property</span></span>     | <span data-ttu-id="bbc64-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbc64-132">Type</span></span>                                                     | <span data-ttu-id="bbc64-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbc64-133">Description</span></span>                                                                                        |
|:-------------|:---------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
|<span data-ttu-id="bbc64-134">categories</span><span class="sxs-lookup"><span data-stu-id="bbc64-134">categories</span></span>    |<span data-ttu-id="bbc64-135">String collection</span><span class="sxs-lookup"><span data-stu-id="bbc64-135">String collection</span></span>                                         | <span data-ttu-id="bbc64-136">Contém categorias que um usuário associou ao projeto (por exemplo: transformação digital, Rig óleo)</span><span class="sxs-lookup"><span data-stu-id="bbc64-136">Contains categories a user has associated with the project (eg: digital transformation, oil rig)</span></span>   |
|<span data-ttu-id="bbc64-137">clientes</span><span class="sxs-lookup"><span data-stu-id="bbc64-137">client</span></span>        |[<span data-ttu-id="bbc64-138">companyDetail</span><span class="sxs-lookup"><span data-stu-id="bbc64-138">companyDetail</span></span>](../resources/companydetail.md)            | <span data-ttu-id="bbc64-139">Contém informações detalhadas sobre o cliente para o qual o projeto foi.</span><span class="sxs-lookup"><span data-stu-id="bbc64-139">Contains detailed information about the client the project was for.</span></span>                                |
|<span data-ttu-id="bbc64-140">conhecidos</span><span class="sxs-lookup"><span data-stu-id="bbc64-140">colleagues</span></span>    |<span data-ttu-id="bbc64-141">coleção [relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="bbc64-141">[relatedPerson](../resources/relatedperson.md) collection</span></span> | <span data-ttu-id="bbc64-142">Pessoas que também trabalharam no projeto.</span><span class="sxs-lookup"><span data-stu-id="bbc64-142">People that also worked on the project.</span></span>                                                            |
|<span data-ttu-id="bbc64-143">detalhada</span><span class="sxs-lookup"><span data-stu-id="bbc64-143">detail</span></span>        |[<span data-ttu-id="bbc64-144">positionDetail</span><span class="sxs-lookup"><span data-stu-id="bbc64-144">positionDetail</span></span>](../resources/positiondetail.md)          | <span data-ttu-id="bbc64-145">Contém detalhes sobre a função Users no projeto.</span><span class="sxs-lookup"><span data-stu-id="bbc64-145">Contains detail about the users role on the project.</span></span>                                               |
|<span data-ttu-id="bbc64-146">displayName</span><span class="sxs-lookup"><span data-stu-id="bbc64-146">displayName</span></span>   |<span data-ttu-id="bbc64-147">String</span><span class="sxs-lookup"><span data-stu-id="bbc64-147">String</span></span>                                                    | <span data-ttu-id="bbc64-148">Contém um nome amigável para o projeto.</span><span class="sxs-lookup"><span data-stu-id="bbc64-148">Contains a friendly name for the project.</span></span>                                                          |
|<span data-ttu-id="bbc64-149">responsáveis</span><span class="sxs-lookup"><span data-stu-id="bbc64-149">sponsors</span></span>      |<span data-ttu-id="bbc64-150">coleção [relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="bbc64-150">[relatedPerson](../resources/relatedperson.md) collection</span></span> | <span data-ttu-id="bbc64-151">Pessoa (pessoas) que patrocinau o projeto.</span><span class="sxs-lookup"><span data-stu-id="bbc64-151">Person(People) who sponsored the project.</span></span>                                                          |

## <a name="response"></a><span data-ttu-id="bbc64-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbc64-152">Response</span></span>

<span data-ttu-id="bbc64-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [projectParticipation](../resources/projectparticipation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbc64-153">If successful, this method returns a `200 OK` response code and an updated [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bbc64-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bbc64-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bbc64-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbc64-155">Request</span></span>

<span data-ttu-id="bbc64-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbc64-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bbc64-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbc64-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bbc64-158">C#</span><span class="sxs-lookup"><span data-stu-id="bbc64-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bbc64-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbc64-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bbc64-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbc64-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bbc64-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbc64-161">Response</span></span>

<span data-ttu-id="bbc64-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bbc64-162">The following is an example of the response.</span></span>

> <span data-ttu-id="bbc64-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbc64-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
