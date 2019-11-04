---
title: Atualizar tipo de recurso projectParticipation
description: Atualiza as propriedades de um objeto projectParticipation no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 3ee963f30289cb07c96860c2f0aeb5ec6096dac2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938412"
---
# <a name="update-projectparticipation"></a><span data-ttu-id="998f3-103">Atualizar projectparticipation</span><span class="sxs-lookup"><span data-stu-id="998f3-103">Update projectparticipation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="998f3-104">Atualiza as propriedades de um objeto [projectParticipation](../resources/projectParticipation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="998f3-104">Update the properties of a [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="998f3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="998f3-105">Permissions</span></span>

<span data-ttu-id="998f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="998f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="998f3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="998f3-108">Permission type</span></span>                        | <span data-ttu-id="998f3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="998f3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="998f3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="998f3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="998f3-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="998f3-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="998f3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="998f3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="998f3-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="998f3-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="998f3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="998f3-114">Application</span></span>                            | <span data-ttu-id="998f3-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="998f3-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="998f3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="998f3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="998f3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="998f3-117">Request headers</span></span>

| <span data-ttu-id="998f3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="998f3-118">Name</span></span>           |<span data-ttu-id="998f3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="998f3-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="998f3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="998f3-120">Authorization</span></span>  | <span data-ttu-id="998f3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="998f3-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="998f3-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="998f3-123">Content-Type</span></span>   | <span data-ttu-id="998f3-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="998f3-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="998f3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="998f3-126">Request body</span></span>

<span data-ttu-id="998f3-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="998f3-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="998f3-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="998f3-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="998f3-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="998f3-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="998f3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="998f3-130">Property</span></span>     | <span data-ttu-id="998f3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="998f3-131">Type</span></span>                                                     | <span data-ttu-id="998f3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="998f3-132">Description</span></span>                                                                                        |
|:-------------|:---------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
|<span data-ttu-id="998f3-133">categories</span><span class="sxs-lookup"><span data-stu-id="998f3-133">categories</span></span>    |<span data-ttu-id="998f3-134">String collection</span><span class="sxs-lookup"><span data-stu-id="998f3-134">String collection</span></span>                                         | <span data-ttu-id="998f3-135">Contém categorias que um usuário associou ao projeto (por exemplo: transformação digital, Rig óleo)</span><span class="sxs-lookup"><span data-stu-id="998f3-135">Contains categories a user has associated with the project (eg: digital transformation, oil rig)</span></span>   |
|<span data-ttu-id="998f3-136">clientes</span><span class="sxs-lookup"><span data-stu-id="998f3-136">client</span></span>        |[<span data-ttu-id="998f3-137">companyDetail</span><span class="sxs-lookup"><span data-stu-id="998f3-137">companyDetail</span></span>](../resources/companydetail.md)            | <span data-ttu-id="998f3-138">Contém informações detalhadas sobre o cliente para o qual o projeto foi.</span><span class="sxs-lookup"><span data-stu-id="998f3-138">Contains detailed information about the client the project was for.</span></span>                                |
|<span data-ttu-id="998f3-139">conhecidos</span><span class="sxs-lookup"><span data-stu-id="998f3-139">colleagues</span></span>    |<span data-ttu-id="998f3-140">coleção [relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="998f3-140">[relatedPerson](../resources/relatedperson.md) collection</span></span> | <span data-ttu-id="998f3-141">Pessoas que também trabalharam no projeto.</span><span class="sxs-lookup"><span data-stu-id="998f3-141">People that also worked on the project.</span></span>                                                            |
|<span data-ttu-id="998f3-142">detalhada</span><span class="sxs-lookup"><span data-stu-id="998f3-142">detail</span></span>        |[<span data-ttu-id="998f3-143">positionDetail</span><span class="sxs-lookup"><span data-stu-id="998f3-143">positionDetail</span></span>](../resources/positiondetail.md)          | <span data-ttu-id="998f3-144">Contém detalhes sobre a função Users no projeto.</span><span class="sxs-lookup"><span data-stu-id="998f3-144">Contains detail about the users role on the project.</span></span>                                               |
|<span data-ttu-id="998f3-145">displayName</span><span class="sxs-lookup"><span data-stu-id="998f3-145">displayName</span></span>   |<span data-ttu-id="998f3-146">String</span><span class="sxs-lookup"><span data-stu-id="998f3-146">String</span></span>                                                    | <span data-ttu-id="998f3-147">Contém um nome amigável para o projeto.</span><span class="sxs-lookup"><span data-stu-id="998f3-147">Contains a friendly name for the project.</span></span>                                                          |
|<span data-ttu-id="998f3-148">responsáveis</span><span class="sxs-lookup"><span data-stu-id="998f3-148">sponsors</span></span>      |<span data-ttu-id="998f3-149">coleção [relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="998f3-149">[relatedPerson](../resources/relatedperson.md) collection</span></span> | <span data-ttu-id="998f3-150">Pessoa (pessoas) que patrocinau o projeto.</span><span class="sxs-lookup"><span data-stu-id="998f3-150">Person(People) who sponsored the project.</span></span>                                                          |

## <a name="response"></a><span data-ttu-id="998f3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="998f3-151">Response</span></span>

<span data-ttu-id="998f3-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [projectParticipation](../resources/projectparticipation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="998f3-152">If successful, this method returns a `200 OK` response code and an updated [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="998f3-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="998f3-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="998f3-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="998f3-154">Request</span></span>

<span data-ttu-id="998f3-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="998f3-155">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="998f3-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="998f3-156">Response</span></span>

<span data-ttu-id="998f3-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="998f3-157">The following is an example of the response.</span></span>

> <span data-ttu-id="998f3-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="998f3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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